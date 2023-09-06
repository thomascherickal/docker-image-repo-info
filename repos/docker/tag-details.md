<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:23`](#docker23)
-	[`docker:23-cli`](#docker23-cli)
-	[`docker:23-dind`](#docker23-dind)
-	[`docker:23-dind-rootless`](#docker23-dind-rootless)
-	[`docker:23-git`](#docker23-git)
-	[`docker:23-windowsservercore`](#docker23-windowsservercore)
-	[`docker:23-windowsservercore-1809`](#docker23-windowsservercore-1809)
-	[`docker:23-windowsservercore-ltsc2022`](#docker23-windowsservercore-ltsc2022)
-	[`docker:23.0`](#docker230)
-	[`docker:23.0-cli`](#docker230-cli)
-	[`docker:23.0-dind`](#docker230-dind)
-	[`docker:23.0-dind-rootless`](#docker230-dind-rootless)
-	[`docker:23.0-git`](#docker230-git)
-	[`docker:23.0-windowsservercore`](#docker230-windowsservercore)
-	[`docker:23.0-windowsservercore-1809`](#docker230-windowsservercore-1809)
-	[`docker:23.0-windowsservercore-ltsc2022`](#docker230-windowsservercore-ltsc2022)
-	[`docker:23.0.6`](#docker2306)
-	[`docker:23.0.6-alpine3.18`](#docker2306-alpine318)
-	[`docker:23.0.6-cli`](#docker2306-cli)
-	[`docker:23.0.6-cli-alpine3.18`](#docker2306-cli-alpine318)
-	[`docker:23.0.6-dind`](#docker2306-dind)
-	[`docker:23.0.6-dind-alpine3.18`](#docker2306-dind-alpine318)
-	[`docker:23.0.6-dind-rootless`](#docker2306-dind-rootless)
-	[`docker:23.0.6-git`](#docker2306-git)
-	[`docker:23.0.6-windowsservercore`](#docker2306-windowsservercore)
-	[`docker:23.0.6-windowsservercore-1809`](#docker2306-windowsservercore-1809)
-	[`docker:23.0.6-windowsservercore-ltsc2022`](#docker2306-windowsservercore-ltsc2022)
-	[`docker:24`](#docker24)
-	[`docker:24-cli`](#docker24-cli)
-	[`docker:24-dind`](#docker24-dind)
-	[`docker:24-dind-rootless`](#docker24-dind-rootless)
-	[`docker:24-git`](#docker24-git)
-	[`docker:24-windowsservercore`](#docker24-windowsservercore)
-	[`docker:24-windowsservercore-1809`](#docker24-windowsservercore-1809)
-	[`docker:24-windowsservercore-ltsc2022`](#docker24-windowsservercore-ltsc2022)
-	[`docker:24.0`](#docker240)
-	[`docker:24.0-cli`](#docker240-cli)
-	[`docker:24.0-dind`](#docker240-dind)
-	[`docker:24.0-dind-rootless`](#docker240-dind-rootless)
-	[`docker:24.0-git`](#docker240-git)
-	[`docker:24.0-windowsservercore`](#docker240-windowsservercore)
-	[`docker:24.0-windowsservercore-1809`](#docker240-windowsservercore-1809)
-	[`docker:24.0-windowsservercore-ltsc2022`](#docker240-windowsservercore-ltsc2022)
-	[`docker:24.0.6`](#docker2406)
-	[`docker:24.0.6-alpine3.18`](#docker2406-alpine318)
-	[`docker:24.0.6-cli`](#docker2406-cli)
-	[`docker:24.0.6-cli-alpine3.18`](#docker2406-cli-alpine318)
-	[`docker:24.0.6-dind`](#docker2406-dind)
-	[`docker:24.0.6-dind-alpine3.18`](#docker2406-dind-alpine318)
-	[`docker:24.0.6-dind-rootless`](#docker2406-dind-rootless)
-	[`docker:24.0.6-git`](#docker2406-git)
-	[`docker:24.0.6-windowsservercore`](#docker2406-windowsservercore)
-	[`docker:24.0.6-windowsservercore-1809`](#docker2406-windowsservercore-1809)
-	[`docker:24.0.6-windowsservercore-ltsc2022`](#docker2406-windowsservercore-ltsc2022)
-	[`docker:cli`](#dockercli)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:23`

```console
$ docker pull docker@sha256:97d1bb55b9bcd6ff473b502b8a3430746cff23f9dd91df2cbcea1fadc007b8ec
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23` - linux; amd64

```console
$ docker pull docker@sha256:e789c61591b754ac6a1ad9ff9d8ee48dc53647af18b138a221f9aa71905ed774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115697171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8200afa4a2a250a8e86fae94260261ea891330888e2a501c04616c3b412726ba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23` - unknown; unknown

```console
$ docker pull docker@sha256:34f3ebd0448c84c8873476834aa905c214fb383ec94980b20c927d5fc6297308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 KB (785793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ede7442e7bcd3e1d14cd5c4c20c8929599ed6fe7d79a80f56ed331ddc71bd3`

```dockerfile
```

-	Layers:
	-	`sha256:ed34957f1ab6901ab74ce916aaadbf43aca380b9e93d89606eb131fb6a3621c4`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 756.2 KB (756247 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e6f47f2c71b4df8f4ef8e667c6a81f7c431ef28cd5cc418e3910febc844ee03b`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 29.5 KB (29546 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2bb31b09e8ef8786e8fdf117e18f9a97fe8369ad6099892dfd50a22109b058e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107083571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4196298824a7c47ea599a8cd85c8878389f40df6ab7194c1cb0e19877771dc93`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23` - unknown; unknown

```console
$ docker pull docker@sha256:b36f12368dfd00f165320084fa74a9a8c2381e05d91f1527dcae7d097844a35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **786.1 KB (786071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff078e33805d986da2bdead56800dca7302eb183ccf46ad6949da81f2b78b7`

```dockerfile
```

-	Layers:
	-	`sha256:499fff7b33ce95b2bbab56c8ca3332333475e391b52152835411f30b6fecc4ed`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 756.5 KB (756460 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7c3f45b51df19196192d2404b6a1096698e512a2253f7d46d99f326e131b29b2`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 29.6 KB (29611 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23-cli`

```console
$ docker pull docker@sha256:9e323066d9872f3083e24860af94deede238b05863fdd00121c460ec11a5f456
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23-cli` - linux; amd64

```console
$ docker pull docker@sha256:c83029a5c07af4f9e1c8bb73bd2111068fb2add670badae58627e1ff3fd5b908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (56954335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a043b0abaae72e0bcc1530993d05015a31f0cccb551f007e8f46e2a10b2704aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 30 Aug 2023 23:04:20 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-cli` - unknown; unknown

```console
$ docker pull docker@sha256:ad725f437c52494010376b3406b4bfa6e064bd6412ae1ec5737b971985b2e120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.4 KB (544399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e74fe0f4e5d56e020d655ce92cd9ec07ac51f759f92425586f85f2fb9ad6639`

```dockerfile
```

-	Layers:
	-	`sha256:4dea5a62d32d2866d11a57bb559e187fe328aec0bf4e1247158ffa52f7a9c4ea`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 508.9 KB (508898 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ce02cf64aee9bbe470d22fcfbd67b9c3d155a40855b4cdd022d8a7fb0a5cddcf`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 35.5 KB (35501 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:608a468c67bfcb236363a1f99577dbb55b4e325411c655a3570f1a9833642978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52733861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97958fa18ed4c2f7d1be862766257a7dc3aab8b128ea11ce062cd3207fddae9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 30 Aug 2023 23:04:20 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-cli` - unknown; unknown

```console
$ docker pull docker@sha256:551ec7e76ca2574cd6cfec60d3a719af7dcc46f8f20d838f661a6baf50c3998c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.3 KB (544275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0e74c483a1ae02e356bb5d0de1023f4546092c07cd1c39c33621321b673ba2`

```dockerfile
```

-	Layers:
	-	`sha256:09cee0bbee438a8faa6c9f77c6a6751f9f464a63e0b2d862a2cefefb8b35cf4e`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 508.9 KB (508930 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:163fbd86889dba496c93a0c1df7c0c2e2758fb016ffb9b087d0dbb09f58bfe1a`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 35.3 KB (35345 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23-dind`

```console
$ docker pull docker@sha256:97d1bb55b9bcd6ff473b502b8a3430746cff23f9dd91df2cbcea1fadc007b8ec
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23-dind` - linux; amd64

```console
$ docker pull docker@sha256:e789c61591b754ac6a1ad9ff9d8ee48dc53647af18b138a221f9aa71905ed774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115697171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8200afa4a2a250a8e86fae94260261ea891330888e2a501c04616c3b412726ba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-dind` - unknown; unknown

```console
$ docker pull docker@sha256:34f3ebd0448c84c8873476834aa905c214fb383ec94980b20c927d5fc6297308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 KB (785793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ede7442e7bcd3e1d14cd5c4c20c8929599ed6fe7d79a80f56ed331ddc71bd3`

```dockerfile
```

-	Layers:
	-	`sha256:ed34957f1ab6901ab74ce916aaadbf43aca380b9e93d89606eb131fb6a3621c4`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 756.2 KB (756247 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e6f47f2c71b4df8f4ef8e667c6a81f7c431ef28cd5cc418e3910febc844ee03b`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 29.5 KB (29546 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2bb31b09e8ef8786e8fdf117e18f9a97fe8369ad6099892dfd50a22109b058e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107083571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4196298824a7c47ea599a8cd85c8878389f40df6ab7194c1cb0e19877771dc93`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-dind` - unknown; unknown

```console
$ docker pull docker@sha256:b36f12368dfd00f165320084fa74a9a8c2381e05d91f1527dcae7d097844a35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **786.1 KB (786071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff078e33805d986da2bdead56800dca7302eb183ccf46ad6949da81f2b78b7`

```dockerfile
```

-	Layers:
	-	`sha256:499fff7b33ce95b2bbab56c8ca3332333475e391b52152835411f30b6fecc4ed`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 756.5 KB (756460 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7c3f45b51df19196192d2404b6a1096698e512a2253f7d46d99f326e131b29b2`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 29.6 KB (29611 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23-dind-rootless`

```console
$ docker pull docker@sha256:0efb72251205581d4b207036415a510c3bc08526b8ab313426901b87a4ce60b9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5685cdce034a91d3d13846ab049e7e8e7758f8ebb24d6d697733f1944d3e819a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137408056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b7444e9281f477cb0c5803a6f598d3cb71d82be8d05563f3cb228c148d77044`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4afedb221fdf37ae0f1e9c505511ef57e6c5e0d47fdd221870dd730e2e109aa0`  
		Last Modified: Fri, 01 Sep 2023 02:51:23 GMT  
		Size: 1.4 MB (1362170 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18089b3504d00bb82232946c72809e37a7ffd275ccdbb782ff01cfff2b726b2c`  
		Last Modified: Fri, 01 Sep 2023 02:51:23 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b511fcf6d96c10e4425b245b9f675077e1cc852af71bf9a2193a86adacb32281`  
		Last Modified: Fri, 01 Sep 2023 02:51:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e53cfd232b06ea5e2d6b9985459f0232248392f329800cf0709cb7daec3228e`  
		Last Modified: Fri, 01 Sep 2023 02:51:24 GMT  
		Size: 20.3 MB (20347085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011a17494bfe75af1afdda085b158cabc695256f95e1e1f72140ec0b62c3d136`  
		Last Modified: Fri, 01 Sep 2023 02:51:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:1845e393b72e87398df05762530a78bfab55609a641f3d1c4b7c818ac0fe4c8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.0 KB (861953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af612d3539418ab94d1d9bd702f1518af14b50731fd782d912bfd642bc8f549f`

```dockerfile
```

-	Layers:
	-	`sha256:a641bf550c419e106c9e59888b84016322fd59b3f3bcfd2698d11faa89cb3d02`  
		Last Modified: Fri, 01 Sep 2023 02:51:22 GMT  
		Size: 831.2 KB (831171 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1178b9b6750fe46ad33765db0a23a8cd503f821825fcb33a2c4928eab4a323c2`  
		Last Modified: Fri, 01 Sep 2023 02:51:22 GMT  
		Size: 30.8 KB (30782 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4a9320d6595a3a08eb0f4fd5b76df08deb7a926bc292585da944319b055de843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130739347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4226b7ecd248fcaaec7d3da2d950134dd61168f9b86e81ace89077dbcd4d8d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5aa08e1d66cf2432aa61153ab1551e2b7f406fd1d3c6c05d2709730afda00f66`  
		Last Modified: Fri, 01 Sep 2023 02:52:39 GMT  
		Size: 1.4 MB (1413171 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabd9555022518db5cd6f9d6540f59399825142dddc3ea57fa3c3d9f060dfb98`  
		Last Modified: Fri, 01 Sep 2023 02:52:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8e6681c4f34283f2117fca926ffb857a61052040f56edeaef4c5004ce8e65f4`  
		Last Modified: Fri, 01 Sep 2023 02:52:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9674110f5c8d3611567531a96e45c6886846e55968142de390f79c78ee3b5e3a`  
		Last Modified: Fri, 01 Sep 2023 02:52:41 GMT  
		Size: 22.2 MB (22240981 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:147f87e3db6c8847ea6872129417eff4a723348a62e859eb403d7048a5a20cbb`  
		Last Modified: Fri, 01 Sep 2023 02:52:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:dadfcbcac2cfd433adc7b4142f881d8e12fef34e38715209087564bb244962d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.2 KB (862232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1b97e5b32958699e4888a985c6d305a5555fc451c26fe4212596b8441b64f5`

```dockerfile
```

-	Layers:
	-	`sha256:ffc1955cb4b44e1f9a25db9e7f684b5a6cb54c8d6e916ab85a68f3deb92acf53`  
		Last Modified: Fri, 01 Sep 2023 02:52:38 GMT  
		Size: 831.4 KB (831394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0df79fc0ed374ce587fe85f134939287cfe4a3e0fe4b54f01a1b9dd3fd8f3ca2`  
		Last Modified: Fri, 01 Sep 2023 02:52:38 GMT  
		Size: 30.8 KB (30838 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23-git`

```console
$ docker pull docker@sha256:83e8049e04c2718c1915865509a3c1577936167cbd1de85c36cab50f06d6158a
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23-git` - linux; amd64

```console
$ docker pull docker@sha256:a548f107683c1a230d9fa65eb4f946e832c1f01ffbc0bd87492e58b7ed13d3e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.6 MB (120632416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0db0a601716ff460bf55a690cda8026bafa81e5bdc2eb666a2281c7d86265ad2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0aeca6a8a19b71e703338c8fe23340a66ca5c380d35701ac59e94afef2b30f65`  
		Last Modified: Fri, 01 Sep 2023 02:51:20 GMT  
		Size: 4.9 MB (4935245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-git` - unknown; unknown

```console
$ docker pull docker@sha256:d37c5358697f46aa9539cd71cf6e0ca5d30f8925f4756623c27d4ce71a92e2d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **815.2 KB (815188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7196406e0901742bfea27bc23d981c673e59acdacf3088168942d639e14ed08`

```dockerfile
```

-	Layers:
	-	`sha256:9ab8565952088e198b34b7db5e3b19a16414ff446f6e68c5707c590bf1afb712`  
		Last Modified: Fri, 01 Sep 2023 02:51:19 GMT  
		Size: 802.6 KB (802551 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e72d2d339f795c73c6905ac75773b878a59b1398bd3a8349c5f43a575f24fca0`  
		Last Modified: Fri, 01 Sep 2023 02:51:19 GMT  
		Size: 12.6 KB (12637 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d294ac166eb13b6eccc30132ffdabe6217f75d44c7cf630910f943254f8a7be2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112105151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2f83da8abf36ae7ad9972703e20f59c17bc3dccf0e90796a3e175c7b39d9d8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37ff5d948beb8d82d08e6f72b6b24dbd122c4a5f6b426b7a52be8e3bac1b15ce`  
		Last Modified: Fri, 01 Sep 2023 02:53:00 GMT  
		Size: 5.0 MB (5021580 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-git` - unknown; unknown

```console
$ docker pull docker@sha256:345d4dbf2e504296a7f2f81a06513631bc25392ca02d35d6491f9cea89b1d0d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **813.2 KB (813230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27cd139fc6cf251de09a4f380a65b5ac0fa50536751f234273a0cfd0ffeb8b5e`

```dockerfile
```

-	Layers:
	-	`sha256:50affc58d2213269fbf0394e5da375165614cd748e09ec3feef48d1d8945744b`  
		Last Modified: Fri, 01 Sep 2023 02:52:59 GMT  
		Size: 802.8 KB (802762 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2872c68e47b18dfe8b7e529166d68d4bfbf2a4cab2d7096b61d25a62ab10d57d`  
		Last Modified: Fri, 01 Sep 2023 02:52:59 GMT  
		Size: 10.5 KB (10468 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23-windowsservercore`

```console
$ docker pull docker@sha256:16b462db085f654f4ce57d7f591511b51fb3487b1058dd3a3627a106c4a8bba4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `docker:23-windowsservercore` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:302c8cffca6b41d60001a2eeb79dfcd4e2c6b74b0c24542ebb056d134fe84856
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791531414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683a51df9326337cbc0c9952319ab1159ce9ed67588d7a7ab972566f6a2e512d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:33:24 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:33:25 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:33:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:19:00 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:19:26 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:19:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:19:27 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:19:28 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:19:54 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e5ba6630913747243f16c95b58df1d8c250c524ddb1d00459cc4bf045f5e8`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836e29352be49089f6845f1d186db438ccea79fd8fd40bbf8143e0cea1ad127b`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702b6bf769b3162353e4653d05135a310199dd75384e801d5a0cb95d586890b5`  
		Last Modified: Fri, 14 Jul 2023 00:40:08 GMT  
		Size: 17.3 MB (17326326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d0d2bd953a11e1c74f54978bc4093611fad5b861020a52a327da28a9f812dc`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c74d5986d7c82fe298f6d23c7c4544e2db166002f2e10f09be308a217261b5`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c23640ed904d02f39fef76ce3aa248259c086e63e507d36d74f4c0e723aa4a`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ecf6a7fd01be9cbd8ba541afab0f6306b745a7b37008c0bb0f94a68913bc92`  
		Last Modified: Wed, 19 Jul 2023 20:23:35 GMT  
		Size: 17.9 MB (17906240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1149f19c417c36254bc6373fd924306cb0c465b7de893f99d53bbe3199f0c30`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8277e4bd032f1a5dabb132a56166f0ef8f35b16afd528c5b5e562f2ea663cd`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0244d3417c443d7cf7fe8914a210d93912c0a9dd581d4d4360401c5f59d0a9cc`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbcfa9d38c0c9f88ccbf3a7a2fa17ce02db7a9d473759654ee87706d2eb62a0`  
		Last Modified: Wed, 19 Jul 2023 20:23:36 GMT  
		Size: 18.5 MB (18457963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:8357222c4f8e4d3732234517e75b5a6d1526bb4a82170773298cb21ffca4384e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993772576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152df6f6b9c8902e86ce2157e7d89769c70630aaa2b33c8cd0da55a4a5d5dbd0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:35:06 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:35:07 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:36:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:20:02 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:21:08 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:21:09 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:22:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe87c749ec26fddbab372ff211c7d036270aa32c5f863788554545b6dc0e65`  
		Last Modified: Fri, 14 Jul 2023 00:40:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c8a148bf7b449438042f9b5b344bc9b3784db6e578afac659f2305b045d8e`  
		Last Modified: Fri, 14 Jul 2023 00:40:23 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d683cfce8a83d53a6a06324c0925b0f0dfb4adbfc19d33a22b1a920fbb48b0`  
		Last Modified: Fri, 14 Jul 2023 00:40:26 GMT  
		Size: 17.5 MB (17492115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663a2d2385c12b481d9a3db965cc1ed948ab38099b811b538e66812c8505feee`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49641e7dc187958ecf1ee7e7db3b1e33e9d30865792ef4b3617c8517cb9205c1`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e903ad2079967f3995b8975f856ab254e20c71b6939750e7868a4895abaa48b`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3fbc75a4b445b862680804d0be73be40e7e3d222645eeab13072656c22ecab`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 17.9 MB (17900340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67553d91a2a75ff6c2e282f1a15d2ca7503ba7b09d274aa650ae462fb46febce`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9156e5832bc6c0ccff3abfa254f4d59660d9a66debdcb8da852b5c3f321f9e6e`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5deaf99b6677fbd2f70aea7d775c789f020ca96ac300c3c76b2037da170b69`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd399bde2e139306ec43944416825461f5d85624fcfece2717c14277eea7ef2`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 18.4 MB (18447902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore-1809`

```console
$ docker pull docker@sha256:b24ed464edcede82751e5e169ab51d6ffa769e2e478e93dc6f57cc82a24a9b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `docker:23-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:8357222c4f8e4d3732234517e75b5a6d1526bb4a82170773298cb21ffca4384e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993772576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152df6f6b9c8902e86ce2157e7d89769c70630aaa2b33c8cd0da55a4a5d5dbd0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:35:06 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:35:07 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:36:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:20:02 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:21:08 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:21:09 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:22:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe87c749ec26fddbab372ff211c7d036270aa32c5f863788554545b6dc0e65`  
		Last Modified: Fri, 14 Jul 2023 00:40:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c8a148bf7b449438042f9b5b344bc9b3784db6e578afac659f2305b045d8e`  
		Last Modified: Fri, 14 Jul 2023 00:40:23 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d683cfce8a83d53a6a06324c0925b0f0dfb4adbfc19d33a22b1a920fbb48b0`  
		Last Modified: Fri, 14 Jul 2023 00:40:26 GMT  
		Size: 17.5 MB (17492115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663a2d2385c12b481d9a3db965cc1ed948ab38099b811b538e66812c8505feee`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49641e7dc187958ecf1ee7e7db3b1e33e9d30865792ef4b3617c8517cb9205c1`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e903ad2079967f3995b8975f856ab254e20c71b6939750e7868a4895abaa48b`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3fbc75a4b445b862680804d0be73be40e7e3d222645eeab13072656c22ecab`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 17.9 MB (17900340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67553d91a2a75ff6c2e282f1a15d2ca7503ba7b09d274aa650ae462fb46febce`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9156e5832bc6c0ccff3abfa254f4d59660d9a66debdcb8da852b5c3f321f9e6e`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5deaf99b6677fbd2f70aea7d775c789f020ca96ac300c3c76b2037da170b69`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd399bde2e139306ec43944416825461f5d85624fcfece2717c14277eea7ef2`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 18.4 MB (18447902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:a04ad4a9927705cfb502baed04e6b7e183e700a9871ea1713168e224fec472cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `docker:23-windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:302c8cffca6b41d60001a2eeb79dfcd4e2c6b74b0c24542ebb056d134fe84856
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791531414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683a51df9326337cbc0c9952319ab1159ce9ed67588d7a7ab972566f6a2e512d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:33:24 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:33:25 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:33:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:19:00 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:19:26 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:19:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:19:27 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:19:28 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:19:54 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e5ba6630913747243f16c95b58df1d8c250c524ddb1d00459cc4bf045f5e8`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836e29352be49089f6845f1d186db438ccea79fd8fd40bbf8143e0cea1ad127b`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702b6bf769b3162353e4653d05135a310199dd75384e801d5a0cb95d586890b5`  
		Last Modified: Fri, 14 Jul 2023 00:40:08 GMT  
		Size: 17.3 MB (17326326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d0d2bd953a11e1c74f54978bc4093611fad5b861020a52a327da28a9f812dc`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c74d5986d7c82fe298f6d23c7c4544e2db166002f2e10f09be308a217261b5`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c23640ed904d02f39fef76ce3aa248259c086e63e507d36d74f4c0e723aa4a`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ecf6a7fd01be9cbd8ba541afab0f6306b745a7b37008c0bb0f94a68913bc92`  
		Last Modified: Wed, 19 Jul 2023 20:23:35 GMT  
		Size: 17.9 MB (17906240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1149f19c417c36254bc6373fd924306cb0c465b7de893f99d53bbe3199f0c30`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8277e4bd032f1a5dabb132a56166f0ef8f35b16afd528c5b5e562f2ea663cd`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0244d3417c443d7cf7fe8914a210d93912c0a9dd581d4d4360401c5f59d0a9cc`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbcfa9d38c0c9f88ccbf3a7a2fa17ce02db7a9d473759654ee87706d2eb62a0`  
		Last Modified: Wed, 19 Jul 2023 20:23:36 GMT  
		Size: 18.5 MB (18457963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0`

```console
$ docker pull docker@sha256:97d1bb55b9bcd6ff473b502b8a3430746cff23f9dd91df2cbcea1fadc007b8ec
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0` - linux; amd64

```console
$ docker pull docker@sha256:e789c61591b754ac6a1ad9ff9d8ee48dc53647af18b138a221f9aa71905ed774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115697171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8200afa4a2a250a8e86fae94260261ea891330888e2a501c04616c3b412726ba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0` - unknown; unknown

```console
$ docker pull docker@sha256:34f3ebd0448c84c8873476834aa905c214fb383ec94980b20c927d5fc6297308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 KB (785793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ede7442e7bcd3e1d14cd5c4c20c8929599ed6fe7d79a80f56ed331ddc71bd3`

```dockerfile
```

-	Layers:
	-	`sha256:ed34957f1ab6901ab74ce916aaadbf43aca380b9e93d89606eb131fb6a3621c4`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 756.2 KB (756247 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e6f47f2c71b4df8f4ef8e667c6a81f7c431ef28cd5cc418e3910febc844ee03b`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 29.5 KB (29546 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2bb31b09e8ef8786e8fdf117e18f9a97fe8369ad6099892dfd50a22109b058e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107083571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4196298824a7c47ea599a8cd85c8878389f40df6ab7194c1cb0e19877771dc93`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0` - unknown; unknown

```console
$ docker pull docker@sha256:b36f12368dfd00f165320084fa74a9a8c2381e05d91f1527dcae7d097844a35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **786.1 KB (786071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff078e33805d986da2bdead56800dca7302eb183ccf46ad6949da81f2b78b7`

```dockerfile
```

-	Layers:
	-	`sha256:499fff7b33ce95b2bbab56c8ca3332333475e391b52152835411f30b6fecc4ed`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 756.5 KB (756460 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7c3f45b51df19196192d2404b6a1096698e512a2253f7d46d99f326e131b29b2`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 29.6 KB (29611 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0-cli`

```console
$ docker pull docker@sha256:9e323066d9872f3083e24860af94deede238b05863fdd00121c460ec11a5f456
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0-cli` - linux; amd64

```console
$ docker pull docker@sha256:c83029a5c07af4f9e1c8bb73bd2111068fb2add670badae58627e1ff3fd5b908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (56954335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a043b0abaae72e0bcc1530993d05015a31f0cccb551f007e8f46e2a10b2704aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 30 Aug 2023 23:04:20 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0-cli` - unknown; unknown

```console
$ docker pull docker@sha256:ad725f437c52494010376b3406b4bfa6e064bd6412ae1ec5737b971985b2e120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.4 KB (544399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e74fe0f4e5d56e020d655ce92cd9ec07ac51f759f92425586f85f2fb9ad6639`

```dockerfile
```

-	Layers:
	-	`sha256:4dea5a62d32d2866d11a57bb559e187fe328aec0bf4e1247158ffa52f7a9c4ea`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 508.9 KB (508898 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ce02cf64aee9bbe470d22fcfbd67b9c3d155a40855b4cdd022d8a7fb0a5cddcf`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 35.5 KB (35501 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:608a468c67bfcb236363a1f99577dbb55b4e325411c655a3570f1a9833642978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52733861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97958fa18ed4c2f7d1be862766257a7dc3aab8b128ea11ce062cd3207fddae9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 30 Aug 2023 23:04:20 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0-cli` - unknown; unknown

```console
$ docker pull docker@sha256:551ec7e76ca2574cd6cfec60d3a719af7dcc46f8f20d838f661a6baf50c3998c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.3 KB (544275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0e74c483a1ae02e356bb5d0de1023f4546092c07cd1c39c33621321b673ba2`

```dockerfile
```

-	Layers:
	-	`sha256:09cee0bbee438a8faa6c9f77c6a6751f9f464a63e0b2d862a2cefefb8b35cf4e`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 508.9 KB (508930 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:163fbd86889dba496c93a0c1df7c0c2e2758fb016ffb9b087d0dbb09f58bfe1a`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 35.3 KB (35345 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0-dind`

```console
$ docker pull docker@sha256:97d1bb55b9bcd6ff473b502b8a3430746cff23f9dd91df2cbcea1fadc007b8ec
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:e789c61591b754ac6a1ad9ff9d8ee48dc53647af18b138a221f9aa71905ed774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115697171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8200afa4a2a250a8e86fae94260261ea891330888e2a501c04616c3b412726ba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0-dind` - unknown; unknown

```console
$ docker pull docker@sha256:34f3ebd0448c84c8873476834aa905c214fb383ec94980b20c927d5fc6297308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 KB (785793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ede7442e7bcd3e1d14cd5c4c20c8929599ed6fe7d79a80f56ed331ddc71bd3`

```dockerfile
```

-	Layers:
	-	`sha256:ed34957f1ab6901ab74ce916aaadbf43aca380b9e93d89606eb131fb6a3621c4`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 756.2 KB (756247 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e6f47f2c71b4df8f4ef8e667c6a81f7c431ef28cd5cc418e3910febc844ee03b`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 29.5 KB (29546 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2bb31b09e8ef8786e8fdf117e18f9a97fe8369ad6099892dfd50a22109b058e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107083571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4196298824a7c47ea599a8cd85c8878389f40df6ab7194c1cb0e19877771dc93`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0-dind` - unknown; unknown

```console
$ docker pull docker@sha256:b36f12368dfd00f165320084fa74a9a8c2381e05d91f1527dcae7d097844a35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **786.1 KB (786071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff078e33805d986da2bdead56800dca7302eb183ccf46ad6949da81f2b78b7`

```dockerfile
```

-	Layers:
	-	`sha256:499fff7b33ce95b2bbab56c8ca3332333475e391b52152835411f30b6fecc4ed`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 756.5 KB (756460 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7c3f45b51df19196192d2404b6a1096698e512a2253f7d46d99f326e131b29b2`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 29.6 KB (29611 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0-dind-rootless`

```console
$ docker pull docker@sha256:0efb72251205581d4b207036415a510c3bc08526b8ab313426901b87a4ce60b9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5685cdce034a91d3d13846ab049e7e8e7758f8ebb24d6d697733f1944d3e819a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137408056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b7444e9281f477cb0c5803a6f598d3cb71d82be8d05563f3cb228c148d77044`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4afedb221fdf37ae0f1e9c505511ef57e6c5e0d47fdd221870dd730e2e109aa0`  
		Last Modified: Fri, 01 Sep 2023 02:51:23 GMT  
		Size: 1.4 MB (1362170 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18089b3504d00bb82232946c72809e37a7ffd275ccdbb782ff01cfff2b726b2c`  
		Last Modified: Fri, 01 Sep 2023 02:51:23 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b511fcf6d96c10e4425b245b9f675077e1cc852af71bf9a2193a86adacb32281`  
		Last Modified: Fri, 01 Sep 2023 02:51:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e53cfd232b06ea5e2d6b9985459f0232248392f329800cf0709cb7daec3228e`  
		Last Modified: Fri, 01 Sep 2023 02:51:24 GMT  
		Size: 20.3 MB (20347085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011a17494bfe75af1afdda085b158cabc695256f95e1e1f72140ec0b62c3d136`  
		Last Modified: Fri, 01 Sep 2023 02:51:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:1845e393b72e87398df05762530a78bfab55609a641f3d1c4b7c818ac0fe4c8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.0 KB (861953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af612d3539418ab94d1d9bd702f1518af14b50731fd782d912bfd642bc8f549f`

```dockerfile
```

-	Layers:
	-	`sha256:a641bf550c419e106c9e59888b84016322fd59b3f3bcfd2698d11faa89cb3d02`  
		Last Modified: Fri, 01 Sep 2023 02:51:22 GMT  
		Size: 831.2 KB (831171 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1178b9b6750fe46ad33765db0a23a8cd503f821825fcb33a2c4928eab4a323c2`  
		Last Modified: Fri, 01 Sep 2023 02:51:22 GMT  
		Size: 30.8 KB (30782 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4a9320d6595a3a08eb0f4fd5b76df08deb7a926bc292585da944319b055de843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130739347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4226b7ecd248fcaaec7d3da2d950134dd61168f9b86e81ace89077dbcd4d8d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5aa08e1d66cf2432aa61153ab1551e2b7f406fd1d3c6c05d2709730afda00f66`  
		Last Modified: Fri, 01 Sep 2023 02:52:39 GMT  
		Size: 1.4 MB (1413171 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabd9555022518db5cd6f9d6540f59399825142dddc3ea57fa3c3d9f060dfb98`  
		Last Modified: Fri, 01 Sep 2023 02:52:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8e6681c4f34283f2117fca926ffb857a61052040f56edeaef4c5004ce8e65f4`  
		Last Modified: Fri, 01 Sep 2023 02:52:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9674110f5c8d3611567531a96e45c6886846e55968142de390f79c78ee3b5e3a`  
		Last Modified: Fri, 01 Sep 2023 02:52:41 GMT  
		Size: 22.2 MB (22240981 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:147f87e3db6c8847ea6872129417eff4a723348a62e859eb403d7048a5a20cbb`  
		Last Modified: Fri, 01 Sep 2023 02:52:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:dadfcbcac2cfd433adc7b4142f881d8e12fef34e38715209087564bb244962d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.2 KB (862232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1b97e5b32958699e4888a985c6d305a5555fc451c26fe4212596b8441b64f5`

```dockerfile
```

-	Layers:
	-	`sha256:ffc1955cb4b44e1f9a25db9e7f684b5a6cb54c8d6e916ab85a68f3deb92acf53`  
		Last Modified: Fri, 01 Sep 2023 02:52:38 GMT  
		Size: 831.4 KB (831394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0df79fc0ed374ce587fe85f134939287cfe4a3e0fe4b54f01a1b9dd3fd8f3ca2`  
		Last Modified: Fri, 01 Sep 2023 02:52:38 GMT  
		Size: 30.8 KB (30838 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0-git`

```console
$ docker pull docker@sha256:83e8049e04c2718c1915865509a3c1577936167cbd1de85c36cab50f06d6158a
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0-git` - linux; amd64

```console
$ docker pull docker@sha256:a548f107683c1a230d9fa65eb4f946e832c1f01ffbc0bd87492e58b7ed13d3e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.6 MB (120632416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0db0a601716ff460bf55a690cda8026bafa81e5bdc2eb666a2281c7d86265ad2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0aeca6a8a19b71e703338c8fe23340a66ca5c380d35701ac59e94afef2b30f65`  
		Last Modified: Fri, 01 Sep 2023 02:51:20 GMT  
		Size: 4.9 MB (4935245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0-git` - unknown; unknown

```console
$ docker pull docker@sha256:d37c5358697f46aa9539cd71cf6e0ca5d30f8925f4756623c27d4ce71a92e2d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **815.2 KB (815188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7196406e0901742bfea27bc23d981c673e59acdacf3088168942d639e14ed08`

```dockerfile
```

-	Layers:
	-	`sha256:9ab8565952088e198b34b7db5e3b19a16414ff446f6e68c5707c590bf1afb712`  
		Last Modified: Fri, 01 Sep 2023 02:51:19 GMT  
		Size: 802.6 KB (802551 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e72d2d339f795c73c6905ac75773b878a59b1398bd3a8349c5f43a575f24fca0`  
		Last Modified: Fri, 01 Sep 2023 02:51:19 GMT  
		Size: 12.6 KB (12637 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d294ac166eb13b6eccc30132ffdabe6217f75d44c7cf630910f943254f8a7be2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112105151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2f83da8abf36ae7ad9972703e20f59c17bc3dccf0e90796a3e175c7b39d9d8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37ff5d948beb8d82d08e6f72b6b24dbd122c4a5f6b426b7a52be8e3bac1b15ce`  
		Last Modified: Fri, 01 Sep 2023 02:53:00 GMT  
		Size: 5.0 MB (5021580 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0-git` - unknown; unknown

```console
$ docker pull docker@sha256:345d4dbf2e504296a7f2f81a06513631bc25392ca02d35d6491f9cea89b1d0d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **813.2 KB (813230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27cd139fc6cf251de09a4f380a65b5ac0fa50536751f234273a0cfd0ffeb8b5e`

```dockerfile
```

-	Layers:
	-	`sha256:50affc58d2213269fbf0394e5da375165614cd748e09ec3feef48d1d8945744b`  
		Last Modified: Fri, 01 Sep 2023 02:52:59 GMT  
		Size: 802.8 KB (802762 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2872c68e47b18dfe8b7e529166d68d4bfbf2a4cab2d7096b61d25a62ab10d57d`  
		Last Modified: Fri, 01 Sep 2023 02:52:59 GMT  
		Size: 10.5 KB (10468 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0-windowsservercore`

```console
$ docker pull docker@sha256:16b462db085f654f4ce57d7f591511b51fb3487b1058dd3a3627a106c4a8bba4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `docker:23.0-windowsservercore` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:302c8cffca6b41d60001a2eeb79dfcd4e2c6b74b0c24542ebb056d134fe84856
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791531414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683a51df9326337cbc0c9952319ab1159ce9ed67588d7a7ab972566f6a2e512d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:33:24 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:33:25 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:33:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:19:00 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:19:26 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:19:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:19:27 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:19:28 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:19:54 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e5ba6630913747243f16c95b58df1d8c250c524ddb1d00459cc4bf045f5e8`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836e29352be49089f6845f1d186db438ccea79fd8fd40bbf8143e0cea1ad127b`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702b6bf769b3162353e4653d05135a310199dd75384e801d5a0cb95d586890b5`  
		Last Modified: Fri, 14 Jul 2023 00:40:08 GMT  
		Size: 17.3 MB (17326326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d0d2bd953a11e1c74f54978bc4093611fad5b861020a52a327da28a9f812dc`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c74d5986d7c82fe298f6d23c7c4544e2db166002f2e10f09be308a217261b5`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c23640ed904d02f39fef76ce3aa248259c086e63e507d36d74f4c0e723aa4a`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ecf6a7fd01be9cbd8ba541afab0f6306b745a7b37008c0bb0f94a68913bc92`  
		Last Modified: Wed, 19 Jul 2023 20:23:35 GMT  
		Size: 17.9 MB (17906240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1149f19c417c36254bc6373fd924306cb0c465b7de893f99d53bbe3199f0c30`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8277e4bd032f1a5dabb132a56166f0ef8f35b16afd528c5b5e562f2ea663cd`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0244d3417c443d7cf7fe8914a210d93912c0a9dd581d4d4360401c5f59d0a9cc`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbcfa9d38c0c9f88ccbf3a7a2fa17ce02db7a9d473759654ee87706d2eb62a0`  
		Last Modified: Wed, 19 Jul 2023 20:23:36 GMT  
		Size: 18.5 MB (18457963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:8357222c4f8e4d3732234517e75b5a6d1526bb4a82170773298cb21ffca4384e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993772576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152df6f6b9c8902e86ce2157e7d89769c70630aaa2b33c8cd0da55a4a5d5dbd0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:35:06 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:35:07 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:36:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:20:02 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:21:08 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:21:09 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:22:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe87c749ec26fddbab372ff211c7d036270aa32c5f863788554545b6dc0e65`  
		Last Modified: Fri, 14 Jul 2023 00:40:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c8a148bf7b449438042f9b5b344bc9b3784db6e578afac659f2305b045d8e`  
		Last Modified: Fri, 14 Jul 2023 00:40:23 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d683cfce8a83d53a6a06324c0925b0f0dfb4adbfc19d33a22b1a920fbb48b0`  
		Last Modified: Fri, 14 Jul 2023 00:40:26 GMT  
		Size: 17.5 MB (17492115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663a2d2385c12b481d9a3db965cc1ed948ab38099b811b538e66812c8505feee`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49641e7dc187958ecf1ee7e7db3b1e33e9d30865792ef4b3617c8517cb9205c1`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e903ad2079967f3995b8975f856ab254e20c71b6939750e7868a4895abaa48b`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3fbc75a4b445b862680804d0be73be40e7e3d222645eeab13072656c22ecab`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 17.9 MB (17900340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67553d91a2a75ff6c2e282f1a15d2ca7503ba7b09d274aa650ae462fb46febce`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9156e5832bc6c0ccff3abfa254f4d59660d9a66debdcb8da852b5c3f321f9e6e`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5deaf99b6677fbd2f70aea7d775c789f020ca96ac300c3c76b2037da170b69`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd399bde2e139306ec43944416825461f5d85624fcfece2717c14277eea7ef2`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 18.4 MB (18447902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore-1809`

```console
$ docker pull docker@sha256:b24ed464edcede82751e5e169ab51d6ffa769e2e478e93dc6f57cc82a24a9b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `docker:23.0-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:8357222c4f8e4d3732234517e75b5a6d1526bb4a82170773298cb21ffca4384e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993772576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152df6f6b9c8902e86ce2157e7d89769c70630aaa2b33c8cd0da55a4a5d5dbd0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:35:06 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:35:07 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:36:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:20:02 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:21:08 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:21:09 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:22:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe87c749ec26fddbab372ff211c7d036270aa32c5f863788554545b6dc0e65`  
		Last Modified: Fri, 14 Jul 2023 00:40:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c8a148bf7b449438042f9b5b344bc9b3784db6e578afac659f2305b045d8e`  
		Last Modified: Fri, 14 Jul 2023 00:40:23 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d683cfce8a83d53a6a06324c0925b0f0dfb4adbfc19d33a22b1a920fbb48b0`  
		Last Modified: Fri, 14 Jul 2023 00:40:26 GMT  
		Size: 17.5 MB (17492115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663a2d2385c12b481d9a3db965cc1ed948ab38099b811b538e66812c8505feee`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49641e7dc187958ecf1ee7e7db3b1e33e9d30865792ef4b3617c8517cb9205c1`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e903ad2079967f3995b8975f856ab254e20c71b6939750e7868a4895abaa48b`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3fbc75a4b445b862680804d0be73be40e7e3d222645eeab13072656c22ecab`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 17.9 MB (17900340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67553d91a2a75ff6c2e282f1a15d2ca7503ba7b09d274aa650ae462fb46febce`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9156e5832bc6c0ccff3abfa254f4d59660d9a66debdcb8da852b5c3f321f9e6e`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5deaf99b6677fbd2f70aea7d775c789f020ca96ac300c3c76b2037da170b69`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd399bde2e139306ec43944416825461f5d85624fcfece2717c14277eea7ef2`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 18.4 MB (18447902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:a04ad4a9927705cfb502baed04e6b7e183e700a9871ea1713168e224fec472cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `docker:23.0-windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:302c8cffca6b41d60001a2eeb79dfcd4e2c6b74b0c24542ebb056d134fe84856
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791531414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683a51df9326337cbc0c9952319ab1159ce9ed67588d7a7ab972566f6a2e512d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:33:24 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:33:25 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:33:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:19:00 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:19:26 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:19:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:19:27 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:19:28 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:19:54 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e5ba6630913747243f16c95b58df1d8c250c524ddb1d00459cc4bf045f5e8`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836e29352be49089f6845f1d186db438ccea79fd8fd40bbf8143e0cea1ad127b`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702b6bf769b3162353e4653d05135a310199dd75384e801d5a0cb95d586890b5`  
		Last Modified: Fri, 14 Jul 2023 00:40:08 GMT  
		Size: 17.3 MB (17326326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d0d2bd953a11e1c74f54978bc4093611fad5b861020a52a327da28a9f812dc`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c74d5986d7c82fe298f6d23c7c4544e2db166002f2e10f09be308a217261b5`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c23640ed904d02f39fef76ce3aa248259c086e63e507d36d74f4c0e723aa4a`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ecf6a7fd01be9cbd8ba541afab0f6306b745a7b37008c0bb0f94a68913bc92`  
		Last Modified: Wed, 19 Jul 2023 20:23:35 GMT  
		Size: 17.9 MB (17906240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1149f19c417c36254bc6373fd924306cb0c465b7de893f99d53bbe3199f0c30`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8277e4bd032f1a5dabb132a56166f0ef8f35b16afd528c5b5e562f2ea663cd`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0244d3417c443d7cf7fe8914a210d93912c0a9dd581d4d4360401c5f59d0a9cc`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbcfa9d38c0c9f88ccbf3a7a2fa17ce02db7a9d473759654ee87706d2eb62a0`  
		Last Modified: Wed, 19 Jul 2023 20:23:36 GMT  
		Size: 18.5 MB (18457963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6`

```console
$ docker pull docker@sha256:97d1bb55b9bcd6ff473b502b8a3430746cff23f9dd91df2cbcea1fadc007b8ec
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0.6` - linux; amd64

```console
$ docker pull docker@sha256:e789c61591b754ac6a1ad9ff9d8ee48dc53647af18b138a221f9aa71905ed774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115697171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8200afa4a2a250a8e86fae94260261ea891330888e2a501c04616c3b412726ba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6` - unknown; unknown

```console
$ docker pull docker@sha256:34f3ebd0448c84c8873476834aa905c214fb383ec94980b20c927d5fc6297308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 KB (785793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ede7442e7bcd3e1d14cd5c4c20c8929599ed6fe7d79a80f56ed331ddc71bd3`

```dockerfile
```

-	Layers:
	-	`sha256:ed34957f1ab6901ab74ce916aaadbf43aca380b9e93d89606eb131fb6a3621c4`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 756.2 KB (756247 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e6f47f2c71b4df8f4ef8e667c6a81f7c431ef28cd5cc418e3910febc844ee03b`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 29.5 KB (29546 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0.6` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2bb31b09e8ef8786e8fdf117e18f9a97fe8369ad6099892dfd50a22109b058e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107083571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4196298824a7c47ea599a8cd85c8878389f40df6ab7194c1cb0e19877771dc93`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6` - unknown; unknown

```console
$ docker pull docker@sha256:b36f12368dfd00f165320084fa74a9a8c2381e05d91f1527dcae7d097844a35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **786.1 KB (786071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff078e33805d986da2bdead56800dca7302eb183ccf46ad6949da81f2b78b7`

```dockerfile
```

-	Layers:
	-	`sha256:499fff7b33ce95b2bbab56c8ca3332333475e391b52152835411f30b6fecc4ed`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 756.5 KB (756460 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7c3f45b51df19196192d2404b6a1096698e512a2253f7d46d99f326e131b29b2`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 29.6 KB (29611 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0.6-alpine3.18`

```console
$ docker pull docker@sha256:97d1bb55b9bcd6ff473b502b8a3430746cff23f9dd91df2cbcea1fadc007b8ec
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0.6-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:e789c61591b754ac6a1ad9ff9d8ee48dc53647af18b138a221f9aa71905ed774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115697171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8200afa4a2a250a8e86fae94260261ea891330888e2a501c04616c3b412726ba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-alpine3.18` - unknown; unknown

```console
$ docker pull docker@sha256:34f3ebd0448c84c8873476834aa905c214fb383ec94980b20c927d5fc6297308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 KB (785793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ede7442e7bcd3e1d14cd5c4c20c8929599ed6fe7d79a80f56ed331ddc71bd3`

```dockerfile
```

-	Layers:
	-	`sha256:ed34957f1ab6901ab74ce916aaadbf43aca380b9e93d89606eb131fb6a3621c4`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 756.2 KB (756247 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e6f47f2c71b4df8f4ef8e667c6a81f7c431ef28cd5cc418e3910febc844ee03b`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 29.5 KB (29546 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0.6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2bb31b09e8ef8786e8fdf117e18f9a97fe8369ad6099892dfd50a22109b058e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107083571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4196298824a7c47ea599a8cd85c8878389f40df6ab7194c1cb0e19877771dc93`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-alpine3.18` - unknown; unknown

```console
$ docker pull docker@sha256:b36f12368dfd00f165320084fa74a9a8c2381e05d91f1527dcae7d097844a35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **786.1 KB (786071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff078e33805d986da2bdead56800dca7302eb183ccf46ad6949da81f2b78b7`

```dockerfile
```

-	Layers:
	-	`sha256:499fff7b33ce95b2bbab56c8ca3332333475e391b52152835411f30b6fecc4ed`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 756.5 KB (756460 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7c3f45b51df19196192d2404b6a1096698e512a2253f7d46d99f326e131b29b2`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 29.6 KB (29611 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0.6-cli`

```console
$ docker pull docker@sha256:9e323066d9872f3083e24860af94deede238b05863fdd00121c460ec11a5f456
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0.6-cli` - linux; amd64

```console
$ docker pull docker@sha256:c83029a5c07af4f9e1c8bb73bd2111068fb2add670badae58627e1ff3fd5b908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (56954335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a043b0abaae72e0bcc1530993d05015a31f0cccb551f007e8f46e2a10b2704aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 30 Aug 2023 23:04:20 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-cli` - unknown; unknown

```console
$ docker pull docker@sha256:ad725f437c52494010376b3406b4bfa6e064bd6412ae1ec5737b971985b2e120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.4 KB (544399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e74fe0f4e5d56e020d655ce92cd9ec07ac51f759f92425586f85f2fb9ad6639`

```dockerfile
```

-	Layers:
	-	`sha256:4dea5a62d32d2866d11a57bb559e187fe328aec0bf4e1247158ffa52f7a9c4ea`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 508.9 KB (508898 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ce02cf64aee9bbe470d22fcfbd67b9c3d155a40855b4cdd022d8a7fb0a5cddcf`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 35.5 KB (35501 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0.6-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:608a468c67bfcb236363a1f99577dbb55b4e325411c655a3570f1a9833642978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52733861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97958fa18ed4c2f7d1be862766257a7dc3aab8b128ea11ce062cd3207fddae9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 30 Aug 2023 23:04:20 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-cli` - unknown; unknown

```console
$ docker pull docker@sha256:551ec7e76ca2574cd6cfec60d3a719af7dcc46f8f20d838f661a6baf50c3998c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.3 KB (544275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0e74c483a1ae02e356bb5d0de1023f4546092c07cd1c39c33621321b673ba2`

```dockerfile
```

-	Layers:
	-	`sha256:09cee0bbee438a8faa6c9f77c6a6751f9f464a63e0b2d862a2cefefb8b35cf4e`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 508.9 KB (508930 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:163fbd86889dba496c93a0c1df7c0c2e2758fb016ffb9b087d0dbb09f58bfe1a`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 35.3 KB (35345 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0.6-cli-alpine3.18`

```console
$ docker pull docker@sha256:9e323066d9872f3083e24860af94deede238b05863fdd00121c460ec11a5f456
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0.6-cli-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:c83029a5c07af4f9e1c8bb73bd2111068fb2add670badae58627e1ff3fd5b908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (56954335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a043b0abaae72e0bcc1530993d05015a31f0cccb551f007e8f46e2a10b2704aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 30 Aug 2023 23:04:20 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-cli-alpine3.18` - unknown; unknown

```console
$ docker pull docker@sha256:ad725f437c52494010376b3406b4bfa6e064bd6412ae1ec5737b971985b2e120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.4 KB (544399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e74fe0f4e5d56e020d655ce92cd9ec07ac51f759f92425586f85f2fb9ad6639`

```dockerfile
```

-	Layers:
	-	`sha256:4dea5a62d32d2866d11a57bb559e187fe328aec0bf4e1247158ffa52f7a9c4ea`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 508.9 KB (508898 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ce02cf64aee9bbe470d22fcfbd67b9c3d155a40855b4cdd022d8a7fb0a5cddcf`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 35.5 KB (35501 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0.6-cli-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:608a468c67bfcb236363a1f99577dbb55b4e325411c655a3570f1a9833642978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52733861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97958fa18ed4c2f7d1be862766257a7dc3aab8b128ea11ce062cd3207fddae9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Wed, 30 Aug 2023 23:04:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 30 Aug 2023 23:04:20 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 30 Aug 2023 23:04:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Aug 2023 23:04:20 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-cli-alpine3.18` - unknown; unknown

```console
$ docker pull docker@sha256:551ec7e76ca2574cd6cfec60d3a719af7dcc46f8f20d838f661a6baf50c3998c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.3 KB (544275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0e74c483a1ae02e356bb5d0de1023f4546092c07cd1c39c33621321b673ba2`

```dockerfile
```

-	Layers:
	-	`sha256:09cee0bbee438a8faa6c9f77c6a6751f9f464a63e0b2d862a2cefefb8b35cf4e`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 508.9 KB (508930 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:163fbd86889dba496c93a0c1df7c0c2e2758fb016ffb9b087d0dbb09f58bfe1a`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 35.3 KB (35345 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0.6-dind`

```console
$ docker pull docker@sha256:97d1bb55b9bcd6ff473b502b8a3430746cff23f9dd91df2cbcea1fadc007b8ec
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0.6-dind` - linux; amd64

```console
$ docker pull docker@sha256:e789c61591b754ac6a1ad9ff9d8ee48dc53647af18b138a221f9aa71905ed774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115697171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8200afa4a2a250a8e86fae94260261ea891330888e2a501c04616c3b412726ba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-dind` - unknown; unknown

```console
$ docker pull docker@sha256:34f3ebd0448c84c8873476834aa905c214fb383ec94980b20c927d5fc6297308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 KB (785793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ede7442e7bcd3e1d14cd5c4c20c8929599ed6fe7d79a80f56ed331ddc71bd3`

```dockerfile
```

-	Layers:
	-	`sha256:ed34957f1ab6901ab74ce916aaadbf43aca380b9e93d89606eb131fb6a3621c4`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 756.2 KB (756247 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e6f47f2c71b4df8f4ef8e667c6a81f7c431ef28cd5cc418e3910febc844ee03b`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 29.5 KB (29546 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0.6-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2bb31b09e8ef8786e8fdf117e18f9a97fe8369ad6099892dfd50a22109b058e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107083571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4196298824a7c47ea599a8cd85c8878389f40df6ab7194c1cb0e19877771dc93`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-dind` - unknown; unknown

```console
$ docker pull docker@sha256:b36f12368dfd00f165320084fa74a9a8c2381e05d91f1527dcae7d097844a35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **786.1 KB (786071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff078e33805d986da2bdead56800dca7302eb183ccf46ad6949da81f2b78b7`

```dockerfile
```

-	Layers:
	-	`sha256:499fff7b33ce95b2bbab56c8ca3332333475e391b52152835411f30b6fecc4ed`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 756.5 KB (756460 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7c3f45b51df19196192d2404b6a1096698e512a2253f7d46d99f326e131b29b2`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 29.6 KB (29611 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0.6-dind-alpine3.18`

```console
$ docker pull docker@sha256:97d1bb55b9bcd6ff473b502b8a3430746cff23f9dd91df2cbcea1fadc007b8ec
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0.6-dind-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:e789c61591b754ac6a1ad9ff9d8ee48dc53647af18b138a221f9aa71905ed774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115697171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8200afa4a2a250a8e86fae94260261ea891330888e2a501c04616c3b412726ba`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-dind-alpine3.18` - unknown; unknown

```console
$ docker pull docker@sha256:34f3ebd0448c84c8873476834aa905c214fb383ec94980b20c927d5fc6297308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.8 KB (785793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20ede7442e7bcd3e1d14cd5c4c20c8929599ed6fe7d79a80f56ed331ddc71bd3`

```dockerfile
```

-	Layers:
	-	`sha256:ed34957f1ab6901ab74ce916aaadbf43aca380b9e93d89606eb131fb6a3621c4`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 756.2 KB (756247 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e6f47f2c71b4df8f4ef8e667c6a81f7c431ef28cd5cc418e3910febc844ee03b`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 29.5 KB (29546 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0.6-dind-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2bb31b09e8ef8786e8fdf117e18f9a97fe8369ad6099892dfd50a22109b058e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107083571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4196298824a7c47ea599a8cd85c8878389f40df6ab7194c1cb0e19877771dc93`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 30 May 2023 23:04:12 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 30 May 2023 23:04:12 GMT
CMD ["/bin/sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 30 May 2023 23:04:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-dind-alpine3.18` - unknown; unknown

```console
$ docker pull docker@sha256:b36f12368dfd00f165320084fa74a9a8c2381e05d91f1527dcae7d097844a35d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **786.1 KB (786071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff078e33805d986da2bdead56800dca7302eb183ccf46ad6949da81f2b78b7`

```dockerfile
```

-	Layers:
	-	`sha256:499fff7b33ce95b2bbab56c8ca3332333475e391b52152835411f30b6fecc4ed`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 756.5 KB (756460 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7c3f45b51df19196192d2404b6a1096698e512a2253f7d46d99f326e131b29b2`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 29.6 KB (29611 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0.6-dind-rootless`

```console
$ docker pull docker@sha256:0efb72251205581d4b207036415a510c3bc08526b8ab313426901b87a4ce60b9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0.6-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5685cdce034a91d3d13846ab049e7e8e7758f8ebb24d6d697733f1944d3e819a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137408056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b7444e9281f477cb0c5803a6f598d3cb71d82be8d05563f3cb228c148d77044`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4afedb221fdf37ae0f1e9c505511ef57e6c5e0d47fdd221870dd730e2e109aa0`  
		Last Modified: Fri, 01 Sep 2023 02:51:23 GMT  
		Size: 1.4 MB (1362170 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18089b3504d00bb82232946c72809e37a7ffd275ccdbb782ff01cfff2b726b2c`  
		Last Modified: Fri, 01 Sep 2023 02:51:23 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b511fcf6d96c10e4425b245b9f675077e1cc852af71bf9a2193a86adacb32281`  
		Last Modified: Fri, 01 Sep 2023 02:51:23 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e53cfd232b06ea5e2d6b9985459f0232248392f329800cf0709cb7daec3228e`  
		Last Modified: Fri, 01 Sep 2023 02:51:24 GMT  
		Size: 20.3 MB (20347085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011a17494bfe75af1afdda085b158cabc695256f95e1e1f72140ec0b62c3d136`  
		Last Modified: Fri, 01 Sep 2023 02:51:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:1845e393b72e87398df05762530a78bfab55609a641f3d1c4b7c818ac0fe4c8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.0 KB (861953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af612d3539418ab94d1d9bd702f1518af14b50731fd782d912bfd642bc8f549f`

```dockerfile
```

-	Layers:
	-	`sha256:a641bf550c419e106c9e59888b84016322fd59b3f3bcfd2698d11faa89cb3d02`  
		Last Modified: Fri, 01 Sep 2023 02:51:22 GMT  
		Size: 831.2 KB (831171 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1178b9b6750fe46ad33765db0a23a8cd503f821825fcb33a2c4928eab4a323c2`  
		Last Modified: Fri, 01 Sep 2023 02:51:22 GMT  
		Size: 30.8 KB (30782 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0.6-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4a9320d6595a3a08eb0f4fd5b76df08deb7a926bc292585da944319b055de843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130739347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4226b7ecd248fcaaec7d3da2d950134dd61168f9b86e81ace89077dbcd4d8d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5aa08e1d66cf2432aa61153ab1551e2b7f406fd1d3c6c05d2709730afda00f66`  
		Last Modified: Fri, 01 Sep 2023 02:52:39 GMT  
		Size: 1.4 MB (1413171 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabd9555022518db5cd6f9d6540f59399825142dddc3ea57fa3c3d9f060dfb98`  
		Last Modified: Fri, 01 Sep 2023 02:52:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8e6681c4f34283f2117fca926ffb857a61052040f56edeaef4c5004ce8e65f4`  
		Last Modified: Fri, 01 Sep 2023 02:52:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9674110f5c8d3611567531a96e45c6886846e55968142de390f79c78ee3b5e3a`  
		Last Modified: Fri, 01 Sep 2023 02:52:41 GMT  
		Size: 22.2 MB (22240981 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:147f87e3db6c8847ea6872129417eff4a723348a62e859eb403d7048a5a20cbb`  
		Last Modified: Fri, 01 Sep 2023 02:52:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:dadfcbcac2cfd433adc7b4142f881d8e12fef34e38715209087564bb244962d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.2 KB (862232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1b97e5b32958699e4888a985c6d305a5555fc451c26fe4212596b8441b64f5`

```dockerfile
```

-	Layers:
	-	`sha256:ffc1955cb4b44e1f9a25db9e7f684b5a6cb54c8d6e916ab85a68f3deb92acf53`  
		Last Modified: Fri, 01 Sep 2023 02:52:38 GMT  
		Size: 831.4 KB (831394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0df79fc0ed374ce587fe85f134939287cfe4a3e0fe4b54f01a1b9dd3fd8f3ca2`  
		Last Modified: Fri, 01 Sep 2023 02:52:38 GMT  
		Size: 30.8 KB (30838 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0.6-git`

```console
$ docker pull docker@sha256:83e8049e04c2718c1915865509a3c1577936167cbd1de85c36cab50f06d6158a
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23.0.6-git` - linux; amd64

```console
$ docker pull docker@sha256:a548f107683c1a230d9fa65eb4f946e832c1f01ffbc0bd87492e58b7ed13d3e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.6 MB (120632416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0db0a601716ff460bf55a690cda8026bafa81e5bdc2eb666a2281c7d86265ad2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dc637b43d9a1be530bbb0bf04f5aa2df0db03a9d8a859d2d73978ba76458922`  
		Last Modified: Fri, 01 Sep 2023 00:51:11 GMT  
		Size: 2.0 MB (2014300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da631a25380a3953c3ec26b068605c249a9c215185b8eba2ff2d46d41b10dda0`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 16.3 MB (16250855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a0b80e8b6f4e1be7904b02b165da4cecbb88d3c348f6b21b7e7cd1a53592b63`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc33a04a2972155da94cd07359a286009e0b946df933f8b8c65b130791a5ab8`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 17.8 MB (17826592 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c36dd47a681e936eca6a43360cbe56501d3f438562a064ecb699803375b7d6e9`  
		Last Modified: Fri, 01 Sep 2023 00:51:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4761ac4fc32b8d5624cca364ae27bce2efb1df033cdd391b36eaab03aae82cd0`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2469fd65498eb05d0318616cdadda08526c43e2e39f71c75a30c1e7218e378cf`  
		Last Modified: Fri, 01 Sep 2023 00:51:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad99793fbd9b04163cad774b87c413299117aec041e69c945a5fc40b5ce254ad`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 7.1 MB (7080264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad957e8578f59bfee255ac5f5fda8c22bf42d33f13986b884ccbe9021b3a6ba`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023311cdc3039f563a8bd5c76da58faef61e97a33601a5454d12076ea57506f2`  
		Last Modified: Fri, 01 Sep 2023 01:50:57 GMT  
		Size: 51.7 MB (51657451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26212cc9ab730f476b8497344849ecc2f7d9d8f65c1a4ffbb455fbf9ad92cc11`  
		Last Modified: Fri, 01 Sep 2023 01:50:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b1e8099f0170ae6d195eaccdbb7041e138fa32b195d7d76f769490774556e5a`  
		Last Modified: Fri, 01 Sep 2023 01:50:56 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0aeca6a8a19b71e703338c8fe23340a66ca5c380d35701ac59e94afef2b30f65`  
		Last Modified: Fri, 01 Sep 2023 02:51:20 GMT  
		Size: 4.9 MB (4935245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-git` - unknown; unknown

```console
$ docker pull docker@sha256:d37c5358697f46aa9539cd71cf6e0ca5d30f8925f4756623c27d4ce71a92e2d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **815.2 KB (815188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7196406e0901742bfea27bc23d981c673e59acdacf3088168942d639e14ed08`

```dockerfile
```

-	Layers:
	-	`sha256:9ab8565952088e198b34b7db5e3b19a16414ff446f6e68c5707c590bf1afb712`  
		Last Modified: Fri, 01 Sep 2023 02:51:19 GMT  
		Size: 802.6 KB (802551 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e72d2d339f795c73c6905ac75773b878a59b1398bd3a8349c5f43a575f24fca0`  
		Last Modified: Fri, 01 Sep 2023 02:51:19 GMT  
		Size: 12.6 KB (12637 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23.0.6-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d294ac166eb13b6eccc30132ffdabe6217f75d44c7cf630910f943254f8a7be2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112105151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2f83da8abf36ae7ad9972703e20f59c17bc3dccf0e90796a3e175c7b39d9d8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f98439dd41c1aa2b7fec01ebd8a6fe6f86d45d34d4b5b2ccc545e06906fba647`  
		Last Modified: Fri, 01 Sep 2023 01:26:14 GMT  
		Size: 16.3 MB (16283689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ea9f56271fd4efb66f5b4b2fcdbb6b1b8aa54e604a818c868c52839b263f26`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b11eb1e2a4a15b54fb772482757aa25902417b1c7bb3a6d4cd2d448bed67fc`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e04686a2b8186e69165cfba25ecf25de27cedf8b04aeb66d1c255a20b42fc1`  
		Last Modified: Fri, 01 Sep 2023 01:26:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f9f8592f5afd6b0428ea754544c0f25dbbe002bdd4d3b3a561359c3243a10f3`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 7.3 MB (7291227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b64f6d12d924d63a583ef57b026e0f9787e44e11db209018fb9717130976318d`  
		Last Modified: Fri, 01 Sep 2023 01:54:04 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b442b3805385e684775ba79c8c2bd1d970dc27dfc91bb93fcb1682be82ebd71d`  
		Last Modified: Fri, 01 Sep 2023 01:54:07 GMT  
		Size: 47.1 MB (47053354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e809baabb04af80b58d47b7a5305af13149063e6f17ec1582240ad21e0b06e4`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87225f99297ea1bba5f6b5f0690f23735b50437ab815abe02eb95619b385f18`  
		Last Modified: Fri, 01 Sep 2023 01:54:05 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37ff5d948beb8d82d08e6f72b6b24dbd122c4a5f6b426b7a52be8e3bac1b15ce`  
		Last Modified: Fri, 01 Sep 2023 02:53:00 GMT  
		Size: 5.0 MB (5021580 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23.0.6-git` - unknown; unknown

```console
$ docker pull docker@sha256:345d4dbf2e504296a7f2f81a06513631bc25392ca02d35d6491f9cea89b1d0d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **813.2 KB (813230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27cd139fc6cf251de09a4f380a65b5ac0fa50536751f234273a0cfd0ffeb8b5e`

```dockerfile
```

-	Layers:
	-	`sha256:50affc58d2213269fbf0394e5da375165614cd748e09ec3feef48d1d8945744b`  
		Last Modified: Fri, 01 Sep 2023 02:52:59 GMT  
		Size: 802.8 KB (802762 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2872c68e47b18dfe8b7e529166d68d4bfbf2a4cab2d7096b61d25a62ab10d57d`  
		Last Modified: Fri, 01 Sep 2023 02:52:59 GMT  
		Size: 10.5 KB (10468 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:23.0.6-windowsservercore`

```console
$ docker pull docker@sha256:16b462db085f654f4ce57d7f591511b51fb3487b1058dd3a3627a106c4a8bba4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `docker:23.0.6-windowsservercore` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:302c8cffca6b41d60001a2eeb79dfcd4e2c6b74b0c24542ebb056d134fe84856
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791531414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683a51df9326337cbc0c9952319ab1159ce9ed67588d7a7ab972566f6a2e512d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:33:24 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:33:25 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:33:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:19:00 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:19:26 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:19:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:19:27 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:19:28 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:19:54 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e5ba6630913747243f16c95b58df1d8c250c524ddb1d00459cc4bf045f5e8`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836e29352be49089f6845f1d186db438ccea79fd8fd40bbf8143e0cea1ad127b`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702b6bf769b3162353e4653d05135a310199dd75384e801d5a0cb95d586890b5`  
		Last Modified: Fri, 14 Jul 2023 00:40:08 GMT  
		Size: 17.3 MB (17326326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d0d2bd953a11e1c74f54978bc4093611fad5b861020a52a327da28a9f812dc`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c74d5986d7c82fe298f6d23c7c4544e2db166002f2e10f09be308a217261b5`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c23640ed904d02f39fef76ce3aa248259c086e63e507d36d74f4c0e723aa4a`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ecf6a7fd01be9cbd8ba541afab0f6306b745a7b37008c0bb0f94a68913bc92`  
		Last Modified: Wed, 19 Jul 2023 20:23:35 GMT  
		Size: 17.9 MB (17906240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1149f19c417c36254bc6373fd924306cb0c465b7de893f99d53bbe3199f0c30`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8277e4bd032f1a5dabb132a56166f0ef8f35b16afd528c5b5e562f2ea663cd`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0244d3417c443d7cf7fe8914a210d93912c0a9dd581d4d4360401c5f59d0a9cc`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbcfa9d38c0c9f88ccbf3a7a2fa17ce02db7a9d473759654ee87706d2eb62a0`  
		Last Modified: Wed, 19 Jul 2023 20:23:36 GMT  
		Size: 18.5 MB (18457963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:8357222c4f8e4d3732234517e75b5a6d1526bb4a82170773298cb21ffca4384e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993772576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152df6f6b9c8902e86ce2157e7d89769c70630aaa2b33c8cd0da55a4a5d5dbd0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:35:06 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:35:07 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:36:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:20:02 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:21:08 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:21:09 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:22:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe87c749ec26fddbab372ff211c7d036270aa32c5f863788554545b6dc0e65`  
		Last Modified: Fri, 14 Jul 2023 00:40:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c8a148bf7b449438042f9b5b344bc9b3784db6e578afac659f2305b045d8e`  
		Last Modified: Fri, 14 Jul 2023 00:40:23 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d683cfce8a83d53a6a06324c0925b0f0dfb4adbfc19d33a22b1a920fbb48b0`  
		Last Modified: Fri, 14 Jul 2023 00:40:26 GMT  
		Size: 17.5 MB (17492115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663a2d2385c12b481d9a3db965cc1ed948ab38099b811b538e66812c8505feee`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49641e7dc187958ecf1ee7e7db3b1e33e9d30865792ef4b3617c8517cb9205c1`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e903ad2079967f3995b8975f856ab254e20c71b6939750e7868a4895abaa48b`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3fbc75a4b445b862680804d0be73be40e7e3d222645eeab13072656c22ecab`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 17.9 MB (17900340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67553d91a2a75ff6c2e282f1a15d2ca7503ba7b09d274aa650ae462fb46febce`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9156e5832bc6c0ccff3abfa254f4d59660d9a66debdcb8da852b5c3f321f9e6e`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5deaf99b6677fbd2f70aea7d775c789f020ca96ac300c3c76b2037da170b69`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd399bde2e139306ec43944416825461f5d85624fcfece2717c14277eea7ef2`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 18.4 MB (18447902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-windowsservercore-1809`

```console
$ docker pull docker@sha256:b24ed464edcede82751e5e169ab51d6ffa769e2e478e93dc6f57cc82a24a9b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `docker:23.0.6-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:8357222c4f8e4d3732234517e75b5a6d1526bb4a82170773298cb21ffca4384e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993772576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152df6f6b9c8902e86ce2157e7d89769c70630aaa2b33c8cd0da55a4a5d5dbd0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:35:06 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:35:07 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:36:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:20:01 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:20:02 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:21:08 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:21:09 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:21:10 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:22:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbe87c749ec26fddbab372ff211c7d036270aa32c5f863788554545b6dc0e65`  
		Last Modified: Fri, 14 Jul 2023 00:40:24 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c8a148bf7b449438042f9b5b344bc9b3784db6e578afac659f2305b045d8e`  
		Last Modified: Fri, 14 Jul 2023 00:40:23 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d683cfce8a83d53a6a06324c0925b0f0dfb4adbfc19d33a22b1a920fbb48b0`  
		Last Modified: Fri, 14 Jul 2023 00:40:26 GMT  
		Size: 17.5 MB (17492115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663a2d2385c12b481d9a3db965cc1ed948ab38099b811b538e66812c8505feee`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49641e7dc187958ecf1ee7e7db3b1e33e9d30865792ef4b3617c8517cb9205c1`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e903ad2079967f3995b8975f856ab254e20c71b6939750e7868a4895abaa48b`  
		Last Modified: Wed, 19 Jul 2023 20:23:50 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3fbc75a4b445b862680804d0be73be40e7e3d222645eeab13072656c22ecab`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 17.9 MB (17900340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67553d91a2a75ff6c2e282f1a15d2ca7503ba7b09d274aa650ae462fb46febce`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9156e5832bc6c0ccff3abfa254f4d59660d9a66debdcb8da852b5c3f321f9e6e`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5deaf99b6677fbd2f70aea7d775c789f020ca96ac300c3c76b2037da170b69`  
		Last Modified: Wed, 19 Jul 2023 20:23:48 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd399bde2e139306ec43944416825461f5d85624fcfece2717c14277eea7ef2`  
		Last Modified: Wed, 19 Jul 2023 20:23:53 GMT  
		Size: 18.4 MB (18447902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:a04ad4a9927705cfb502baed04e6b7e183e700a9871ea1713168e224fec472cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `docker:23.0.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:302c8cffca6b41d60001a2eeb79dfcd4e2c6b74b0c24542ebb056d134fe84856
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791531414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683a51df9326337cbc0c9952319ab1159ce9ed67588d7a7ab972566f6a2e512d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 14 Jul 2023 00:33:24 GMT
ENV DOCKER_VERSION=23.0.6
# Fri, 14 Jul 2023 00:33:25 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Fri, 14 Jul 2023 00:33:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 20:18:59 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Wed, 19 Jul 2023 20:19:00 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Wed, 19 Jul 2023 20:19:26 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Wed, 19 Jul 2023 20:19:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 20:19:27 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Wed, 19 Jul 2023 20:19:28 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Wed, 19 Jul 2023 20:19:54 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e5ba6630913747243f16c95b58df1d8c250c524ddb1d00459cc4bf045f5e8`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836e29352be49089f6845f1d186db438ccea79fd8fd40bbf8143e0cea1ad127b`  
		Last Modified: Fri, 14 Jul 2023 00:40:05 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702b6bf769b3162353e4653d05135a310199dd75384e801d5a0cb95d586890b5`  
		Last Modified: Fri, 14 Jul 2023 00:40:08 GMT  
		Size: 17.3 MB (17326326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d0d2bd953a11e1c74f54978bc4093611fad5b861020a52a327da28a9f812dc`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c74d5986d7c82fe298f6d23c7c4544e2db166002f2e10f09be308a217261b5`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c23640ed904d02f39fef76ce3aa248259c086e63e507d36d74f4c0e723aa4a`  
		Last Modified: Wed, 19 Jul 2023 20:23:33 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ecf6a7fd01be9cbd8ba541afab0f6306b745a7b37008c0bb0f94a68913bc92`  
		Last Modified: Wed, 19 Jul 2023 20:23:35 GMT  
		Size: 17.9 MB (17906240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1149f19c417c36254bc6373fd924306cb0c465b7de893f99d53bbe3199f0c30`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8277e4bd032f1a5dabb132a56166f0ef8f35b16afd528c5b5e562f2ea663cd`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0244d3417c443d7cf7fe8914a210d93912c0a9dd581d4d4360401c5f59d0a9cc`  
		Last Modified: Wed, 19 Jul 2023 20:23:31 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbcfa9d38c0c9f88ccbf3a7a2fa17ce02db7a9d473759654ee87706d2eb62a0`  
		Last Modified: Wed, 19 Jul 2023 20:23:36 GMT  
		Size: 18.5 MB (18457963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24`

```console
$ docker pull docker@sha256:3c6e4dca7a63c9a32a4e00da40461ce067f255987ccc9721cf18ffa087bcd1ef
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24` - linux; amd64

```console
$ docker pull docker@sha256:78e33a72a1df68d3b4341630a215626e79e45725e205f0355dc05df1b81ad68a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118557115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7015f2c475d511a251955877c2862016a4042512ba625ed905e69202f87e1a21`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24` - unknown; unknown

```console
$ docker pull docker@sha256:20f0d7c1e0ae8d99ea5f3501bfdda377cbef396dbd2cd8cd3c7fcd7597ee53b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.0 KB (786975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888e0f2341b28c595a15c556b7de2ef7b2193098083e90eb91c6b2ece4e62bec`

```dockerfile
```

-	Layers:
	-	`sha256:03a9e1145cddad6d8a9abd6d2286a33aeb8a425a56d89b267f34fa0ab3583d19`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 756.8 KB (756837 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eab5af778a6b0c2b95e4a1d9822191969109fc98ecde4850f146a3316b98a606`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 30.1 KB (30138 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:901dc6a38f98d1d06349951cdb3ca2e9ccd584800cd993df01c05cedf2843b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109859474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b564bb4cc4b98471f04d1e557a0ab96507f66c49cde4467b977093ec650c5f1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24` - unknown; unknown

```console
$ docker pull docker@sha256:77cc4a62cc1fb365e00a9a862478351523483c725343bef1b5b22f1771c43c5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.3 KB (787263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd8daf7609eefe181ab4e37963a8fa890fb51c1b9cc55d830dc3b342df02116e`

```dockerfile
```

-	Layers:
	-	`sha256:bb166e5b7fefafbf2b267ea78ffbc0f9f613d29a85403496612c8793e9042840`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 757.1 KB (757056 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c60cc6727f24722478cbb7a66e7581f4809f0f34e65a4820502072281db4b9df`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 30.2 KB (30207 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24-cli`

```console
$ docker pull docker@sha256:9b367a609980ee1cea24eced8c0b74f568c82b132e3d33eaa0f6541d9953bf5e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-cli` - linux; amd64

```console
$ docker pull docker@sha256:f9248b5872788eb49e736e528ebcf31968ccec5e6b8e6b846e809398a70ff519
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57093908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7844b29e3e744b792cd5c4bdda96161321cc768956e12dc028b589cadff514f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfafd3a03f86f8f8813d8593cbcdbb0f2bd563485a255b17fba55572660fc1c8`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 2.0 MB (2014278 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f11d96ce7eaab5d8477cac5287a279a9adf2f4c6d778b63270e1b221ab4584d0`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 16.4 MB (16390442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6adc040a05ccb3acafec7f4a65c399d368ffc9e014b4d984a42f2432a8f58f45`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 17.5 MB (17459264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:787484ec7e57111029c1f29235e0a0b33350e0befb17a7a15cbd76f5f5dd23d2`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 17.8 MB (17826602 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab22443da284594177ff13db91a7431d3471578ba1b745c66d6e895454f3429c`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4df676a3ac49055d4890d082ac1cdb61ec9a439259ea4fe5a839577c85067b72`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:579a751e9a42cd0a3ebd9915f4b50a56c8708c8bd093068e7d6f83634cb4fe53`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:df87b5147e586ef8ff0c49661841df6195ef78838784c99480b004114fd97662
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.0 KB (544983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d60bf9b69d0463620e58ccb7aa1113c63dcd41f64a932f47a0136160cf48be`

```dockerfile
```

-	Layers:
	-	`sha256:b790b0d0b8fe886c8f509fda7018f6e0facc92710788f97fd2fbfba705ab442c`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 509.2 KB (509190 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c22f71319459495f30ee1aaf1c322b60bad57466e66d498b2631f7f9fa5d4c34`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 35.8 KB (35793 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5e359ed63a7701d9562c556b0f222dc8e3ad19bcee0566a30833f5de1d30750c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52847495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065d24f0bfb34c1647d63547971b8c05d6b5edcb05e971ff58391625e032cd1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:767c2a40dc41374be62f00886c074a5c66733ebfa45696a9b8765a285eed5c72`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.4 MB (15438722 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011855a528fc2a658b48d2b14e37cf356d07a9b1c2cd8641c6a5e7cfa3ccafaf`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.8 MB (15768059 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2eb2999eb53e5e7a79b2d27342e4d916d743647901d49b0e96f2fa58d5e6070a`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 16.3 MB (16283682 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52a6c18002043ece3e43cadab3fa052630597b7bb8976ad905b872d056af785f`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a01340eade1af75fe9e912e065ccb2d2075e8c1b101cbbac08859ca74998d154`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcee97a2aa0f0c046fe3ed0b1e4942ac4fa93452309bd96070b95e8ae6a56168`  
		Last Modified: Wed, 06 Sep 2023 01:23:42 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:707f2d1c97a881e3bd8058d3ccb992bdfc2bc27dbec9196934975e1aa8f2c107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.9 KB (544862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be9e052d5b72f24afea01106b8a559cbe5075943addc694ed44d571f5e372ab`

```dockerfile
```

-	Layers:
	-	`sha256:e3c93f3b12dca7a0a023b607a1bd29a2b5de1caea0ce43e2f9dd243d95f17c8d`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 509.2 KB (509224 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:327f4bb108e7d6f2ecbb6f2c3882f50292572fff6e829191a422654e7a740db1`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 35.6 KB (35638 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24-dind`

```console
$ docker pull docker@sha256:3c6e4dca7a63c9a32a4e00da40461ce067f255987ccc9721cf18ffa087bcd1ef
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-dind` - linux; amd64

```console
$ docker pull docker@sha256:78e33a72a1df68d3b4341630a215626e79e45725e205f0355dc05df1b81ad68a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118557115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7015f2c475d511a251955877c2862016a4042512ba625ed905e69202f87e1a21`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind` - unknown; unknown

```console
$ docker pull docker@sha256:20f0d7c1e0ae8d99ea5f3501bfdda377cbef396dbd2cd8cd3c7fcd7597ee53b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.0 KB (786975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888e0f2341b28c595a15c556b7de2ef7b2193098083e90eb91c6b2ece4e62bec`

```dockerfile
```

-	Layers:
	-	`sha256:03a9e1145cddad6d8a9abd6d2286a33aeb8a425a56d89b267f34fa0ab3583d19`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 756.8 KB (756837 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eab5af778a6b0c2b95e4a1d9822191969109fc98ecde4850f146a3316b98a606`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 30.1 KB (30138 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:901dc6a38f98d1d06349951cdb3ca2e9ccd584800cd993df01c05cedf2843b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109859474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b564bb4cc4b98471f04d1e557a0ab96507f66c49cde4467b977093ec650c5f1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind` - unknown; unknown

```console
$ docker pull docker@sha256:77cc4a62cc1fb365e00a9a862478351523483c725343bef1b5b22f1771c43c5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.3 KB (787263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd8daf7609eefe181ab4e37963a8fa890fb51c1b9cc55d830dc3b342df02116e`

```dockerfile
```

-	Layers:
	-	`sha256:bb166e5b7fefafbf2b267ea78ffbc0f9f613d29a85403496612c8793e9042840`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 757.1 KB (757056 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c60cc6727f24722478cbb7a66e7581f4809f0f34e65a4820502072281db4b9df`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 30.2 KB (30207 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24-dind-rootless`

```console
$ docker pull docker@sha256:1efae30b885343f906a11d382509e5177e7acfea1d63d786941beb83685656a6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c80204c95aef7d81b017a5be00b61a841eb55758b4e72413ee2e9e8b554b66c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140579964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fed477a4899a587575cfce5cbe1811f6de019caec34609033a2f3d941bed817`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59443f8fa96049a4cf8d67317e5f823d846af2f9af78a86594e6586e939ee05d`  
		Last Modified: Fri, 01 Sep 2023 02:51:26 GMT  
		Size: 1.4 MB (1362146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98316da633db7edabfb8501df1c0f234f4d1e7c858aebcaca1df19e76e81817b`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1a039201548858b79cf3cc0bc49dc786d9188355988b02c4470004b370cfe70`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c280db80bab216e68945db9df61354adbfdddbf9f78c1a9fbbaa87dec04cb28e`  
		Last Modified: Fri, 01 Sep 2023 02:51:26 GMT  
		Size: 20.7 MB (20659076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2604315ba333e12dc0c16f81f4b608f109b8741b369ef25dbb65064deb2270d5`  
		Last Modified: Fri, 01 Sep 2023 02:51:26 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:bdea2a36f08e4211670cb172e088b3161818a1218010d451073be58d4cc4504e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.6 KB (862575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c6f610a81a6bacc84e64edbced072acff4b58ea4554ee24b0983afb732297c`

```dockerfile
```

-	Layers:
	-	`sha256:99d26d8e565fe2f748370f1c1497d0f7405e6a6a110e026b4f7f1ee561e3a08a`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 831.5 KB (831481 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:be40bc8c58b56816d6e977289238cf2424927d70fdeea9ed2d194c7b15a12234`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 31.1 KB (31094 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9c259ddd5697c1e260b1a381a100efa8bbb8864a0309a0d9420c3615a50b9d69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133723324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2638ec79b2a983a1bbd8c322a4462430d88303cdac2772d3bcfd670cb02cc156`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53878b06e1035044e67284bff906d3fc0df204161f5b009e9469da72477fa877`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 1.4 MB (1413168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e2ed305ea804e13233d7ec358d01eaf806b8d509f69d3278110f58ee9a8fcb0`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a6909dcb096132bdecc208fc905fcde36ac61c392a8e6c160889db94c44bbd7e`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0601c227926d4724b23791c8938b61d3968de7bb59646eeb00baee453e2ee4b`  
		Last Modified: Fri, 01 Sep 2023 02:51:54 GMT  
		Size: 22.4 MB (22449056 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6891c0c2c0ddd6a941fa5ca3131f2e83affd2cd56a3bcd57d8a6523d49ed56ca`  
		Last Modified: Fri, 01 Sep 2023 02:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:d7a1856277fbca39f82595a356a1db09e440393c79143820abfda61909f21af6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.9 KB (862864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542808f7074eafea27da73818e7c3a841ae6aa971753cd7344be0cacc363717a`

```dockerfile
```

-	Layers:
	-	`sha256:b04be43b56807d8c53ae591cb7ea77e35f514039e7e2514ebd1ac6b789dbc111`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 831.7 KB (831712 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b9ffa9d0bdbba40c3831fffbe2b6a85e02ca3991b0da5a36a7e9c75ee60bed66`  
		Last Modified: Fri, 01 Sep 2023 02:51:52 GMT  
		Size: 31.2 KB (31152 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24-git`

```console
$ docker pull docker@sha256:6d688492ebeb7902f180d9cfb589b5f9113fc758edabcb3b82df8f86c34b3f90
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-git` - linux; amd64

```console
$ docker pull docker@sha256:5b8c2653daf3eb59abbecf241dcbe12fa9e61813277bc3fd5248aea8c2d7a9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123492341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5317c041666eaf7f7c1893d9777527bbeb0decfd24ab715284ca14aa882241`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.5
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3011158b365f995fe31d93d2e89c0d74cddec794939e497e31c151f253bffae0`  
		Last Modified: Fri, 01 Sep 2023 02:51:15 GMT  
		Size: 4.9 MB (4935226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-git` - unknown; unknown

```console
$ docker pull docker@sha256:56759434ecca7c8b986be2f82694e0186fa7e71fb8082b98c7a31054c74a95f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **815.8 KB (815770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a38823fb0c813029d4604ae2b59a383f5d8792046d5cad3f4fe401f6ca41512`

```dockerfile
```

-	Layers:
	-	`sha256:16a3147ffec7dad2355c48f5a4b8a42e5565b75bbc599f9f595697873fb9a488`  
		Last Modified: Fri, 01 Sep 2023 02:51:15 GMT  
		Size: 802.8 KB (802841 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:46b98e19a72926c6941bb0d61072231db056038b7aa44f89150caf4a5a00756c`  
		Last Modified: Fri, 01 Sep 2023 02:51:14 GMT  
		Size: 12.9 KB (12929 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:24d3a88cd48430f0d644698d1af801887ffddb0d8352cc74052b8d3860af07a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114881054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:202873fceeb44d792f95943d18a54e6bce99ed53fe90c3fd9de41afc43c718e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.5
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb2f25f8887e66ab99e5140de9e72c589ddf0d593cf2302e5542c41e6d9d23a7`  
		Last Modified: Fri, 01 Sep 2023 02:52:13 GMT  
		Size: 5.0 MB (5021580 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-git` - unknown; unknown

```console
$ docker pull docker@sha256:6c1a5b8a7f8c123e101d4a1486f20638eda931d4b9818d02dd2a57c629002205
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **813.8 KB (813820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9acb3f9b51cd6e0970a451952654ed286a169c5c191e60b39359ed64f58cbc04`

```dockerfile
```

-	Layers:
	-	`sha256:b86dfe324eab5a824ef87f50112eee9995f094746b70235f913c054ede3178e6`  
		Last Modified: Fri, 01 Sep 2023 02:52:12 GMT  
		Size: 803.1 KB (803056 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:625a52e6134a0e12843f919ad63bff5d924c7bdf915b14a862e500a75618580c`  
		Last Modified: Fri, 01 Sep 2023 02:52:12 GMT  
		Size: 10.8 KB (10764 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24-windowsservercore`

```console
$ docker pull docker@sha256:dde81d7f2600ac22de6bfa8c7a07c4881524d1f45b803aebd69de7bdfcf5c1ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `docker:24-windowsservercore` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:f036505370e71fe6013e09eae58982bf19d779f261af758f03c3e0ca6e959fb6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791668357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e53ea0a0809793c899cf1e9cb3de891686b773872e92353ab6872f21093da2aa`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:15:13 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:15:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:15:45 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:15:46 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:15:47 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:16:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:16:18 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:16:19 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:16:20 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:16:48 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901deda7922d35795e3d4991c73cb1cab61c3b129a15bb04b3e7d123d0de0b60`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027eea06d0080daedf5ef523c93e969ec807b2a65dcd1021840f7e70db9f2a2`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486b855c5d89d784c7e85907326d05d26635441a754e9e426498138dc6fdd419`  
		Last Modified: Mon, 24 Jul 2023 22:21:36 GMT  
		Size: 17.5 MB (17465980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc0f5529504e867302acf706f596cbbe06f751ce571b8bbfd746e8b44b35db`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56660e6caa6afda40f70e06ad0adb7679ddd6362b112bf884959a9daa03f43ff`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da8ddac8b835e0b3f3ca4464213330eb286a31ea01b6d75b4f6353e2511083`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4f9f340fe4664aa4293c04caf8451644aa2f34e790ed08c60628376b6dc39`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 17.9 MB (17902937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8577eb74030f9da73f6f4a8dfc61abfe3a516bc71c0cdaf04aa41aaa5dfea7f`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2ae56b025d396a3597cfb2e9efa8779218d8b955a42b2d8dac86568f88eac8`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4b75aa8a819fda1544fe1e0e3befc8d1863729ec8df3d31f37b4e8c7608d9e`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966a418a3938e0554b46c43cacefdbe319c43861b807d6ac33e85e49c1c98d38`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 18.5 MB (18458205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:4ced44b2a9980116f078f1d4848c10ee0283902b9a1d508e6cf4aafbce3d3868
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993906076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755cf7950481c506283cd30fb68ffb4affa45ca5275b3aa5f346caa36f1dd253`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:16:56 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:16:57 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:18:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:18:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:18:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:18:10 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:19:23 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:19:25 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:20:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2828f54bc3b0d02a4c8b471fc44b6318a0be2b9409bb1c6555ae5430316de`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afa9d718105d43e5cf00564b995fe8b1f6259a84386406d7d566c2a467be18`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfca0ac7b7aebd4db3ee5b56977ee4242ec31f4262b541a5cb9e91041294a3f`  
		Last Modified: Mon, 24 Jul 2023 22:21:57 GMT  
		Size: 17.6 MB (17638105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e03760602364c4d21bbcda283366105ce48a61694ee415d935a4ce22aef03d`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcacb30c234bcade9db59bff00606d6e4432c65428ddb7a5919d82172700b4e`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a0b8e41707d2d1eb6d6ff3431d0d0b4f87e909f3722abeb94c44a3e9740261`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6415f8b4089b9fa213c16a68b1060faa1bd792ab011b27f358a326a7eafadd3a`  
		Last Modified: Mon, 24 Jul 2023 22:21:55 GMT  
		Size: 17.9 MB (17890313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67080a6fba2e9f7f1ab50eff043a6e8c7dea8ca31779d1dd087bd269f6be6d97`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a4edc0e994d2c782f76fa0ec93913467d6e3388943dd7884c38c1d444b0fad`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d533ad3c0b792a6a69b0573489d6628605c7fd8514021d65a9063886ed3e36`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e50d630030b8b04b07b76780e17708870d4943248c548a60a040099e237f0`  
		Last Modified: Mon, 24 Jul 2023 22:21:56 GMT  
		Size: 18.4 MB (18445548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-windowsservercore-1809`

```console
$ docker pull docker@sha256:a785eccd876138d5172dd1cf10d7e79ab801281784dbe5d8912b95fe8f2e8266
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `docker:24-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:4ced44b2a9980116f078f1d4848c10ee0283902b9a1d508e6cf4aafbce3d3868
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993906076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755cf7950481c506283cd30fb68ffb4affa45ca5275b3aa5f346caa36f1dd253`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:16:56 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:16:57 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:18:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:18:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:18:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:18:10 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:19:23 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:19:25 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:20:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2828f54bc3b0d02a4c8b471fc44b6318a0be2b9409bb1c6555ae5430316de`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afa9d718105d43e5cf00564b995fe8b1f6259a84386406d7d566c2a467be18`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfca0ac7b7aebd4db3ee5b56977ee4242ec31f4262b541a5cb9e91041294a3f`  
		Last Modified: Mon, 24 Jul 2023 22:21:57 GMT  
		Size: 17.6 MB (17638105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e03760602364c4d21bbcda283366105ce48a61694ee415d935a4ce22aef03d`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcacb30c234bcade9db59bff00606d6e4432c65428ddb7a5919d82172700b4e`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a0b8e41707d2d1eb6d6ff3431d0d0b4f87e909f3722abeb94c44a3e9740261`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6415f8b4089b9fa213c16a68b1060faa1bd792ab011b27f358a326a7eafadd3a`  
		Last Modified: Mon, 24 Jul 2023 22:21:55 GMT  
		Size: 17.9 MB (17890313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67080a6fba2e9f7f1ab50eff043a6e8c7dea8ca31779d1dd087bd269f6be6d97`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a4edc0e994d2c782f76fa0ec93913467d6e3388943dd7884c38c1d444b0fad`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d533ad3c0b792a6a69b0573489d6628605c7fd8514021d65a9063886ed3e36`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e50d630030b8b04b07b76780e17708870d4943248c548a60a040099e237f0`  
		Last Modified: Mon, 24 Jul 2023 22:21:56 GMT  
		Size: 18.4 MB (18445548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:6446b2f91d9e216ea9430abc2619ab0abfb508c8a2fd55be5d52441b0a04eabc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `docker:24-windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:f036505370e71fe6013e09eae58982bf19d779f261af758f03c3e0ca6e959fb6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791668357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e53ea0a0809793c899cf1e9cb3de891686b773872e92353ab6872f21093da2aa`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:15:13 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:15:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:15:45 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:15:46 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:15:47 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:16:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:16:18 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:16:19 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:16:20 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:16:48 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901deda7922d35795e3d4991c73cb1cab61c3b129a15bb04b3e7d123d0de0b60`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027eea06d0080daedf5ef523c93e969ec807b2a65dcd1021840f7e70db9f2a2`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486b855c5d89d784c7e85907326d05d26635441a754e9e426498138dc6fdd419`  
		Last Modified: Mon, 24 Jul 2023 22:21:36 GMT  
		Size: 17.5 MB (17465980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc0f5529504e867302acf706f596cbbe06f751ce571b8bbfd746e8b44b35db`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56660e6caa6afda40f70e06ad0adb7679ddd6362b112bf884959a9daa03f43ff`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da8ddac8b835e0b3f3ca4464213330eb286a31ea01b6d75b4f6353e2511083`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4f9f340fe4664aa4293c04caf8451644aa2f34e790ed08c60628376b6dc39`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 17.9 MB (17902937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8577eb74030f9da73f6f4a8dfc61abfe3a516bc71c0cdaf04aa41aaa5dfea7f`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2ae56b025d396a3597cfb2e9efa8779218d8b955a42b2d8dac86568f88eac8`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4b75aa8a819fda1544fe1e0e3befc8d1863729ec8df3d31f37b4e8c7608d9e`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966a418a3938e0554b46c43cacefdbe319c43861b807d6ac33e85e49c1c98d38`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 18.5 MB (18458205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0`

```console
$ docker pull docker@sha256:3c6e4dca7a63c9a32a4e00da40461ce067f255987ccc9721cf18ffa087bcd1ef
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0` - linux; amd64

```console
$ docker pull docker@sha256:78e33a72a1df68d3b4341630a215626e79e45725e205f0355dc05df1b81ad68a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118557115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7015f2c475d511a251955877c2862016a4042512ba625ed905e69202f87e1a21`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0` - unknown; unknown

```console
$ docker pull docker@sha256:20f0d7c1e0ae8d99ea5f3501bfdda377cbef396dbd2cd8cd3c7fcd7597ee53b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.0 KB (786975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888e0f2341b28c595a15c556b7de2ef7b2193098083e90eb91c6b2ece4e62bec`

```dockerfile
```

-	Layers:
	-	`sha256:03a9e1145cddad6d8a9abd6d2286a33aeb8a425a56d89b267f34fa0ab3583d19`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 756.8 KB (756837 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eab5af778a6b0c2b95e4a1d9822191969109fc98ecde4850f146a3316b98a606`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 30.1 KB (30138 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:901dc6a38f98d1d06349951cdb3ca2e9ccd584800cd993df01c05cedf2843b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109859474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b564bb4cc4b98471f04d1e557a0ab96507f66c49cde4467b977093ec650c5f1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0` - unknown; unknown

```console
$ docker pull docker@sha256:77cc4a62cc1fb365e00a9a862478351523483c725343bef1b5b22f1771c43c5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.3 KB (787263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd8daf7609eefe181ab4e37963a8fa890fb51c1b9cc55d830dc3b342df02116e`

```dockerfile
```

-	Layers:
	-	`sha256:bb166e5b7fefafbf2b267ea78ffbc0f9f613d29a85403496612c8793e9042840`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 757.1 KB (757056 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c60cc6727f24722478cbb7a66e7581f4809f0f34e65a4820502072281db4b9df`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 30.2 KB (30207 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0-cli`

```console
$ docker pull docker@sha256:9b367a609980ee1cea24eced8c0b74f568c82b132e3d33eaa0f6541d9953bf5e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0-cli` - linux; amd64

```console
$ docker pull docker@sha256:f9248b5872788eb49e736e528ebcf31968ccec5e6b8e6b846e809398a70ff519
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57093908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7844b29e3e744b792cd5c4bdda96161321cc768956e12dc028b589cadff514f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfafd3a03f86f8f8813d8593cbcdbb0f2bd563485a255b17fba55572660fc1c8`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 2.0 MB (2014278 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f11d96ce7eaab5d8477cac5287a279a9adf2f4c6d778b63270e1b221ab4584d0`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 16.4 MB (16390442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6adc040a05ccb3acafec7f4a65c399d368ffc9e014b4d984a42f2432a8f58f45`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 17.5 MB (17459264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:787484ec7e57111029c1f29235e0a0b33350e0befb17a7a15cbd76f5f5dd23d2`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 17.8 MB (17826602 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab22443da284594177ff13db91a7431d3471578ba1b745c66d6e895454f3429c`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4df676a3ac49055d4890d082ac1cdb61ec9a439259ea4fe5a839577c85067b72`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:579a751e9a42cd0a3ebd9915f4b50a56c8708c8bd093068e7d6f83634cb4fe53`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-cli` - unknown; unknown

```console
$ docker pull docker@sha256:df87b5147e586ef8ff0c49661841df6195ef78838784c99480b004114fd97662
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.0 KB (544983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d60bf9b69d0463620e58ccb7aa1113c63dcd41f64a932f47a0136160cf48be`

```dockerfile
```

-	Layers:
	-	`sha256:b790b0d0b8fe886c8f509fda7018f6e0facc92710788f97fd2fbfba705ab442c`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 509.2 KB (509190 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c22f71319459495f30ee1aaf1c322b60bad57466e66d498b2631f7f9fa5d4c34`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 35.8 KB (35793 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5e359ed63a7701d9562c556b0f222dc8e3ad19bcee0566a30833f5de1d30750c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52847495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065d24f0bfb34c1647d63547971b8c05d6b5edcb05e971ff58391625e032cd1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:767c2a40dc41374be62f00886c074a5c66733ebfa45696a9b8765a285eed5c72`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.4 MB (15438722 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011855a528fc2a658b48d2b14e37cf356d07a9b1c2cd8641c6a5e7cfa3ccafaf`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.8 MB (15768059 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2eb2999eb53e5e7a79b2d27342e4d916d743647901d49b0e96f2fa58d5e6070a`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 16.3 MB (16283682 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52a6c18002043ece3e43cadab3fa052630597b7bb8976ad905b872d056af785f`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a01340eade1af75fe9e912e065ccb2d2075e8c1b101cbbac08859ca74998d154`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcee97a2aa0f0c046fe3ed0b1e4942ac4fa93452309bd96070b95e8ae6a56168`  
		Last Modified: Wed, 06 Sep 2023 01:23:42 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-cli` - unknown; unknown

```console
$ docker pull docker@sha256:707f2d1c97a881e3bd8058d3ccb992bdfc2bc27dbec9196934975e1aa8f2c107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.9 KB (544862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be9e052d5b72f24afea01106b8a559cbe5075943addc694ed44d571f5e372ab`

```dockerfile
```

-	Layers:
	-	`sha256:e3c93f3b12dca7a0a023b607a1bd29a2b5de1caea0ce43e2f9dd243d95f17c8d`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 509.2 KB (509224 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:327f4bb108e7d6f2ecbb6f2c3882f50292572fff6e829191a422654e7a740db1`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 35.6 KB (35638 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0-dind`

```console
$ docker pull docker@sha256:3c6e4dca7a63c9a32a4e00da40461ce067f255987ccc9721cf18ffa087bcd1ef
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:78e33a72a1df68d3b4341630a215626e79e45725e205f0355dc05df1b81ad68a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118557115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7015f2c475d511a251955877c2862016a4042512ba625ed905e69202f87e1a21`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-dind` - unknown; unknown

```console
$ docker pull docker@sha256:20f0d7c1e0ae8d99ea5f3501bfdda377cbef396dbd2cd8cd3c7fcd7597ee53b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.0 KB (786975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888e0f2341b28c595a15c556b7de2ef7b2193098083e90eb91c6b2ece4e62bec`

```dockerfile
```

-	Layers:
	-	`sha256:03a9e1145cddad6d8a9abd6d2286a33aeb8a425a56d89b267f34fa0ab3583d19`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 756.8 KB (756837 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eab5af778a6b0c2b95e4a1d9822191969109fc98ecde4850f146a3316b98a606`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 30.1 KB (30138 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:901dc6a38f98d1d06349951cdb3ca2e9ccd584800cd993df01c05cedf2843b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109859474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b564bb4cc4b98471f04d1e557a0ab96507f66c49cde4467b977093ec650c5f1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-dind` - unknown; unknown

```console
$ docker pull docker@sha256:77cc4a62cc1fb365e00a9a862478351523483c725343bef1b5b22f1771c43c5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.3 KB (787263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd8daf7609eefe181ab4e37963a8fa890fb51c1b9cc55d830dc3b342df02116e`

```dockerfile
```

-	Layers:
	-	`sha256:bb166e5b7fefafbf2b267ea78ffbc0f9f613d29a85403496612c8793e9042840`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 757.1 KB (757056 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c60cc6727f24722478cbb7a66e7581f4809f0f34e65a4820502072281db4b9df`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 30.2 KB (30207 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0-dind-rootless`

```console
$ docker pull docker@sha256:1efae30b885343f906a11d382509e5177e7acfea1d63d786941beb83685656a6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c80204c95aef7d81b017a5be00b61a841eb55758b4e72413ee2e9e8b554b66c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140579964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fed477a4899a587575cfce5cbe1811f6de019caec34609033a2f3d941bed817`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59443f8fa96049a4cf8d67317e5f823d846af2f9af78a86594e6586e939ee05d`  
		Last Modified: Fri, 01 Sep 2023 02:51:26 GMT  
		Size: 1.4 MB (1362146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98316da633db7edabfb8501df1c0f234f4d1e7c858aebcaca1df19e76e81817b`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1a039201548858b79cf3cc0bc49dc786d9188355988b02c4470004b370cfe70`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c280db80bab216e68945db9df61354adbfdddbf9f78c1a9fbbaa87dec04cb28e`  
		Last Modified: Fri, 01 Sep 2023 02:51:26 GMT  
		Size: 20.7 MB (20659076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2604315ba333e12dc0c16f81f4b608f109b8741b369ef25dbb65064deb2270d5`  
		Last Modified: Fri, 01 Sep 2023 02:51:26 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:bdea2a36f08e4211670cb172e088b3161818a1218010d451073be58d4cc4504e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.6 KB (862575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c6f610a81a6bacc84e64edbced072acff4b58ea4554ee24b0983afb732297c`

```dockerfile
```

-	Layers:
	-	`sha256:99d26d8e565fe2f748370f1c1497d0f7405e6a6a110e026b4f7f1ee561e3a08a`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 831.5 KB (831481 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:be40bc8c58b56816d6e977289238cf2424927d70fdeea9ed2d194c7b15a12234`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 31.1 KB (31094 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9c259ddd5697c1e260b1a381a100efa8bbb8864a0309a0d9420c3615a50b9d69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133723324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2638ec79b2a983a1bbd8c322a4462430d88303cdac2772d3bcfd670cb02cc156`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53878b06e1035044e67284bff906d3fc0df204161f5b009e9469da72477fa877`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 1.4 MB (1413168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e2ed305ea804e13233d7ec358d01eaf806b8d509f69d3278110f58ee9a8fcb0`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a6909dcb096132bdecc208fc905fcde36ac61c392a8e6c160889db94c44bbd7e`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0601c227926d4724b23791c8938b61d3968de7bb59646eeb00baee453e2ee4b`  
		Last Modified: Fri, 01 Sep 2023 02:51:54 GMT  
		Size: 22.4 MB (22449056 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6891c0c2c0ddd6a941fa5ca3131f2e83affd2cd56a3bcd57d8a6523d49ed56ca`  
		Last Modified: Fri, 01 Sep 2023 02:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:d7a1856277fbca39f82595a356a1db09e440393c79143820abfda61909f21af6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.9 KB (862864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542808f7074eafea27da73818e7c3a841ae6aa971753cd7344be0cacc363717a`

```dockerfile
```

-	Layers:
	-	`sha256:b04be43b56807d8c53ae591cb7ea77e35f514039e7e2514ebd1ac6b789dbc111`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 831.7 KB (831712 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b9ffa9d0bdbba40c3831fffbe2b6a85e02ca3991b0da5a36a7e9c75ee60bed66`  
		Last Modified: Fri, 01 Sep 2023 02:51:52 GMT  
		Size: 31.2 KB (31152 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0-git`

```console
$ docker pull docker@sha256:6d688492ebeb7902f180d9cfb589b5f9113fc758edabcb3b82df8f86c34b3f90
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0-git` - linux; amd64

```console
$ docker pull docker@sha256:5b8c2653daf3eb59abbecf241dcbe12fa9e61813277bc3fd5248aea8c2d7a9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123492341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5317c041666eaf7f7c1893d9777527bbeb0decfd24ab715284ca14aa882241`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.5
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3011158b365f995fe31d93d2e89c0d74cddec794939e497e31c151f253bffae0`  
		Last Modified: Fri, 01 Sep 2023 02:51:15 GMT  
		Size: 4.9 MB (4935226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-git` - unknown; unknown

```console
$ docker pull docker@sha256:56759434ecca7c8b986be2f82694e0186fa7e71fb8082b98c7a31054c74a95f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **815.8 KB (815770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a38823fb0c813029d4604ae2b59a383f5d8792046d5cad3f4fe401f6ca41512`

```dockerfile
```

-	Layers:
	-	`sha256:16a3147ffec7dad2355c48f5a4b8a42e5565b75bbc599f9f595697873fb9a488`  
		Last Modified: Fri, 01 Sep 2023 02:51:15 GMT  
		Size: 802.8 KB (802841 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:46b98e19a72926c6941bb0d61072231db056038b7aa44f89150caf4a5a00756c`  
		Last Modified: Fri, 01 Sep 2023 02:51:14 GMT  
		Size: 12.9 KB (12929 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:24d3a88cd48430f0d644698d1af801887ffddb0d8352cc74052b8d3860af07a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114881054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:202873fceeb44d792f95943d18a54e6bce99ed53fe90c3fd9de41afc43c718e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.5
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb2f25f8887e66ab99e5140de9e72c589ddf0d593cf2302e5542c41e6d9d23a7`  
		Last Modified: Fri, 01 Sep 2023 02:52:13 GMT  
		Size: 5.0 MB (5021580 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-git` - unknown; unknown

```console
$ docker pull docker@sha256:6c1a5b8a7f8c123e101d4a1486f20638eda931d4b9818d02dd2a57c629002205
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **813.8 KB (813820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9acb3f9b51cd6e0970a451952654ed286a169c5c191e60b39359ed64f58cbc04`

```dockerfile
```

-	Layers:
	-	`sha256:b86dfe324eab5a824ef87f50112eee9995f094746b70235f913c054ede3178e6`  
		Last Modified: Fri, 01 Sep 2023 02:52:12 GMT  
		Size: 803.1 KB (803056 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:625a52e6134a0e12843f919ad63bff5d924c7bdf915b14a862e500a75618580c`  
		Last Modified: Fri, 01 Sep 2023 02:52:12 GMT  
		Size: 10.8 KB (10764 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0-windowsservercore`

```console
$ docker pull docker@sha256:dde81d7f2600ac22de6bfa8c7a07c4881524d1f45b803aebd69de7bdfcf5c1ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `docker:24.0-windowsservercore` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:f036505370e71fe6013e09eae58982bf19d779f261af758f03c3e0ca6e959fb6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791668357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e53ea0a0809793c899cf1e9cb3de891686b773872e92353ab6872f21093da2aa`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:15:13 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:15:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:15:45 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:15:46 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:15:47 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:16:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:16:18 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:16:19 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:16:20 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:16:48 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901deda7922d35795e3d4991c73cb1cab61c3b129a15bb04b3e7d123d0de0b60`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027eea06d0080daedf5ef523c93e969ec807b2a65dcd1021840f7e70db9f2a2`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486b855c5d89d784c7e85907326d05d26635441a754e9e426498138dc6fdd419`  
		Last Modified: Mon, 24 Jul 2023 22:21:36 GMT  
		Size: 17.5 MB (17465980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc0f5529504e867302acf706f596cbbe06f751ce571b8bbfd746e8b44b35db`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56660e6caa6afda40f70e06ad0adb7679ddd6362b112bf884959a9daa03f43ff`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da8ddac8b835e0b3f3ca4464213330eb286a31ea01b6d75b4f6353e2511083`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4f9f340fe4664aa4293c04caf8451644aa2f34e790ed08c60628376b6dc39`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 17.9 MB (17902937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8577eb74030f9da73f6f4a8dfc61abfe3a516bc71c0cdaf04aa41aaa5dfea7f`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2ae56b025d396a3597cfb2e9efa8779218d8b955a42b2d8dac86568f88eac8`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4b75aa8a819fda1544fe1e0e3befc8d1863729ec8df3d31f37b4e8c7608d9e`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966a418a3938e0554b46c43cacefdbe319c43861b807d6ac33e85e49c1c98d38`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 18.5 MB (18458205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:4ced44b2a9980116f078f1d4848c10ee0283902b9a1d508e6cf4aafbce3d3868
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993906076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755cf7950481c506283cd30fb68ffb4affa45ca5275b3aa5f346caa36f1dd253`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:16:56 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:16:57 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:18:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:18:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:18:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:18:10 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:19:23 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:19:25 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:20:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2828f54bc3b0d02a4c8b471fc44b6318a0be2b9409bb1c6555ae5430316de`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afa9d718105d43e5cf00564b995fe8b1f6259a84386406d7d566c2a467be18`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfca0ac7b7aebd4db3ee5b56977ee4242ec31f4262b541a5cb9e91041294a3f`  
		Last Modified: Mon, 24 Jul 2023 22:21:57 GMT  
		Size: 17.6 MB (17638105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e03760602364c4d21bbcda283366105ce48a61694ee415d935a4ce22aef03d`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcacb30c234bcade9db59bff00606d6e4432c65428ddb7a5919d82172700b4e`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a0b8e41707d2d1eb6d6ff3431d0d0b4f87e909f3722abeb94c44a3e9740261`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6415f8b4089b9fa213c16a68b1060faa1bd792ab011b27f358a326a7eafadd3a`  
		Last Modified: Mon, 24 Jul 2023 22:21:55 GMT  
		Size: 17.9 MB (17890313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67080a6fba2e9f7f1ab50eff043a6e8c7dea8ca31779d1dd087bd269f6be6d97`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a4edc0e994d2c782f76fa0ec93913467d6e3388943dd7884c38c1d444b0fad`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d533ad3c0b792a6a69b0573489d6628605c7fd8514021d65a9063886ed3e36`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e50d630030b8b04b07b76780e17708870d4943248c548a60a040099e237f0`  
		Last Modified: Mon, 24 Jul 2023 22:21:56 GMT  
		Size: 18.4 MB (18445548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-windowsservercore-1809`

```console
$ docker pull docker@sha256:a785eccd876138d5172dd1cf10d7e79ab801281784dbe5d8912b95fe8f2e8266
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `docker:24.0-windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:4ced44b2a9980116f078f1d4848c10ee0283902b9a1d508e6cf4aafbce3d3868
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993906076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755cf7950481c506283cd30fb68ffb4affa45ca5275b3aa5f346caa36f1dd253`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:16:56 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:16:57 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:18:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:18:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:18:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:18:10 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:19:23 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:19:25 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:20:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2828f54bc3b0d02a4c8b471fc44b6318a0be2b9409bb1c6555ae5430316de`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afa9d718105d43e5cf00564b995fe8b1f6259a84386406d7d566c2a467be18`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfca0ac7b7aebd4db3ee5b56977ee4242ec31f4262b541a5cb9e91041294a3f`  
		Last Modified: Mon, 24 Jul 2023 22:21:57 GMT  
		Size: 17.6 MB (17638105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e03760602364c4d21bbcda283366105ce48a61694ee415d935a4ce22aef03d`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcacb30c234bcade9db59bff00606d6e4432c65428ddb7a5919d82172700b4e`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a0b8e41707d2d1eb6d6ff3431d0d0b4f87e909f3722abeb94c44a3e9740261`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6415f8b4089b9fa213c16a68b1060faa1bd792ab011b27f358a326a7eafadd3a`  
		Last Modified: Mon, 24 Jul 2023 22:21:55 GMT  
		Size: 17.9 MB (17890313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67080a6fba2e9f7f1ab50eff043a6e8c7dea8ca31779d1dd087bd269f6be6d97`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a4edc0e994d2c782f76fa0ec93913467d6e3388943dd7884c38c1d444b0fad`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d533ad3c0b792a6a69b0573489d6628605c7fd8514021d65a9063886ed3e36`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e50d630030b8b04b07b76780e17708870d4943248c548a60a040099e237f0`  
		Last Modified: Mon, 24 Jul 2023 22:21:56 GMT  
		Size: 18.4 MB (18445548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:6446b2f91d9e216ea9430abc2619ab0abfb508c8a2fd55be5d52441b0a04eabc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `docker:24.0-windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:f036505370e71fe6013e09eae58982bf19d779f261af758f03c3e0ca6e959fb6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791668357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e53ea0a0809793c899cf1e9cb3de891686b773872e92353ab6872f21093da2aa`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:15:13 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:15:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:15:45 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:15:46 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:15:47 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:16:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:16:18 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:16:19 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:16:20 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:16:48 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901deda7922d35795e3d4991c73cb1cab61c3b129a15bb04b3e7d123d0de0b60`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027eea06d0080daedf5ef523c93e969ec807b2a65dcd1021840f7e70db9f2a2`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486b855c5d89d784c7e85907326d05d26635441a754e9e426498138dc6fdd419`  
		Last Modified: Mon, 24 Jul 2023 22:21:36 GMT  
		Size: 17.5 MB (17465980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc0f5529504e867302acf706f596cbbe06f751ce571b8bbfd746e8b44b35db`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56660e6caa6afda40f70e06ad0adb7679ddd6362b112bf884959a9daa03f43ff`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da8ddac8b835e0b3f3ca4464213330eb286a31ea01b6d75b4f6353e2511083`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4f9f340fe4664aa4293c04caf8451644aa2f34e790ed08c60628376b6dc39`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 17.9 MB (17902937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8577eb74030f9da73f6f4a8dfc61abfe3a516bc71c0cdaf04aa41aaa5dfea7f`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2ae56b025d396a3597cfb2e9efa8779218d8b955a42b2d8dac86568f88eac8`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4b75aa8a819fda1544fe1e0e3befc8d1863729ec8df3d31f37b4e8c7608d9e`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966a418a3938e0554b46c43cacefdbe319c43861b807d6ac33e85e49c1c98d38`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 18.5 MB (18458205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0.6`

```console
$ docker pull docker@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `docker:24.0.6-alpine3.18`

```console
$ docker pull docker@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `docker:24.0.6-cli`

```console
$ docker pull docker@sha256:9b367a609980ee1cea24eced8c0b74f568c82b132e3d33eaa0f6541d9953bf5e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0.6-cli` - linux; amd64

```console
$ docker pull docker@sha256:f9248b5872788eb49e736e528ebcf31968ccec5e6b8e6b846e809398a70ff519
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57093908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7844b29e3e744b792cd5c4bdda96161321cc768956e12dc028b589cadff514f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfafd3a03f86f8f8813d8593cbcdbb0f2bd563485a255b17fba55572660fc1c8`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 2.0 MB (2014278 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f11d96ce7eaab5d8477cac5287a279a9adf2f4c6d778b63270e1b221ab4584d0`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 16.4 MB (16390442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6adc040a05ccb3acafec7f4a65c399d368ffc9e014b4d984a42f2432a8f58f45`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 17.5 MB (17459264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:787484ec7e57111029c1f29235e0a0b33350e0befb17a7a15cbd76f5f5dd23d2`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 17.8 MB (17826602 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab22443da284594177ff13db91a7431d3471578ba1b745c66d6e895454f3429c`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4df676a3ac49055d4890d082ac1cdb61ec9a439259ea4fe5a839577c85067b72`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:579a751e9a42cd0a3ebd9915f4b50a56c8708c8bd093068e7d6f83634cb4fe53`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0.6-cli` - unknown; unknown

```console
$ docker pull docker@sha256:df87b5147e586ef8ff0c49661841df6195ef78838784c99480b004114fd97662
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.0 KB (544983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d60bf9b69d0463620e58ccb7aa1113c63dcd41f64a932f47a0136160cf48be`

```dockerfile
```

-	Layers:
	-	`sha256:b790b0d0b8fe886c8f509fda7018f6e0facc92710788f97fd2fbfba705ab442c`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 509.2 KB (509190 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c22f71319459495f30ee1aaf1c322b60bad57466e66d498b2631f7f9fa5d4c34`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 35.8 KB (35793 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0.6-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5e359ed63a7701d9562c556b0f222dc8e3ad19bcee0566a30833f5de1d30750c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52847495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065d24f0bfb34c1647d63547971b8c05d6b5edcb05e971ff58391625e032cd1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:767c2a40dc41374be62f00886c074a5c66733ebfa45696a9b8765a285eed5c72`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.4 MB (15438722 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011855a528fc2a658b48d2b14e37cf356d07a9b1c2cd8641c6a5e7cfa3ccafaf`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.8 MB (15768059 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2eb2999eb53e5e7a79b2d27342e4d916d743647901d49b0e96f2fa58d5e6070a`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 16.3 MB (16283682 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52a6c18002043ece3e43cadab3fa052630597b7bb8976ad905b872d056af785f`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a01340eade1af75fe9e912e065ccb2d2075e8c1b101cbbac08859ca74998d154`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcee97a2aa0f0c046fe3ed0b1e4942ac4fa93452309bd96070b95e8ae6a56168`  
		Last Modified: Wed, 06 Sep 2023 01:23:42 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0.6-cli` - unknown; unknown

```console
$ docker pull docker@sha256:707f2d1c97a881e3bd8058d3ccb992bdfc2bc27dbec9196934975e1aa8f2c107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.9 KB (544862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be9e052d5b72f24afea01106b8a559cbe5075943addc694ed44d571f5e372ab`

```dockerfile
```

-	Layers:
	-	`sha256:e3c93f3b12dca7a0a023b607a1bd29a2b5de1caea0ce43e2f9dd243d95f17c8d`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 509.2 KB (509224 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:327f4bb108e7d6f2ecbb6f2c3882f50292572fff6e829191a422654e7a740db1`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 35.6 KB (35638 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0.6-cli-alpine3.18`

```console
$ docker pull docker@sha256:9b367a609980ee1cea24eced8c0b74f568c82b132e3d33eaa0f6541d9953bf5e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0.6-cli-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:f9248b5872788eb49e736e528ebcf31968ccec5e6b8e6b846e809398a70ff519
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57093908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7844b29e3e744b792cd5c4bdda96161321cc768956e12dc028b589cadff514f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfafd3a03f86f8f8813d8593cbcdbb0f2bd563485a255b17fba55572660fc1c8`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 2.0 MB (2014278 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f11d96ce7eaab5d8477cac5287a279a9adf2f4c6d778b63270e1b221ab4584d0`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 16.4 MB (16390442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6adc040a05ccb3acafec7f4a65c399d368ffc9e014b4d984a42f2432a8f58f45`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 17.5 MB (17459264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:787484ec7e57111029c1f29235e0a0b33350e0befb17a7a15cbd76f5f5dd23d2`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 17.8 MB (17826602 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab22443da284594177ff13db91a7431d3471578ba1b745c66d6e895454f3429c`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4df676a3ac49055d4890d082ac1cdb61ec9a439259ea4fe5a839577c85067b72`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:579a751e9a42cd0a3ebd9915f4b50a56c8708c8bd093068e7d6f83634cb4fe53`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0.6-cli-alpine3.18` - unknown; unknown

```console
$ docker pull docker@sha256:df87b5147e586ef8ff0c49661841df6195ef78838784c99480b004114fd97662
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.0 KB (544983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d60bf9b69d0463620e58ccb7aa1113c63dcd41f64a932f47a0136160cf48be`

```dockerfile
```

-	Layers:
	-	`sha256:b790b0d0b8fe886c8f509fda7018f6e0facc92710788f97fd2fbfba705ab442c`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 509.2 KB (509190 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c22f71319459495f30ee1aaf1c322b60bad57466e66d498b2631f7f9fa5d4c34`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 35.8 KB (35793 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0.6-cli-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5e359ed63a7701d9562c556b0f222dc8e3ad19bcee0566a30833f5de1d30750c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52847495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065d24f0bfb34c1647d63547971b8c05d6b5edcb05e971ff58391625e032cd1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:767c2a40dc41374be62f00886c074a5c66733ebfa45696a9b8765a285eed5c72`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.4 MB (15438722 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011855a528fc2a658b48d2b14e37cf356d07a9b1c2cd8641c6a5e7cfa3ccafaf`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.8 MB (15768059 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2eb2999eb53e5e7a79b2d27342e4d916d743647901d49b0e96f2fa58d5e6070a`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 16.3 MB (16283682 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52a6c18002043ece3e43cadab3fa052630597b7bb8976ad905b872d056af785f`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a01340eade1af75fe9e912e065ccb2d2075e8c1b101cbbac08859ca74998d154`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcee97a2aa0f0c046fe3ed0b1e4942ac4fa93452309bd96070b95e8ae6a56168`  
		Last Modified: Wed, 06 Sep 2023 01:23:42 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0.6-cli-alpine3.18` - unknown; unknown

```console
$ docker pull docker@sha256:707f2d1c97a881e3bd8058d3ccb992bdfc2bc27dbec9196934975e1aa8f2c107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.9 KB (544862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be9e052d5b72f24afea01106b8a559cbe5075943addc694ed44d571f5e372ab`

```dockerfile
```

-	Layers:
	-	`sha256:e3c93f3b12dca7a0a023b607a1bd29a2b5de1caea0ce43e2f9dd243d95f17c8d`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 509.2 KB (509224 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:327f4bb108e7d6f2ecbb6f2c3882f50292572fff6e829191a422654e7a740db1`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 35.6 KB (35638 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0.6-dind`

```console
$ docker pull docker@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `docker:24.0.6-dind-alpine3.18`

```console
$ docker pull docker@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `docker:24.0.6-dind-rootless`

```console
$ docker pull docker@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `docker:24.0.6-git`

```console
$ docker pull docker@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `docker:24.0.6-windowsservercore`

```console
$ docker pull docker@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `docker:24.0.6-windowsservercore-1809`

```console
$ docker pull docker@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `docker:24.0.6-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `docker:cli`

```console
$ docker pull docker@sha256:9b367a609980ee1cea24eced8c0b74f568c82b132e3d33eaa0f6541d9953bf5e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:f9248b5872788eb49e736e528ebcf31968ccec5e6b8e6b846e809398a70ff519
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57093908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7844b29e3e744b792cd5c4bdda96161321cc768956e12dc028b589cadff514f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfafd3a03f86f8f8813d8593cbcdbb0f2bd563485a255b17fba55572660fc1c8`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 2.0 MB (2014278 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f11d96ce7eaab5d8477cac5287a279a9adf2f4c6d778b63270e1b221ab4584d0`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 16.4 MB (16390442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6adc040a05ccb3acafec7f4a65c399d368ffc9e014b4d984a42f2432a8f58f45`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 17.5 MB (17459264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:787484ec7e57111029c1f29235e0a0b33350e0befb17a7a15cbd76f5f5dd23d2`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 17.8 MB (17826602 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab22443da284594177ff13db91a7431d3471578ba1b745c66d6e895454f3429c`  
		Last Modified: Wed, 06 Sep 2023 01:13:26 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4df676a3ac49055d4890d082ac1cdb61ec9a439259ea4fe5a839577c85067b72`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:579a751e9a42cd0a3ebd9915f4b50a56c8708c8bd093068e7d6f83634cb4fe53`  
		Last Modified: Wed, 06 Sep 2023 01:13:27 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:df87b5147e586ef8ff0c49661841df6195ef78838784c99480b004114fd97662
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.0 KB (544983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d60bf9b69d0463620e58ccb7aa1113c63dcd41f64a932f47a0136160cf48be`

```dockerfile
```

-	Layers:
	-	`sha256:b790b0d0b8fe886c8f509fda7018f6e0facc92710788f97fd2fbfba705ab442c`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 509.2 KB (509190 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c22f71319459495f30ee1aaf1c322b60bad57466e66d498b2631f7f9fa5d4c34`  
		Last Modified: Wed, 06 Sep 2023 01:13:25 GMT  
		Size: 35.8 KB (35793 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5e359ed63a7701d9562c556b0f222dc8e3ad19bcee0566a30833f5de1d30750c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52847495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065d24f0bfb34c1647d63547971b8c05d6b5edcb05e971ff58391625e032cd1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:767c2a40dc41374be62f00886c074a5c66733ebfa45696a9b8765a285eed5c72`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.4 MB (15438722 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011855a528fc2a658b48d2b14e37cf356d07a9b1c2cd8641c6a5e7cfa3ccafaf`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.8 MB (15768059 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2eb2999eb53e5e7a79b2d27342e4d916d743647901d49b0e96f2fa58d5e6070a`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 16.3 MB (16283682 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52a6c18002043ece3e43cadab3fa052630597b7bb8976ad905b872d056af785f`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a01340eade1af75fe9e912e065ccb2d2075e8c1b101cbbac08859ca74998d154`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcee97a2aa0f0c046fe3ed0b1e4942ac4fa93452309bd96070b95e8ae6a56168`  
		Last Modified: Wed, 06 Sep 2023 01:23:42 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:707f2d1c97a881e3bd8058d3ccb992bdfc2bc27dbec9196934975e1aa8f2c107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.9 KB (544862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be9e052d5b72f24afea01106b8a559cbe5075943addc694ed44d571f5e372ab`

```dockerfile
```

-	Layers:
	-	`sha256:e3c93f3b12dca7a0a023b607a1bd29a2b5de1caea0ce43e2f9dd243d95f17c8d`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 509.2 KB (509224 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:327f4bb108e7d6f2ecbb6f2c3882f50292572fff6e829191a422654e7a740db1`  
		Last Modified: Wed, 06 Sep 2023 01:23:40 GMT  
		Size: 35.6 KB (35638 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:dind`

```console
$ docker pull docker@sha256:3c6e4dca7a63c9a32a4e00da40461ce067f255987ccc9721cf18ffa087bcd1ef
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:78e33a72a1df68d3b4341630a215626e79e45725e205f0355dc05df1b81ad68a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118557115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7015f2c475d511a251955877c2862016a4042512ba625ed905e69202f87e1a21`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:20f0d7c1e0ae8d99ea5f3501bfdda377cbef396dbd2cd8cd3c7fcd7597ee53b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.0 KB (786975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888e0f2341b28c595a15c556b7de2ef7b2193098083e90eb91c6b2ece4e62bec`

```dockerfile
```

-	Layers:
	-	`sha256:03a9e1145cddad6d8a9abd6d2286a33aeb8a425a56d89b267f34fa0ab3583d19`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 756.8 KB (756837 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eab5af778a6b0c2b95e4a1d9822191969109fc98ecde4850f146a3316b98a606`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 30.1 KB (30138 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:901dc6a38f98d1d06349951cdb3ca2e9ccd584800cd993df01c05cedf2843b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109859474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b564bb4cc4b98471f04d1e557a0ab96507f66c49cde4467b977093ec650c5f1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:77cc4a62cc1fb365e00a9a862478351523483c725343bef1b5b22f1771c43c5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.3 KB (787263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd8daf7609eefe181ab4e37963a8fa890fb51c1b9cc55d830dc3b342df02116e`

```dockerfile
```

-	Layers:
	-	`sha256:bb166e5b7fefafbf2b267ea78ffbc0f9f613d29a85403496612c8793e9042840`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 757.1 KB (757056 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c60cc6727f24722478cbb7a66e7581f4809f0f34e65a4820502072281db4b9df`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 30.2 KB (30207 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:1efae30b885343f906a11d382509e5177e7acfea1d63d786941beb83685656a6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c80204c95aef7d81b017a5be00b61a841eb55758b4e72413ee2e9e8b554b66c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140579964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fed477a4899a587575cfce5cbe1811f6de019caec34609033a2f3d941bed817`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59443f8fa96049a4cf8d67317e5f823d846af2f9af78a86594e6586e939ee05d`  
		Last Modified: Fri, 01 Sep 2023 02:51:26 GMT  
		Size: 1.4 MB (1362146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98316da633db7edabfb8501df1c0f234f4d1e7c858aebcaca1df19e76e81817b`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1a039201548858b79cf3cc0bc49dc786d9188355988b02c4470004b370cfe70`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c280db80bab216e68945db9df61354adbfdddbf9f78c1a9fbbaa87dec04cb28e`  
		Last Modified: Fri, 01 Sep 2023 02:51:26 GMT  
		Size: 20.7 MB (20659076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2604315ba333e12dc0c16f81f4b608f109b8741b369ef25dbb65064deb2270d5`  
		Last Modified: Fri, 01 Sep 2023 02:51:26 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:bdea2a36f08e4211670cb172e088b3161818a1218010d451073be58d4cc4504e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.6 KB (862575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c6f610a81a6bacc84e64edbced072acff4b58ea4554ee24b0983afb732297c`

```dockerfile
```

-	Layers:
	-	`sha256:99d26d8e565fe2f748370f1c1497d0f7405e6a6a110e026b4f7f1ee561e3a08a`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 831.5 KB (831481 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:be40bc8c58b56816d6e977289238cf2424927d70fdeea9ed2d194c7b15a12234`  
		Last Modified: Fri, 01 Sep 2023 02:51:25 GMT  
		Size: 31.1 KB (31094 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9c259ddd5697c1e260b1a381a100efa8bbb8864a0309a0d9420c3615a50b9d69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133723324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2638ec79b2a983a1bbd8c322a4462430d88303cdac2772d3bcfd670cb02cc156`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53878b06e1035044e67284bff906d3fc0df204161f5b009e9469da72477fa877`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 1.4 MB (1413168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e2ed305ea804e13233d7ec358d01eaf806b8d509f69d3278110f58ee9a8fcb0`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a6909dcb096132bdecc208fc905fcde36ac61c392a8e6c160889db94c44bbd7e`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0601c227926d4724b23791c8938b61d3968de7bb59646eeb00baee453e2ee4b`  
		Last Modified: Fri, 01 Sep 2023 02:51:54 GMT  
		Size: 22.4 MB (22449056 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6891c0c2c0ddd6a941fa5ca3131f2e83affd2cd56a3bcd57d8a6523d49ed56ca`  
		Last Modified: Fri, 01 Sep 2023 02:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:d7a1856277fbca39f82595a356a1db09e440393c79143820abfda61909f21af6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **862.9 KB (862864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542808f7074eafea27da73818e7c3a841ae6aa971753cd7344be0cacc363717a`

```dockerfile
```

-	Layers:
	-	`sha256:b04be43b56807d8c53ae591cb7ea77e35f514039e7e2514ebd1ac6b789dbc111`  
		Last Modified: Fri, 01 Sep 2023 02:51:53 GMT  
		Size: 831.7 KB (831712 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b9ffa9d0bdbba40c3831fffbe2b6a85e02ca3991b0da5a36a7e9c75ee60bed66`  
		Last Modified: Fri, 01 Sep 2023 02:51:52 GMT  
		Size: 31.2 KB (31152 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:git`

```console
$ docker pull docker@sha256:6d688492ebeb7902f180d9cfb589b5f9113fc758edabcb3b82df8f86c34b3f90
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:5b8c2653daf3eb59abbecf241dcbe12fa9e61813277bc3fd5248aea8c2d7a9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123492341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5317c041666eaf7f7c1893d9777527bbeb0decfd24ab715284ca14aa882241`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.5
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3011158b365f995fe31d93d2e89c0d74cddec794939e497e31c151f253bffae0`  
		Last Modified: Fri, 01 Sep 2023 02:51:15 GMT  
		Size: 4.9 MB (4935226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:git` - unknown; unknown

```console
$ docker pull docker@sha256:56759434ecca7c8b986be2f82694e0186fa7e71fb8082b98c7a31054c74a95f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **815.8 KB (815770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a38823fb0c813029d4604ae2b59a383f5d8792046d5cad3f4fe401f6ca41512`

```dockerfile
```

-	Layers:
	-	`sha256:16a3147ffec7dad2355c48f5a4b8a42e5565b75bbc599f9f595697873fb9a488`  
		Last Modified: Fri, 01 Sep 2023 02:51:15 GMT  
		Size: 802.8 KB (802841 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:46b98e19a72926c6941bb0d61072231db056038b7aa44f89150caf4a5a00756c`  
		Last Modified: Fri, 01 Sep 2023 02:51:14 GMT  
		Size: 12.9 KB (12929 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:24d3a88cd48430f0d644698d1af801887ffddb0d8352cc74052b8d3860af07a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114881054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:202873fceeb44d792f95943d18a54e6bce99ed53fe90c3fd9de41afc43c718e1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.5
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb2f25f8887e66ab99e5140de9e72c589ddf0d593cf2302e5542c41e6d9d23a7`  
		Last Modified: Fri, 01 Sep 2023 02:52:13 GMT  
		Size: 5.0 MB (5021580 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:git` - unknown; unknown

```console
$ docker pull docker@sha256:6c1a5b8a7f8c123e101d4a1486f20638eda931d4b9818d02dd2a57c629002205
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **813.8 KB (813820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9acb3f9b51cd6e0970a451952654ed286a169c5c191e60b39359ed64f58cbc04`

```dockerfile
```

-	Layers:
	-	`sha256:b86dfe324eab5a824ef87f50112eee9995f094746b70235f913c054ede3178e6`  
		Last Modified: Fri, 01 Sep 2023 02:52:12 GMT  
		Size: 803.1 KB (803056 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:625a52e6134a0e12843f919ad63bff5d924c7bdf915b14a862e500a75618580c`  
		Last Modified: Fri, 01 Sep 2023 02:52:12 GMT  
		Size: 10.8 KB (10764 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:latest`

```console
$ docker pull docker@sha256:3c6e4dca7a63c9a32a4e00da40461ce067f255987ccc9721cf18ffa087bcd1ef
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:78e33a72a1df68d3b4341630a215626e79e45725e205f0355dc05df1b81ad68a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118557115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7015f2c475d511a251955877c2862016a4042512ba625ed905e69202f87e1a21`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110ac87b2a727c4c5eb8ee9d1f3cbf1df239ca23abafeae9063664206effd46c`  
		Last Modified: Fri, 01 Sep 2023 00:50:56 GMT  
		Size: 2.0 MB (2014286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb3b0f7713d74440f758920f806604dc18003428e40c3adfda95ddf176663025`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 16.4 MB (16390651 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbab7b71df77ab8209d6010cd468cc0466afd60250f78f9e51bacc857d4e21df`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.5 MB (17459273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7115b760bf892077f958365d78ecee5bc1b2a945336a0987f6648a266a1cf769`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 17.8 MB (17826604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb33fbb55f1a2f4c4727afaf80cf10ec6af383a2beec12437d4b75e6cde4be61`  
		Last Modified: Fri, 01 Sep 2023 00:50:57 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30fbbdffb8e345217b129c74f11cd8eb4e954c9e99586444d271acdd729e2c30`  
		Last Modified: Fri, 01 Sep 2023 00:50:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55fb24f75fb015a50686f8ed2a930ff0792e4c58a6c9b8c55ff4f57a06dec820`  
		Last Modified: Fri, 01 Sep 2023 00:50:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aabff4d636f814f9819ae37656bba46b3252c9ff0d0370aaf21c1215f59ebe9f`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 7.1 MB (7080310 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d75ebc365546d935f8a58388c34faa054bb5aabb20d80366d97f5c8c2ab14972`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d54b27304de7143b6ca4436c805c33f9bd691b751177958bc907d5aebe91c8bd`  
		Last Modified: Fri, 01 Sep 2023 01:51:03 GMT  
		Size: 54.4 MB (54377552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b4b9734a564f97a28163b6f682e51485d82c5da5049e67fdc3bfdc17f178703`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc79f9020c0e1016b1ad9f651c87ce068efb1031e49f80f63a14892f59a6f17`  
		Last Modified: Fri, 01 Sep 2023 01:51:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:latest` - unknown; unknown

```console
$ docker pull docker@sha256:20f0d7c1e0ae8d99ea5f3501bfdda377cbef396dbd2cd8cd3c7fcd7597ee53b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.0 KB (786975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888e0f2341b28c595a15c556b7de2ef7b2193098083e90eb91c6b2ece4e62bec`

```dockerfile
```

-	Layers:
	-	`sha256:03a9e1145cddad6d8a9abd6d2286a33aeb8a425a56d89b267f34fa0ab3583d19`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 756.8 KB (756837 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eab5af778a6b0c2b95e4a1d9822191969109fc98ecde4850f146a3316b98a606`  
		Last Modified: Fri, 01 Sep 2023 01:51:00 GMT  
		Size: 30.1 KB (30138 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:901dc6a38f98d1d06349951cdb3ca2e9ccd584800cd993df01c05cedf2843b82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109859474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b564bb4cc4b98471f04d1e557a0ab96507f66c49cde4467b977093ec650c5f1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.21.0
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-x86_64'; 			sha256='08e549924823e97a3ea303c2309b812dfd5223b8be5ff96fe41bf75181ce0977'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv6'; 			sha256='058ec96bc81ddeb317d160a6dea5bd8ac65dc2e90afff86bcc31f3f818f3fc5a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-armv7'; 			sha256='d46dbbbf5723c45125277c7c75b757b22679962707b2276a6d52f35964583c42'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-aarch64'; 			sha256='5daf8d1a04cd649ad4a64221d0ca0cffcce33c740e60d5b15698545ce6d0436b'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-ppc64le'; 			sha256='fadbb72890d72f1246b213c453ec90cf494f4f8ea3dda2f63678de53a7e97c15'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-riscv64'; 			sha256='cd01536476864bd97c6ce3dfd317730535e51b2e252e9468de0379cc84298187'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-linux-s390x'; 			sha256='dfa8ab3ccc83311a2a4fddc43654de06c13cadc7caf629a0ddeceabd24bb6308'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4befa581740e7c16bd32ac4084ff4c844bf2f0b6d98a960ae6d432749bf00734`  
		Last Modified: Fri, 01 Sep 2023 01:23:07 GMT  
		Size: 16.3 MB (16283699 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e2b1302e6182b6780648863bfc0936d688ac0026408b2a8741d9eb4e5622860`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cf66d53f7de3b4c8526595dd272c84645feecb105970dce4af187d82a3486b6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4968bdb89a604162d04d897daf1522e03c1577cefc976964927eb0d96c49f6`  
		Last Modified: Fri, 01 Sep 2023 01:23:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36b1c38ea0707fa5c2044f95cdf9c13bdac6fe32c09dd351bfed7b736660e929`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 7.3 MB (7291226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e97e89203332a18b4257fd34a3391ba96940d2a8ee15b2a911989ad2ba5be6`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:167a7c4f8d8d35722c7a9ceae69bf71295cce21e754beb50f02db0682c415769`  
		Last Modified: Fri, 01 Sep 2023 01:53:35 GMT  
		Size: 49.7 MB (49718887 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39a0355ba5d9012607a678f687402ca9a1b7b8084b4e19a41e944d4080f3409a`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd53f0d7f1834bd427ab641a8e012e4a1d9d252191a5fe17322dd1e1f9ece852`  
		Last Modified: Fri, 01 Sep 2023 01:53:33 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:latest` - unknown; unknown

```console
$ docker pull docker@sha256:77cc4a62cc1fb365e00a9a862478351523483c725343bef1b5b22f1771c43c5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **787.3 KB (787263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd8daf7609eefe181ab4e37963a8fa890fb51c1b9cc55d830dc3b342df02116e`

```dockerfile
```

-	Layers:
	-	`sha256:bb166e5b7fefafbf2b267ea78ffbc0f9f613d29a85403496612c8793e9042840`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 757.1 KB (757056 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c60cc6727f24722478cbb7a66e7581f4809f0f34e65a4820502072281db4b9df`  
		Last Modified: Fri, 01 Sep 2023 01:53:32 GMT  
		Size: 30.2 KB (30207 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:dde81d7f2600ac22de6bfa8c7a07c4881524d1f45b803aebd69de7bdfcf5c1ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `docker:windowsservercore` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:f036505370e71fe6013e09eae58982bf19d779f261af758f03c3e0ca6e959fb6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791668357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e53ea0a0809793c899cf1e9cb3de891686b773872e92353ab6872f21093da2aa`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:15:13 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:15:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:15:45 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:15:46 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:15:47 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:16:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:16:18 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:16:19 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:16:20 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:16:48 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901deda7922d35795e3d4991c73cb1cab61c3b129a15bb04b3e7d123d0de0b60`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027eea06d0080daedf5ef523c93e969ec807b2a65dcd1021840f7e70db9f2a2`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486b855c5d89d784c7e85907326d05d26635441a754e9e426498138dc6fdd419`  
		Last Modified: Mon, 24 Jul 2023 22:21:36 GMT  
		Size: 17.5 MB (17465980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc0f5529504e867302acf706f596cbbe06f751ce571b8bbfd746e8b44b35db`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56660e6caa6afda40f70e06ad0adb7679ddd6362b112bf884959a9daa03f43ff`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da8ddac8b835e0b3f3ca4464213330eb286a31ea01b6d75b4f6353e2511083`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4f9f340fe4664aa4293c04caf8451644aa2f34e790ed08c60628376b6dc39`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 17.9 MB (17902937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8577eb74030f9da73f6f4a8dfc61abfe3a516bc71c0cdaf04aa41aaa5dfea7f`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2ae56b025d396a3597cfb2e9efa8779218d8b955a42b2d8dac86568f88eac8`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4b75aa8a819fda1544fe1e0e3befc8d1863729ec8df3d31f37b4e8c7608d9e`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966a418a3938e0554b46c43cacefdbe319c43861b807d6ac33e85e49c1c98d38`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 18.5 MB (18458205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:4ced44b2a9980116f078f1d4848c10ee0283902b9a1d508e6cf4aafbce3d3868
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993906076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755cf7950481c506283cd30fb68ffb4affa45ca5275b3aa5f346caa36f1dd253`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:16:56 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:16:57 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:18:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:18:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:18:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:18:10 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:19:23 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:19:25 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:20:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2828f54bc3b0d02a4c8b471fc44b6318a0be2b9409bb1c6555ae5430316de`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afa9d718105d43e5cf00564b995fe8b1f6259a84386406d7d566c2a467be18`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfca0ac7b7aebd4db3ee5b56977ee4242ec31f4262b541a5cb9e91041294a3f`  
		Last Modified: Mon, 24 Jul 2023 22:21:57 GMT  
		Size: 17.6 MB (17638105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e03760602364c4d21bbcda283366105ce48a61694ee415d935a4ce22aef03d`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcacb30c234bcade9db59bff00606d6e4432c65428ddb7a5919d82172700b4e`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a0b8e41707d2d1eb6d6ff3431d0d0b4f87e909f3722abeb94c44a3e9740261`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6415f8b4089b9fa213c16a68b1060faa1bd792ab011b27f358a326a7eafadd3a`  
		Last Modified: Mon, 24 Jul 2023 22:21:55 GMT  
		Size: 17.9 MB (17890313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67080a6fba2e9f7f1ab50eff043a6e8c7dea8ca31779d1dd087bd269f6be6d97`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a4edc0e994d2c782f76fa0ec93913467d6e3388943dd7884c38c1d444b0fad`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d533ad3c0b792a6a69b0573489d6628605c7fd8514021d65a9063886ed3e36`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e50d630030b8b04b07b76780e17708870d4943248c548a60a040099e237f0`  
		Last Modified: Mon, 24 Jul 2023 22:21:56 GMT  
		Size: 18.4 MB (18445548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:a785eccd876138d5172dd1cf10d7e79ab801281784dbe5d8912b95fe8f2e8266
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull docker@sha256:4ced44b2a9980116f078f1d4848c10ee0283902b9a1d508e6cf4aafbce3d3868
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1993906076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755cf7950481c506283cd30fb68ffb4affa45ca5275b3aa5f346caa36f1dd253`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Fri, 07 Jul 2023 08:17:39 GMT
RUN Install update 10.0.17763.4645
# Thu, 13 Jul 2023 20:32:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:29:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:16:56 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:16:57 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:18:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:18:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:18:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:18:10 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:19:23 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:19:24 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:19:25 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:20:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36dba1ee29cd36713c8785a5de7dd2a487244d734ed4c5e7b0a6890bffb806e`  
		Last Modified: Tue, 11 Jul 2023 18:27:38 GMT  
		Size: 289.1 MB (289068746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e991bb72ebb8bf12a5cb5fcb2075d938e3508db6634bdfe6a5bb73e4c612051`  
		Last Modified: Thu, 13 Jul 2023 21:08:51 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb4cf79c2f4d846a90b33b635df0502f42d01fd0ee86b04449dfcec7cef5db`  
		Last Modified: Fri, 14 Jul 2023 00:39:45 GMT  
		Size: 230.5 KB (230461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb2828f54bc3b0d02a4c8b471fc44b6318a0be2b9409bb1c6555ae5430316de`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afa9d718105d43e5cf00564b995fe8b1f6259a84386406d7d566c2a467be18`  
		Last Modified: Mon, 24 Jul 2023 22:21:54 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfca0ac7b7aebd4db3ee5b56977ee4242ec31f4262b541a5cb9e91041294a3f`  
		Last Modified: Mon, 24 Jul 2023 22:21:57 GMT  
		Size: 17.6 MB (17638105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e03760602364c4d21bbcda283366105ce48a61694ee415d935a4ce22aef03d`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcacb30c234bcade9db59bff00606d6e4432c65428ddb7a5919d82172700b4e`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a0b8e41707d2d1eb6d6ff3431d0d0b4f87e909f3722abeb94c44a3e9740261`  
		Last Modified: Mon, 24 Jul 2023 22:21:52 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6415f8b4089b9fa213c16a68b1060faa1bd792ab011b27f358a326a7eafadd3a`  
		Last Modified: Mon, 24 Jul 2023 22:21:55 GMT  
		Size: 17.9 MB (17890313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67080a6fba2e9f7f1ab50eff043a6e8c7dea8ca31779d1dd087bd269f6be6d97`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a4edc0e994d2c782f76fa0ec93913467d6e3388943dd7884c38c1d444b0fad`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d533ad3c0b792a6a69b0573489d6628605c7fd8514021d65a9063886ed3e36`  
		Last Modified: Mon, 24 Jul 2023 22:21:50 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e50d630030b8b04b07b76780e17708870d4943248c548a60a040099e237f0`  
		Last Modified: Mon, 24 Jul 2023 22:21:56 GMT  
		Size: 18.4 MB (18445548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:6446b2f91d9e216ea9430abc2619ab0abfb508c8a2fd55be5d52441b0a04eabc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull docker@sha256:f036505370e71fe6013e09eae58982bf19d779f261af758f03c3e0ca6e959fb6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1791668357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e53ea0a0809793c899cf1e9cb3de891686b773872e92353ab6872f21093da2aa`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 20:29:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 14 Jul 2023 00:27:02 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Mon, 24 Jul 2023 22:15:13 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 22:15:14 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.5.zip
# Mon, 24 Jul 2023 22:15:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:15:45 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 22:15:46 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.windows-amd64.exe
# Mon, 24 Jul 2023 22:15:47 GMT
ENV DOCKER_BUILDX_SHA256=d9419c0838c8a08c2da28fcee585f48926c4dd64e5be1d96eb55da12fa3332d9
# Mon, 24 Jul 2023 22:16:17 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Mon, 24 Jul 2023 22:16:18 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 22:16:19 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-windows-x86_64.exe
# Mon, 24 Jul 2023 22:16:20 GMT
ENV DOCKER_COMPOSE_SHA256=d381f0697ce5d469917ab343dd4e59ae404865af8a5cf43178005bf400f0113a
# Mon, 24 Jul 2023 22:16:48 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e3828ab9c4326158b6161915d8bad87619b3107529ab32863eb31b684d127`  
		Last Modified: Thu, 13 Jul 2023 21:07:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e9081d64b30fd475f9121be79bf5756df76494ba98c3208a0e6c46228f7f6`  
		Last Modified: Fri, 14 Jul 2023 00:39:18 GMT  
		Size: 463.2 KB (463247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901deda7922d35795e3d4991c73cb1cab61c3b129a15bb04b3e7d123d0de0b60`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d027eea06d0080daedf5ef523c93e969ec807b2a65dcd1021840f7e70db9f2a2`  
		Last Modified: Mon, 24 Jul 2023 22:21:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486b855c5d89d784c7e85907326d05d26635441a754e9e426498138dc6fdd419`  
		Last Modified: Mon, 24 Jul 2023 22:21:36 GMT  
		Size: 17.5 MB (17465980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc0f5529504e867302acf706f596cbbe06f751ce571b8bbfd746e8b44b35db`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56660e6caa6afda40f70e06ad0adb7679ddd6362b112bf884959a9daa03f43ff`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60da8ddac8b835e0b3f3ca4464213330eb286a31ea01b6d75b4f6353e2511083`  
		Last Modified: Mon, 24 Jul 2023 22:21:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4f9f340fe4664aa4293c04caf8451644aa2f34e790ed08c60628376b6dc39`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 17.9 MB (17902937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8577eb74030f9da73f6f4a8dfc61abfe3a516bc71c0cdaf04aa41aaa5dfea7f`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2ae56b025d396a3597cfb2e9efa8779218d8b955a42b2d8dac86568f88eac8`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4b75aa8a819fda1544fe1e0e3befc8d1863729ec8df3d31f37b4e8c7608d9e`  
		Last Modified: Mon, 24 Jul 2023 22:21:29 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966a418a3938e0554b46c43cacefdbe319c43861b807d6ac33e85e49c1c98d38`  
		Last Modified: Mon, 24 Jul 2023 22:21:34 GMT  
		Size: 18.5 MB (18458205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
