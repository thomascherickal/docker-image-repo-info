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
-	[`docker:20.10.15`](#docker201015)
-	[`docker:20.10.15-alpine3.15`](#docker201015-alpine315)
-	[`docker:20.10.15-dind`](#docker201015-dind)
-	[`docker:20.10.15-dind-alpine3.15`](#docker201015-dind-alpine315)
-	[`docker:20.10.15-dind-rootless`](#docker201015-dind-rootless)
-	[`docker:20.10.15-git`](#docker201015-git)
-	[`docker:20.10.15-windowsservercore`](#docker201015-windowsservercore)
-	[`docker:20.10.15-windowsservercore-1809`](#docker201015-windowsservercore-1809)
-	[`docker:20.10.15-windowsservercore-ltsc2022`](#docker201015-windowsservercore-ltsc2022)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:20`

```console
$ docker pull docker@sha256:d11ece2878a6f8efbced93964e6ae22aa21721bc0efd9ef2e7e28685859d49d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:e52c95a544fa26c6d8577ea62596849143f4678d1086b52197e58bf77dc2a11b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93815417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea969625ebd2ada93d5e0cdeae98952b015d2a9521ecd793edf6a128939eab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e18aeb402936db9a724855ca75c4dde8540fa1f71273aeadb2d3660800403a1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86081746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ba2f3b7c338f7b9900c78c4605f7ce24d7083f09155221c24eeac44437b973`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:fb9cc626282893e4c7af33821af0ea7f6f8349d06955fef47efed35d6dbfc518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:bfba7b914767c3e037a040f1d9f85ad723a8c1fa52c596c6b233226f9614eb0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100557649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38003cc3a7ba9abd5e2a3f94c797f237f139118df6af1c0838a6d4ea021b0c6f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e5bc7537e92712bb526f60fed8a26a8f604275cd9991e86c16e2508946ccb7ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92707025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cd1505f2e8cc2cb33bbd004024038a207d64bc164d0e4a02784dd6d4ddbd51b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:aa45a0004d874e539af63bfad8db9ee7f00e847dae83be333a59cbed442751c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:b05edbab49df0c916810ee6ff4aab6bab3dc9518b4a8e1b960af37143c7320d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121065216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f1b93e523ccc3bb545467872a43f2a1bbc5a8a20a515cc7a9d0b643a52093a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
# Wed, 11 May 2022 01:30:58 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 01:30:58 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 01:30:59 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 01:31:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 01:31:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3274bbdde54bb4a48874b2ce035e92a09cb808e71aa62674d2b45feb1b8c335`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.2 MB (1161979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d1ddc5adfd1cb7677ff044ff73cb26aadc1c8bfd561d4d01bd5a277ea695bf`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4637389793458adbb0a60e604cf1a24c364b4ebfba0bf0dcb518c42d1bda9768`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f7d295b80db32082883f9fe59863d70d879876e123ec3d35965b8a5a0d8b99`  
		Last Modified: Wed, 11 May 2022 01:32:13 GMT  
		Size: 19.3 MB (19343874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb529ec47f8280e1c14cafe4c44f90ee830858c572841b0a981ab78b6e2550d3`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:86bdf6636db6a8b06847ac84644c7d50300c2955b2b200ce3aa55f3074ebecd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115065045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3e6f1e988d89dd418bf82197674b0e012f1aece1514f899a6397dd8a544668e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
# Wed, 11 May 2022 00:43:36 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 00:43:36 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 00:43:37 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 00:43:42 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 00:43:43 GMT
USER rootless
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b3985e0ad4d291eea7cf874cc318605bcf5da8770d51f4b65555611d8ec1cd`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.2 MB (1177961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7d124f6c1ceea4201be7da76786410ebeebbc1ca0754d98f312a30c3d9421f`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1273b4a7d40bb74302f237cb53eb0bcc54444ca383e15e5d33b3d060b5f98dd1`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2a3f703dc20a84ab20a7a95730da6579aac72a8c58bc0d24929d8617dc634c`  
		Last Modified: Wed, 11 May 2022 00:45:25 GMT  
		Size: 21.2 MB (21178440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66854ad6b8b792204d375a5f73dd9da3f91f4ef4bca9cce17479a18a62843ce8`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:804169b2f206a1eb99707a01c057413b0373a177e6cd0ebd79ca04134adc8981
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:d049d53085db2916345b06b72e04e061437b254300dc319e0f2dd932586e16b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100640719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a86e5919cce735123e1bfb4d72c987abb1427de078506828723a2a677f17b2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:31:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6528dd3b557823e0917ff9a89a5a3e96ab5db4beb04369fa74dedf54ec5d0f8`  
		Last Modified: Wed, 11 May 2022 01:32:31 GMT  
		Size: 6.8 MB (6825302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6408bd6587f86e51d8b510824e4d02f9234b12596cfe9a6c4d1f992bfb4c982a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (93017466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db57e40fdd155aef868beef5df895c1cac8a30a2b93dd69ef4fd363fe3daaa4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:51 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed14c2edfc4c1e09a3dc29020e19fad2d064256d93ffbc664d1f2a35beca119`  
		Last Modified: Wed, 11 May 2022 00:45:48 GMT  
		Size: 6.9 MB (6935720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:311d0808bb6738e1c87f394e539317e65289dcc8bbacafcea913752349f07e40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `docker:20-windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:1ad631482450acde3320d7cb23c8b56e3ea96af38436b696cf33e88ee48e678d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290644402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47174e8eafd1ce43847db1dfb8e1b645ad2c294426fff36ab98908475ae871d0`
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
# Wed, 11 May 2022 01:15:13 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:15:56 GMT
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
	-	`sha256:e4895cbb4f41e9db1f54c64e945e94ee0aa1521fabb64533954262a4e7e8ea32`  
		Last Modified: Wed, 11 May 2022 01:18:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71224d5ad52c5f62da3a2584b6ba45e398215f8497a5fd43b234190b0f240adc`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05d0103bd5ed165b25daa42f4def923ca4f54e66ead624eb85d3bcdc5194e8`  
		Last Modified: Wed, 11 May 2022 01:19:43 GMT  
		Size: 52.5 MB (52500443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:31dcdd35e3b51cab21a5e3595b1fb98bc2e0299c78f0429ea0a86c534cf3bab7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556828985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9049e8afec65e60c04dc8e34f79f883a885aff08b1652374efd8d306439bdf8b`
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
# Wed, 11 May 2022 01:17:08 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:17:09 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:18:09 GMT
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
	-	`sha256:60be3898d881db4d601a12aafc54eec7c0dfece1dca6bbd49a9b83d8960fd9b1`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d94933d82ab878efa8b78e97811840e787dfd21efb94ad17dbecaa40f6a93d`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3878d883ad2ec89939898edcd7a6861bb777c5a24b7563d515b0e4929191eb`  
		Last Modified: Wed, 11 May 2022 01:20:51 GMT  
		Size: 52.3 MB (52282860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:acfd53e7787f2304485e9cb5dbfab73c9e87a9a48bf42e7cbb0004da6eecc0d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:31dcdd35e3b51cab21a5e3595b1fb98bc2e0299c78f0429ea0a86c534cf3bab7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556828985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9049e8afec65e60c04dc8e34f79f883a885aff08b1652374efd8d306439bdf8b`
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
# Wed, 11 May 2022 01:17:08 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:17:09 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:18:09 GMT
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
	-	`sha256:60be3898d881db4d601a12aafc54eec7c0dfece1dca6bbd49a9b83d8960fd9b1`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d94933d82ab878efa8b78e97811840e787dfd21efb94ad17dbecaa40f6a93d`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3878d883ad2ec89939898edcd7a6861bb777c5a24b7563d515b0e4929191eb`  
		Last Modified: Wed, 11 May 2022 01:20:51 GMT  
		Size: 52.3 MB (52282860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:1ff3efb884e46bf756076aca17d89bc267b6ee0d739e19354c5e20a54962e31a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `docker:20-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:1ad631482450acde3320d7cb23c8b56e3ea96af38436b696cf33e88ee48e678d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290644402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47174e8eafd1ce43847db1dfb8e1b645ad2c294426fff36ab98908475ae871d0`
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
# Wed, 11 May 2022 01:15:13 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:15:56 GMT
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
	-	`sha256:e4895cbb4f41e9db1f54c64e945e94ee0aa1521fabb64533954262a4e7e8ea32`  
		Last Modified: Wed, 11 May 2022 01:18:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71224d5ad52c5f62da3a2584b6ba45e398215f8497a5fd43b234190b0f240adc`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05d0103bd5ed165b25daa42f4def923ca4f54e66ead624eb85d3bcdc5194e8`  
		Last Modified: Wed, 11 May 2022 01:19:43 GMT  
		Size: 52.5 MB (52500443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:d11ece2878a6f8efbced93964e6ae22aa21721bc0efd9ef2e7e28685859d49d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:e52c95a544fa26c6d8577ea62596849143f4678d1086b52197e58bf77dc2a11b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93815417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea969625ebd2ada93d5e0cdeae98952b015d2a9521ecd793edf6a128939eab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e18aeb402936db9a724855ca75c4dde8540fa1f71273aeadb2d3660800403a1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86081746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ba2f3b7c338f7b9900c78c4605f7ce24d7083f09155221c24eeac44437b973`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:fb9cc626282893e4c7af33821af0ea7f6f8349d06955fef47efed35d6dbfc518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:bfba7b914767c3e037a040f1d9f85ad723a8c1fa52c596c6b233226f9614eb0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100557649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38003cc3a7ba9abd5e2a3f94c797f237f139118df6af1c0838a6d4ea021b0c6f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e5bc7537e92712bb526f60fed8a26a8f604275cd9991e86c16e2508946ccb7ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92707025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cd1505f2e8cc2cb33bbd004024038a207d64bc164d0e4a02784dd6d4ddbd51b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:aa45a0004d874e539af63bfad8db9ee7f00e847dae83be333a59cbed442751c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:b05edbab49df0c916810ee6ff4aab6bab3dc9518b4a8e1b960af37143c7320d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121065216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f1b93e523ccc3bb545467872a43f2a1bbc5a8a20a515cc7a9d0b643a52093a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
# Wed, 11 May 2022 01:30:58 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 01:30:58 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 01:30:59 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 01:31:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 01:31:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3274bbdde54bb4a48874b2ce035e92a09cb808e71aa62674d2b45feb1b8c335`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.2 MB (1161979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d1ddc5adfd1cb7677ff044ff73cb26aadc1c8bfd561d4d01bd5a277ea695bf`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4637389793458adbb0a60e604cf1a24c364b4ebfba0bf0dcb518c42d1bda9768`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f7d295b80db32082883f9fe59863d70d879876e123ec3d35965b8a5a0d8b99`  
		Last Modified: Wed, 11 May 2022 01:32:13 GMT  
		Size: 19.3 MB (19343874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb529ec47f8280e1c14cafe4c44f90ee830858c572841b0a981ab78b6e2550d3`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:86bdf6636db6a8b06847ac84644c7d50300c2955b2b200ce3aa55f3074ebecd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115065045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3e6f1e988d89dd418bf82197674b0e012f1aece1514f899a6397dd8a544668e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
# Wed, 11 May 2022 00:43:36 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 00:43:36 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 00:43:37 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 00:43:42 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 00:43:43 GMT
USER rootless
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b3985e0ad4d291eea7cf874cc318605bcf5da8770d51f4b65555611d8ec1cd`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.2 MB (1177961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7d124f6c1ceea4201be7da76786410ebeebbc1ca0754d98f312a30c3d9421f`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1273b4a7d40bb74302f237cb53eb0bcc54444ca383e15e5d33b3d060b5f98dd1`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2a3f703dc20a84ab20a7a95730da6579aac72a8c58bc0d24929d8617dc634c`  
		Last Modified: Wed, 11 May 2022 00:45:25 GMT  
		Size: 21.2 MB (21178440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66854ad6b8b792204d375a5f73dd9da3f91f4ef4bca9cce17479a18a62843ce8`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:804169b2f206a1eb99707a01c057413b0373a177e6cd0ebd79ca04134adc8981
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:d049d53085db2916345b06b72e04e061437b254300dc319e0f2dd932586e16b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100640719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a86e5919cce735123e1bfb4d72c987abb1427de078506828723a2a677f17b2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:31:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6528dd3b557823e0917ff9a89a5a3e96ab5db4beb04369fa74dedf54ec5d0f8`  
		Last Modified: Wed, 11 May 2022 01:32:31 GMT  
		Size: 6.8 MB (6825302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6408bd6587f86e51d8b510824e4d02f9234b12596cfe9a6c4d1f992bfb4c982a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (93017466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db57e40fdd155aef868beef5df895c1cac8a30a2b93dd69ef4fd363fe3daaa4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:51 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed14c2edfc4c1e09a3dc29020e19fad2d064256d93ffbc664d1f2a35beca119`  
		Last Modified: Wed, 11 May 2022 00:45:48 GMT  
		Size: 6.9 MB (6935720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:311d0808bb6738e1c87f394e539317e65289dcc8bbacafcea913752349f07e40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:1ad631482450acde3320d7cb23c8b56e3ea96af38436b696cf33e88ee48e678d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290644402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47174e8eafd1ce43847db1dfb8e1b645ad2c294426fff36ab98908475ae871d0`
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
# Wed, 11 May 2022 01:15:13 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:15:56 GMT
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
	-	`sha256:e4895cbb4f41e9db1f54c64e945e94ee0aa1521fabb64533954262a4e7e8ea32`  
		Last Modified: Wed, 11 May 2022 01:18:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71224d5ad52c5f62da3a2584b6ba45e398215f8497a5fd43b234190b0f240adc`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05d0103bd5ed165b25daa42f4def923ca4f54e66ead624eb85d3bcdc5194e8`  
		Last Modified: Wed, 11 May 2022 01:19:43 GMT  
		Size: 52.5 MB (52500443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:31dcdd35e3b51cab21a5e3595b1fb98bc2e0299c78f0429ea0a86c534cf3bab7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556828985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9049e8afec65e60c04dc8e34f79f883a885aff08b1652374efd8d306439bdf8b`
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
# Wed, 11 May 2022 01:17:08 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:17:09 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:18:09 GMT
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
	-	`sha256:60be3898d881db4d601a12aafc54eec7c0dfece1dca6bbd49a9b83d8960fd9b1`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d94933d82ab878efa8b78e97811840e787dfd21efb94ad17dbecaa40f6a93d`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3878d883ad2ec89939898edcd7a6861bb777c5a24b7563d515b0e4929191eb`  
		Last Modified: Wed, 11 May 2022 01:20:51 GMT  
		Size: 52.3 MB (52282860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:acfd53e7787f2304485e9cb5dbfab73c9e87a9a48bf42e7cbb0004da6eecc0d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:31dcdd35e3b51cab21a5e3595b1fb98bc2e0299c78f0429ea0a86c534cf3bab7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556828985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9049e8afec65e60c04dc8e34f79f883a885aff08b1652374efd8d306439bdf8b`
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
# Wed, 11 May 2022 01:17:08 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:17:09 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:18:09 GMT
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
	-	`sha256:60be3898d881db4d601a12aafc54eec7c0dfece1dca6bbd49a9b83d8960fd9b1`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d94933d82ab878efa8b78e97811840e787dfd21efb94ad17dbecaa40f6a93d`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3878d883ad2ec89939898edcd7a6861bb777c5a24b7563d515b0e4929191eb`  
		Last Modified: Wed, 11 May 2022 01:20:51 GMT  
		Size: 52.3 MB (52282860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:1ff3efb884e46bf756076aca17d89bc267b6ee0d739e19354c5e20a54962e31a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `docker:20.10-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:1ad631482450acde3320d7cb23c8b56e3ea96af38436b696cf33e88ee48e678d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290644402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47174e8eafd1ce43847db1dfb8e1b645ad2c294426fff36ab98908475ae871d0`
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
# Wed, 11 May 2022 01:15:13 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:15:56 GMT
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
	-	`sha256:e4895cbb4f41e9db1f54c64e945e94ee0aa1521fabb64533954262a4e7e8ea32`  
		Last Modified: Wed, 11 May 2022 01:18:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71224d5ad52c5f62da3a2584b6ba45e398215f8497a5fd43b234190b0f240adc`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05d0103bd5ed165b25daa42f4def923ca4f54e66ead624eb85d3bcdc5194e8`  
		Last Modified: Wed, 11 May 2022 01:19:43 GMT  
		Size: 52.5 MB (52500443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.15`

```console
$ docker pull docker@sha256:d11ece2878a6f8efbced93964e6ae22aa21721bc0efd9ef2e7e28685859d49d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.15` - linux; amd64

```console
$ docker pull docker@sha256:e52c95a544fa26c6d8577ea62596849143f4678d1086b52197e58bf77dc2a11b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93815417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea969625ebd2ada93d5e0cdeae98952b015d2a9521ecd793edf6a128939eab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e18aeb402936db9a724855ca75c4dde8540fa1f71273aeadb2d3660800403a1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86081746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ba2f3b7c338f7b9900c78c4605f7ce24d7083f09155221c24eeac44437b973`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.15-alpine3.15`

```console
$ docker pull docker@sha256:d11ece2878a6f8efbced93964e6ae22aa21721bc0efd9ef2e7e28685859d49d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.15-alpine3.15` - linux; amd64

```console
$ docker pull docker@sha256:e52c95a544fa26c6d8577ea62596849143f4678d1086b52197e58bf77dc2a11b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93815417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea969625ebd2ada93d5e0cdeae98952b015d2a9521ecd793edf6a128939eab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.15-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e18aeb402936db9a724855ca75c4dde8540fa1f71273aeadb2d3660800403a1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86081746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ba2f3b7c338f7b9900c78c4605f7ce24d7083f09155221c24eeac44437b973`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.15-dind`

```console
$ docker pull docker@sha256:fb9cc626282893e4c7af33821af0ea7f6f8349d06955fef47efed35d6dbfc518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.15-dind` - linux; amd64

```console
$ docker pull docker@sha256:bfba7b914767c3e037a040f1d9f85ad723a8c1fa52c596c6b233226f9614eb0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100557649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38003cc3a7ba9abd5e2a3f94c797f237f139118df6af1c0838a6d4ea021b0c6f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.15-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e5bc7537e92712bb526f60fed8a26a8f604275cd9991e86c16e2508946ccb7ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92707025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cd1505f2e8cc2cb33bbd004024038a207d64bc164d0e4a02784dd6d4ddbd51b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.15-dind-alpine3.15`

```console
$ docker pull docker@sha256:fb9cc626282893e4c7af33821af0ea7f6f8349d06955fef47efed35d6dbfc518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.15-dind-alpine3.15` - linux; amd64

```console
$ docker pull docker@sha256:bfba7b914767c3e037a040f1d9f85ad723a8c1fa52c596c6b233226f9614eb0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100557649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38003cc3a7ba9abd5e2a3f94c797f237f139118df6af1c0838a6d4ea021b0c6f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.15-dind-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e5bc7537e92712bb526f60fed8a26a8f604275cd9991e86c16e2508946ccb7ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92707025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cd1505f2e8cc2cb33bbd004024038a207d64bc164d0e4a02784dd6d4ddbd51b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.15-dind-rootless`

```console
$ docker pull docker@sha256:aa45a0004d874e539af63bfad8db9ee7f00e847dae83be333a59cbed442751c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.15-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:b05edbab49df0c916810ee6ff4aab6bab3dc9518b4a8e1b960af37143c7320d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121065216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f1b93e523ccc3bb545467872a43f2a1bbc5a8a20a515cc7a9d0b643a52093a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
# Wed, 11 May 2022 01:30:58 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 01:30:58 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 01:30:59 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 01:31:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 01:31:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3274bbdde54bb4a48874b2ce035e92a09cb808e71aa62674d2b45feb1b8c335`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.2 MB (1161979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d1ddc5adfd1cb7677ff044ff73cb26aadc1c8bfd561d4d01bd5a277ea695bf`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4637389793458adbb0a60e604cf1a24c364b4ebfba0bf0dcb518c42d1bda9768`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f7d295b80db32082883f9fe59863d70d879876e123ec3d35965b8a5a0d8b99`  
		Last Modified: Wed, 11 May 2022 01:32:13 GMT  
		Size: 19.3 MB (19343874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb529ec47f8280e1c14cafe4c44f90ee830858c572841b0a981ab78b6e2550d3`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.15-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:86bdf6636db6a8b06847ac84644c7d50300c2955b2b200ce3aa55f3074ebecd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115065045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3e6f1e988d89dd418bf82197674b0e012f1aece1514f899a6397dd8a544668e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
# Wed, 11 May 2022 00:43:36 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 00:43:36 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 00:43:37 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 00:43:42 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 00:43:43 GMT
USER rootless
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b3985e0ad4d291eea7cf874cc318605bcf5da8770d51f4b65555611d8ec1cd`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.2 MB (1177961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7d124f6c1ceea4201be7da76786410ebeebbc1ca0754d98f312a30c3d9421f`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1273b4a7d40bb74302f237cb53eb0bcc54444ca383e15e5d33b3d060b5f98dd1`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2a3f703dc20a84ab20a7a95730da6579aac72a8c58bc0d24929d8617dc634c`  
		Last Modified: Wed, 11 May 2022 00:45:25 GMT  
		Size: 21.2 MB (21178440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66854ad6b8b792204d375a5f73dd9da3f91f4ef4bca9cce17479a18a62843ce8`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.15-git`

```console
$ docker pull docker@sha256:804169b2f206a1eb99707a01c057413b0373a177e6cd0ebd79ca04134adc8981
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.15-git` - linux; amd64

```console
$ docker pull docker@sha256:d049d53085db2916345b06b72e04e061437b254300dc319e0f2dd932586e16b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100640719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a86e5919cce735123e1bfb4d72c987abb1427de078506828723a2a677f17b2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:31:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6528dd3b557823e0917ff9a89a5a3e96ab5db4beb04369fa74dedf54ec5d0f8`  
		Last Modified: Wed, 11 May 2022 01:32:31 GMT  
		Size: 6.8 MB (6825302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.15-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6408bd6587f86e51d8b510824e4d02f9234b12596cfe9a6c4d1f992bfb4c982a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (93017466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db57e40fdd155aef868beef5df895c1cac8a30a2b93dd69ef4fd363fe3daaa4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:51 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed14c2edfc4c1e09a3dc29020e19fad2d064256d93ffbc664d1f2a35beca119`  
		Last Modified: Wed, 11 May 2022 00:45:48 GMT  
		Size: 6.9 MB (6935720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.15-windowsservercore`

```console
$ docker pull docker@sha256:311d0808bb6738e1c87f394e539317e65289dcc8bbacafcea913752349f07e40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `docker:20.10.15-windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:1ad631482450acde3320d7cb23c8b56e3ea96af38436b696cf33e88ee48e678d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290644402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47174e8eafd1ce43847db1dfb8e1b645ad2c294426fff36ab98908475ae871d0`
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
# Wed, 11 May 2022 01:15:13 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:15:56 GMT
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
	-	`sha256:e4895cbb4f41e9db1f54c64e945e94ee0aa1521fabb64533954262a4e7e8ea32`  
		Last Modified: Wed, 11 May 2022 01:18:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71224d5ad52c5f62da3a2584b6ba45e398215f8497a5fd43b234190b0f240adc`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05d0103bd5ed165b25daa42f4def923ca4f54e66ead624eb85d3bcdc5194e8`  
		Last Modified: Wed, 11 May 2022 01:19:43 GMT  
		Size: 52.5 MB (52500443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.15-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:31dcdd35e3b51cab21a5e3595b1fb98bc2e0299c78f0429ea0a86c534cf3bab7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556828985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9049e8afec65e60c04dc8e34f79f883a885aff08b1652374efd8d306439bdf8b`
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
# Wed, 11 May 2022 01:17:08 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:17:09 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:18:09 GMT
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
	-	`sha256:60be3898d881db4d601a12aafc54eec7c0dfece1dca6bbd49a9b83d8960fd9b1`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d94933d82ab878efa8b78e97811840e787dfd21efb94ad17dbecaa40f6a93d`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3878d883ad2ec89939898edcd7a6861bb777c5a24b7563d515b0e4929191eb`  
		Last Modified: Wed, 11 May 2022 01:20:51 GMT  
		Size: 52.3 MB (52282860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.15-windowsservercore-1809`

```console
$ docker pull docker@sha256:acfd53e7787f2304485e9cb5dbfab73c9e87a9a48bf42e7cbb0004da6eecc0d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `docker:20.10.15-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:31dcdd35e3b51cab21a5e3595b1fb98bc2e0299c78f0429ea0a86c534cf3bab7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556828985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9049e8afec65e60c04dc8e34f79f883a885aff08b1652374efd8d306439bdf8b`
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
# Wed, 11 May 2022 01:17:08 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:17:09 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:18:09 GMT
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
	-	`sha256:60be3898d881db4d601a12aafc54eec7c0dfece1dca6bbd49a9b83d8960fd9b1`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d94933d82ab878efa8b78e97811840e787dfd21efb94ad17dbecaa40f6a93d`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3878d883ad2ec89939898edcd7a6861bb777c5a24b7563d515b0e4929191eb`  
		Last Modified: Wed, 11 May 2022 01:20:51 GMT  
		Size: 52.3 MB (52282860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.15-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:1ff3efb884e46bf756076aca17d89bc267b6ee0d739e19354c5e20a54962e31a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `docker:20.10.15-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:1ad631482450acde3320d7cb23c8b56e3ea96af38436b696cf33e88ee48e678d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290644402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47174e8eafd1ce43847db1dfb8e1b645ad2c294426fff36ab98908475ae871d0`
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
# Wed, 11 May 2022 01:15:13 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:15:56 GMT
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
	-	`sha256:e4895cbb4f41e9db1f54c64e945e94ee0aa1521fabb64533954262a4e7e8ea32`  
		Last Modified: Wed, 11 May 2022 01:18:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71224d5ad52c5f62da3a2584b6ba45e398215f8497a5fd43b234190b0f240adc`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05d0103bd5ed165b25daa42f4def923ca4f54e66ead624eb85d3bcdc5194e8`  
		Last Modified: Wed, 11 May 2022 01:19:43 GMT  
		Size: 52.5 MB (52500443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:fb9cc626282893e4c7af33821af0ea7f6f8349d06955fef47efed35d6dbfc518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:bfba7b914767c3e037a040f1d9f85ad723a8c1fa52c596c6b233226f9614eb0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100557649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38003cc3a7ba9abd5e2a3f94c797f237f139118df6af1c0838a6d4ea021b0c6f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e5bc7537e92712bb526f60fed8a26a8f604275cd9991e86c16e2508946ccb7ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92707025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cd1505f2e8cc2cb33bbd004024038a207d64bc164d0e4a02784dd6d4ddbd51b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:aa45a0004d874e539af63bfad8db9ee7f00e847dae83be333a59cbed442751c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:b05edbab49df0c916810ee6ff4aab6bab3dc9518b4a8e1b960af37143c7320d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121065216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f1b93e523ccc3bb545467872a43f2a1bbc5a8a20a515cc7a9d0b643a52093a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
# Wed, 11 May 2022 01:30:58 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 01:30:58 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 01:30:59 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 01:31:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 01:31:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3274bbdde54bb4a48874b2ce035e92a09cb808e71aa62674d2b45feb1b8c335`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.2 MB (1161979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d1ddc5adfd1cb7677ff044ff73cb26aadc1c8bfd561d4d01bd5a277ea695bf`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4637389793458adbb0a60e604cf1a24c364b4ebfba0bf0dcb518c42d1bda9768`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f7d295b80db32082883f9fe59863d70d879876e123ec3d35965b8a5a0d8b99`  
		Last Modified: Wed, 11 May 2022 01:32:13 GMT  
		Size: 19.3 MB (19343874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb529ec47f8280e1c14cafe4c44f90ee830858c572841b0a981ab78b6e2550d3`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:86bdf6636db6a8b06847ac84644c7d50300c2955b2b200ce3aa55f3074ebecd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115065045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3e6f1e988d89dd418bf82197674b0e012f1aece1514f899a6397dd8a544668e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
# Wed, 11 May 2022 00:43:36 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 00:43:36 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 00:43:37 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 00:43:42 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 00:43:43 GMT
USER rootless
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b3985e0ad4d291eea7cf874cc318605bcf5da8770d51f4b65555611d8ec1cd`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.2 MB (1177961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7d124f6c1ceea4201be7da76786410ebeebbc1ca0754d98f312a30c3d9421f`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1273b4a7d40bb74302f237cb53eb0bcc54444ca383e15e5d33b3d060b5f98dd1`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2a3f703dc20a84ab20a7a95730da6579aac72a8c58bc0d24929d8617dc634c`  
		Last Modified: Wed, 11 May 2022 00:45:25 GMT  
		Size: 21.2 MB (21178440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66854ad6b8b792204d375a5f73dd9da3f91f4ef4bca9cce17479a18a62843ce8`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:804169b2f206a1eb99707a01c057413b0373a177e6cd0ebd79ca04134adc8981
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:d049d53085db2916345b06b72e04e061437b254300dc319e0f2dd932586e16b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100640719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a86e5919cce735123e1bfb4d72c987abb1427de078506828723a2a677f17b2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:31:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6528dd3b557823e0917ff9a89a5a3e96ab5db4beb04369fa74dedf54ec5d0f8`  
		Last Modified: Wed, 11 May 2022 01:32:31 GMT  
		Size: 6.8 MB (6825302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6408bd6587f86e51d8b510824e4d02f9234b12596cfe9a6c4d1f992bfb4c982a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (93017466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db57e40fdd155aef868beef5df895c1cac8a30a2b93dd69ef4fd363fe3daaa4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:51 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed14c2edfc4c1e09a3dc29020e19fad2d064256d93ffbc664d1f2a35beca119`  
		Last Modified: Wed, 11 May 2022 00:45:48 GMT  
		Size: 6.9 MB (6935720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:d11ece2878a6f8efbced93964e6ae22aa21721bc0efd9ef2e7e28685859d49d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:e52c95a544fa26c6d8577ea62596849143f4678d1086b52197e58bf77dc2a11b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93815417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea969625ebd2ada93d5e0cdeae98952b015d2a9521ecd793edf6a128939eab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e18aeb402936db9a724855ca75c4dde8540fa1f71273aeadb2d3660800403a1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86081746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42ba2f3b7c338f7b9900c78c4605f7ce24d7083f09155221c24eeac44437b973`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:311d0808bb6738e1c87f394e539317e65289dcc8bbacafcea913752349f07e40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `docker:windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:1ad631482450acde3320d7cb23c8b56e3ea96af38436b696cf33e88ee48e678d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290644402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47174e8eafd1ce43847db1dfb8e1b645ad2c294426fff36ab98908475ae871d0`
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
# Wed, 11 May 2022 01:15:13 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:15:56 GMT
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
	-	`sha256:e4895cbb4f41e9db1f54c64e945e94ee0aa1521fabb64533954262a4e7e8ea32`  
		Last Modified: Wed, 11 May 2022 01:18:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71224d5ad52c5f62da3a2584b6ba45e398215f8497a5fd43b234190b0f240adc`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05d0103bd5ed165b25daa42f4def923ca4f54e66ead624eb85d3bcdc5194e8`  
		Last Modified: Wed, 11 May 2022 01:19:43 GMT  
		Size: 52.5 MB (52500443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:31dcdd35e3b51cab21a5e3595b1fb98bc2e0299c78f0429ea0a86c534cf3bab7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556828985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9049e8afec65e60c04dc8e34f79f883a885aff08b1652374efd8d306439bdf8b`
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
# Wed, 11 May 2022 01:17:08 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:17:09 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:18:09 GMT
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
	-	`sha256:60be3898d881db4d601a12aafc54eec7c0dfece1dca6bbd49a9b83d8960fd9b1`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d94933d82ab878efa8b78e97811840e787dfd21efb94ad17dbecaa40f6a93d`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3878d883ad2ec89939898edcd7a6861bb777c5a24b7563d515b0e4929191eb`  
		Last Modified: Wed, 11 May 2022 01:20:51 GMT  
		Size: 52.3 MB (52282860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:acfd53e7787f2304485e9cb5dbfab73c9e87a9a48bf42e7cbb0004da6eecc0d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:31dcdd35e3b51cab21a5e3595b1fb98bc2e0299c78f0429ea0a86c534cf3bab7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556828985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9049e8afec65e60c04dc8e34f79f883a885aff08b1652374efd8d306439bdf8b`
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
# Wed, 11 May 2022 01:17:08 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:17:09 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:18:09 GMT
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
	-	`sha256:60be3898d881db4d601a12aafc54eec7c0dfece1dca6bbd49a9b83d8960fd9b1`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d94933d82ab878efa8b78e97811840e787dfd21efb94ad17dbecaa40f6a93d`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3878d883ad2ec89939898edcd7a6861bb777c5a24b7563d515b0e4929191eb`  
		Last Modified: Wed, 11 May 2022 01:20:51 GMT  
		Size: 52.3 MB (52282860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:1ff3efb884e46bf756076aca17d89bc267b6ee0d739e19354c5e20a54962e31a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull docker@sha256:1ad631482450acde3320d7cb23c8b56e3ea96af38436b696cf33e88ee48e678d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2290644402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47174e8eafd1ce43847db1dfb8e1b645ad2c294426fff36ab98908475ae871d0`
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
# Wed, 11 May 2022 01:15:13 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:15:56 GMT
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
	-	`sha256:e4895cbb4f41e9db1f54c64e945e94ee0aa1521fabb64533954262a4e7e8ea32`  
		Last Modified: Wed, 11 May 2022 01:18:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71224d5ad52c5f62da3a2584b6ba45e398215f8497a5fd43b234190b0f240adc`  
		Last Modified: Wed, 11 May 2022 01:18:49 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05d0103bd5ed165b25daa42f4def923ca4f54e66ead624eb85d3bcdc5194e8`  
		Last Modified: Wed, 11 May 2022 01:19:43 GMT  
		Size: 52.5 MB (52500443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
