<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

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
-	[`docker:24.0.7`](#docker2407)
-	[`docker:24.0.7-alpine3.18`](#docker2407-alpine318)
-	[`docker:24.0.7-cli`](#docker2407-cli)
-	[`docker:24.0.7-cli-alpine3.18`](#docker2407-cli-alpine318)
-	[`docker:24.0.7-dind`](#docker2407-dind)
-	[`docker:24.0.7-dind-alpine3.18`](#docker2407-dind-alpine318)
-	[`docker:24.0.7-dind-rootless`](#docker2407-dind-rootless)
-	[`docker:24.0.7-git`](#docker2407-git)
-	[`docker:24.0.7-windowsservercore`](#docker2407-windowsservercore)
-	[`docker:24.0.7-windowsservercore-1809`](#docker2407-windowsservercore-1809)
-	[`docker:24.0.7-windowsservercore-ltsc2022`](#docker2407-windowsservercore-ltsc2022)
-	[`docker:cli`](#dockercli)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:24`

```console
$ docker pull docker@sha256:0752ca4e936da012c173c119217c0f9599b3b191c1557e53206d5d06d2627580
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24` - linux; amd64

```console
$ docker pull docker@sha256:74e78208fc18da48ddf8b569abe21563730845c312130bd0f0b059746a7e10f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118536604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114405a05c1ea1579eada94100ea1262ec351ce96625fed47684ed05ef48f52f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24` - unknown; unknown

```console
$ docker pull docker@sha256:32bcc64f2342b9b4d239bc563b6136a3f2c8c4ec7c0b1b8a0159ea159131c66d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.0 KB (732982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742d72f2efb6cda226ca77f818decb8c96a54c83fd8a5ee45ebd0f4cb4432493`

```dockerfile
```

-	Layers:
	-	`sha256:dfb66480a0d5e8b3e0f100d57763a66e5f53dd59649388029d7395a9b9e22985`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 702.9 KB (702854 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0a6ef7e7265b4a34b64183232c7c53a3e9d151b070323f48ecc62433addde4f5`  
		Last Modified: Thu, 19 Oct 2023 03:15:28 GMT  
		Size: 30.1 KB (30128 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24` - linux; arm variant v6

```console
$ docker pull docker@sha256:3b9c201a958ca8287e09b71e46d225852effd86c080dbf9bf4bd8887c96bb393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111730242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378ee0fe8270d7a0b77b97ec7144132b710f93b2f605f4d58d7ed903ea921700`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c183f2f030545a92229eb1d957a3d27a632065fd3e889fc1821df61e705e8e`  
		Last Modified: Thu, 19 Oct 2023 04:44:13 GMT  
		Size: 7.2 MB (7173654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd6749d2a6490b564ea75608c30867d181bee08328b6d9261af8546e213744`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb92ac4eb0bdd3c74efcc1b6a7da46be2c315b825f313701621f05757da245`  
		Last Modified: Thu, 19 Oct 2023 04:44:20 GMT  
		Size: 50.9 MB (50936158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7db9246e2c193486442265643f2a84289eec2df6ada560c67809901314b47`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab1b151f3d0bcd981b77eecf172b682f3474cdc742f366600d378b119a5c9a`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 2.8 KB (2796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24` - linux; arm variant v7

```console
$ docker pull docker@sha256:d540c1e08caba133a46bf8d458253158143f00ad92da9a6b41e545da381639bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110546565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83f5a2ae6d81508dcfad2aa9837a2bd5b0fb43a928565a117e6f92a7f1b2052e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04261eaf858b9479a1d7176630c8bbd7196ea372d024b17b1e7354e0d24c16c2`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 6.5 MB (6469635 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34bf6d61289016c22a2a8fd3022160a5358e1ad2d6c72c7dc5cf382cddd15653`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7f6001c2b47951d06a099362aeb56a04176dfd1c1fc0ddc5c1bdb8c0a34474`  
		Last Modified: Thu, 19 Oct 2023 06:54:18 GMT  
		Size: 50.9 MB (50936137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4c99b97523144da18c38ab3adb6cf7c3d7f8b070e5eb9942761666f8fa9d58`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053b0aba8a62b2d1ebadcd710799a63584f106e45cda4ac37ad86a107d7de70f`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 2.8 KB (2797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24` - unknown; unknown

```console
$ docker pull docker@sha256:0fb45f97b44a9fd07d91798156de1c8e5feee9ef91bbcb918dca2552283673b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.3 KB (733269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f05479573db10e995800169c17cc75dc7e02754a961730757f0ab0e57eefa3`

```dockerfile
```

-	Layers:
	-	`sha256:79ed0876afb43b9f34c2ad8abab3df2b215642df1353865e7f19b939f12992cd`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 702.9 KB (702936 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ff33b8332a65e8707424c58afd06e0da9b0c83886d7078e89615993510af5044`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 30.3 KB (30333 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c4f291842cc372be20d42c77bf29c3cc5f302989dfd0b6de574ca75a2a444087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109839965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b3167e27ccfb4dfa4fa0fcaa3fea4c2026e8d09cc3c209d3db8cb8b27224e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24` - unknown; unknown

```console
$ docker pull docker@sha256:9d66b06e4f1158baf427971f83571abe635d5bc5ef22d8cc4344f9c7b5e11fe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.1 KB (733077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625c5a6acfba0dd0de4524db7ddc2c0be3bb531c9febd06badb4e8bf179ba5c5`

```dockerfile
```

-	Layers:
	-	`sha256:53f6704407130f584a1f72df612b15e8dc8092b8dba809328e0a1f83ecd338d6`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 702.9 KB (702879 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3f75f2b4b1808936dcfc233ce3ac1d12741e81d0459cbf547be77385a4aee3dc`  
		Last Modified: Thu, 19 Oct 2023 08:39:22 GMT  
		Size: 30.2 KB (30198 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24-cli`

```console
$ docker pull docker@sha256:4865ba3135696b1c0e1b6bf323a5ef9402013244a69280543cf16aebc1da2b49
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-cli` - linux; amd64

```console
$ docker pull docker@sha256:789420937a26ebec564c47161164faf74d9de353539273ae7904229a5f3e5b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57099399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b67d930a0cca6847a99b95b85b36a9ac12cee20a21287127b14da64d1946bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:b5d5d8838c5713859922b1a19a03c004867d85b812ab5e92e1545f84b1234eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 KB (399302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02683e982681bcbf4a1a62ba5f77e9d89b24b9b0bb5fe8237ff69aaadfdb3a04`

```dockerfile
```

-	Layers:
	-	`sha256:14374abf45bae1e3e070c4baa97b47f1475d9a0a928e5bf3cc2f2ea739cb43da`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 363.5 KB (363519 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c6a63e5a737768c94345029588b7b2cbbd160667d93d710f706e40ed91413929`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 35.8 KB (35783 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-cli` - linux; arm variant v6

```console
$ docker pull docker@sha256:ff0fd928e653fa68ef74a55176e13ebb8dd2f8ac47b4f14248f056afe46a2171
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53615303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d70a15d2461e904100529d3d28e6f26d3bdc4ea9bd0ab8993082f5b83fa1d2b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-cli` - linux; arm variant v7

```console
$ docker pull docker@sha256:a26fe5863bb4158d8299df0e9133af0dc97ac7ed7537380d3990fa1e8f5e51bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53135663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b1d618bb96b56678094389031e7c08dce5ebe736b62ff92c7d71b8622c9221`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:efa475bd4aa53d695ee55df6c73d572d2be01e54e73a49674ed227b469da118d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 KB (399321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a054df93652b09d80b5c38006fbdceb1feaa8075f7428900cedf3a2b791667db`

```dockerfile
```

-	Layers:
	-	`sha256:39396a9f1f54b6de0baaee6a76517409540d0c9fdf05e89e7b24aafa80096638`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 363.6 KB (363561 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ffd4d5053927223f1562259738aeb32f076000d0b6c34f5982815d8e88e92bf1`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 35.8 KB (35760 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:55e2b2dfc3e8cac05521cc6a4f9c8aa97cf1290052cd1f54a45e17136b5aceaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52855252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fa15b6055e9eeaad38c87602b9548b90fda56c3bb21d21d9d03e564ca6f2764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:0d00e3c266fb4af54c0711d8c022d24ee55d46d9fa5b81fda8d4d33ce991d1c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.2 KB (399163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0095154483d0f23ec2378e28784fa23c02947429d9887390a48470bae96fdf9`

```dockerfile
```

-	Layers:
	-	`sha256:af0e147ec9339cbdc6caa4eef3cea829589eb0ddb71b39c8b80ae52514d3549d`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 363.5 KB (363534 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:279d55a79ed6483042d0e4381f1a5fd0c7d4778230aba7c78f42331aa6b5bb6d`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 35.6 KB (35629 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24-dind`

```console
$ docker pull docker@sha256:0752ca4e936da012c173c119217c0f9599b3b191c1557e53206d5d06d2627580
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-dind` - linux; amd64

```console
$ docker pull docker@sha256:74e78208fc18da48ddf8b569abe21563730845c312130bd0f0b059746a7e10f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118536604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114405a05c1ea1579eada94100ea1262ec351ce96625fed47684ed05ef48f52f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind` - unknown; unknown

```console
$ docker pull docker@sha256:32bcc64f2342b9b4d239bc563b6136a3f2c8c4ec7c0b1b8a0159ea159131c66d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.0 KB (732982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742d72f2efb6cda226ca77f818decb8c96a54c83fd8a5ee45ebd0f4cb4432493`

```dockerfile
```

-	Layers:
	-	`sha256:dfb66480a0d5e8b3e0f100d57763a66e5f53dd59649388029d7395a9b9e22985`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 702.9 KB (702854 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0a6ef7e7265b4a34b64183232c7c53a3e9d151b070323f48ecc62433addde4f5`  
		Last Modified: Thu, 19 Oct 2023 03:15:28 GMT  
		Size: 30.1 KB (30128 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:3b9c201a958ca8287e09b71e46d225852effd86c080dbf9bf4bd8887c96bb393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111730242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378ee0fe8270d7a0b77b97ec7144132b710f93b2f605f4d58d7ed903ea921700`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c183f2f030545a92229eb1d957a3d27a632065fd3e889fc1821df61e705e8e`  
		Last Modified: Thu, 19 Oct 2023 04:44:13 GMT  
		Size: 7.2 MB (7173654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd6749d2a6490b564ea75608c30867d181bee08328b6d9261af8546e213744`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb92ac4eb0bdd3c74efcc1b6a7da46be2c315b825f313701621f05757da245`  
		Last Modified: Thu, 19 Oct 2023 04:44:20 GMT  
		Size: 50.9 MB (50936158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7db9246e2c193486442265643f2a84289eec2df6ada560c67809901314b47`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab1b151f3d0bcd981b77eecf172b682f3474cdc742f366600d378b119a5c9a`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 2.8 KB (2796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:d540c1e08caba133a46bf8d458253158143f00ad92da9a6b41e545da381639bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110546565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83f5a2ae6d81508dcfad2aa9837a2bd5b0fb43a928565a117e6f92a7f1b2052e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04261eaf858b9479a1d7176630c8bbd7196ea372d024b17b1e7354e0d24c16c2`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 6.5 MB (6469635 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34bf6d61289016c22a2a8fd3022160a5358e1ad2d6c72c7dc5cf382cddd15653`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7f6001c2b47951d06a099362aeb56a04176dfd1c1fc0ddc5c1bdb8c0a34474`  
		Last Modified: Thu, 19 Oct 2023 06:54:18 GMT  
		Size: 50.9 MB (50936137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4c99b97523144da18c38ab3adb6cf7c3d7f8b070e5eb9942761666f8fa9d58`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053b0aba8a62b2d1ebadcd710799a63584f106e45cda4ac37ad86a107d7de70f`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 2.8 KB (2797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind` - unknown; unknown

```console
$ docker pull docker@sha256:0fb45f97b44a9fd07d91798156de1c8e5feee9ef91bbcb918dca2552283673b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.3 KB (733269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f05479573db10e995800169c17cc75dc7e02754a961730757f0ab0e57eefa3`

```dockerfile
```

-	Layers:
	-	`sha256:79ed0876afb43b9f34c2ad8abab3df2b215642df1353865e7f19b939f12992cd`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 702.9 KB (702936 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ff33b8332a65e8707424c58afd06e0da9b0c83886d7078e89615993510af5044`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 30.3 KB (30333 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c4f291842cc372be20d42c77bf29c3cc5f302989dfd0b6de574ca75a2a444087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109839965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b3167e27ccfb4dfa4fa0fcaa3fea4c2026e8d09cc3c209d3db8cb8b27224e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind` - unknown; unknown

```console
$ docker pull docker@sha256:9d66b06e4f1158baf427971f83571abe635d5bc5ef22d8cc4344f9c7b5e11fe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.1 KB (733077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625c5a6acfba0dd0de4524db7ddc2c0be3bb531c9febd06badb4e8bf179ba5c5`

```dockerfile
```

-	Layers:
	-	`sha256:53f6704407130f584a1f72df612b15e8dc8092b8dba809328e0a1f83ecd338d6`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 702.9 KB (702879 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3f75f2b4b1808936dcfc233ce3ac1d12741e81d0459cbf547be77385a4aee3dc`  
		Last Modified: Thu, 19 Oct 2023 08:39:22 GMT  
		Size: 30.2 KB (30198 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24-dind-rootless`

```console
$ docker pull docker@sha256:71bee62410f63c1b313d3a6b14f4ed657b448ecacb69a8098deff9ae53010b19
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5e6bef9db0bb59ded0834ccf7953b7ff4fba228c0b62f40d0dd84cf6fb929f6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140560736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6a3d03b4335d3c77905757053aeb7d3b276a299ea360d049ca5319426071b2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
USER rootless
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51331694e511817c7af194b499671898dc666d5a1246478039ac7cbe4b8bb928`  
		Last Modified: Thu, 19 Oct 2023 04:06:27 GMT  
		Size: 1.4 MB (1362179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a05bb47bbc48d4359156ea4ad95b35ed79c5a16503b490d39fde39f5743dd580`  
		Last Modified: Thu, 19 Oct 2023 04:06:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6841788dd624e9c7343e25f901454d5e09cd3ad4b3c0f9418f66c503ac848711`  
		Last Modified: Thu, 19 Oct 2023 04:06:27 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:729437d46a9fe2fe36b282defe38f2a4f0f39bd398b9f47b8a9ac2d5a9f4987c`  
		Last Modified: Thu, 19 Oct 2023 04:06:29 GMT  
		Size: 20.7 MB (20660322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15ae4caf84a6e8590b6225b631a1bfcf10f417ce106af28c49f7eb72196effbe`  
		Last Modified: Thu, 19 Oct 2023 04:06:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:6c000e6ecf7be401312530c955dc48603d0a301b2450302fbf29aba6f5e21623
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **777.1 KB (777130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a26ec4c100e1cb1da7753bee45b48cebc2266ebf28d99d704b0735db7bcbed`

```dockerfile
```

-	Layers:
	-	`sha256:8e41c8d50b467c850c3ff7e4f049fd4a2ce5b3787fd13da5389e4759a8672bb4`  
		Last Modified: Thu, 19 Oct 2023 04:06:26 GMT  
		Size: 746.0 KB (746048 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9de2eee0dcd20e7a1709a88819367161618aea1ed5d944d63dd6427dc419368a`  
		Last Modified: Thu, 19 Oct 2023 04:06:26 GMT  
		Size: 31.1 KB (31082 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:42441ba25e32850da9df550a240c5583e37bf21de7190d1840dc2aeaa70fed6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133703554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2a5f3b9f1aeada90e298c000d285e31ea0b29c4397c4dfaccef88eceb389fe2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
USER rootless
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bca473d3d6cc9b124cd49408a18f60218bcd8cb366e56a3b16e18e934228b2e1`  
		Last Modified: Thu, 19 Oct 2023 09:04:35 GMT  
		Size: 1.4 MB (1413154 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b973c3488b8d0250e2ae2c52cb652304a7abab1644c18e1207d9a3822bd1d17`  
		Last Modified: Thu, 19 Oct 2023 09:04:35 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90f01a8ca69a1582ddbe39d495781d8b154de69989d89ae55e04dab61fb49ccf`  
		Last Modified: Thu, 19 Oct 2023 09:04:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:442dfac109ba1720ef139f23f3b17d5b7f196c11075a86a842966d816b0f36dc`  
		Last Modified: Thu, 19 Oct 2023 09:04:37 GMT  
		Size: 22.4 MB (22448806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6733ab06e49858ad2a4afb9b4f52aeb72694046b855fbec5a8728e4fa51ae8d9`  
		Last Modified: Thu, 19 Oct 2023 09:04:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:34bf7fdd92e10f28722d896db78e5cd89f9251a276dece636173aaeb4c16f65f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **777.2 KB (777203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85afdc700cb054338ac5d23874d67d86ef33460e2762b701dd5c006e0d7a3e`

```dockerfile
```

-	Layers:
	-	`sha256:5f3f7869dda1395b108e38a74799402ec328daa66f758066ebe5c399dddfcb98`  
		Last Modified: Thu, 19 Oct 2023 09:04:34 GMT  
		Size: 746.1 KB (746061 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8950340c6d28e1c91dd6419aa4a01f1690740ed770b0a9efce2e078381919c5d`  
		Last Modified: Thu, 19 Oct 2023 09:04:34 GMT  
		Size: 31.1 KB (31142 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24-git`

```console
$ docker pull docker@sha256:cc2d2f4fca4d5c78508ee85db7af568a08f97559c2e20f69bb91e498b885dde2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-git` - linux; amd64

```console
$ docker pull docker@sha256:00b5b6a006ff69369d3971b2055bb2da7000a8e9971005f36879dab92de4ef98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123479937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be7e484a4dfd5b5dd06b7c0ed89758b50908fe0db096183d8cfdadb98a0b9b4`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6466ad09233589febc284d1c1f41a4c39f0fa0a5b1aa1bea85891ddba7739539`  
		Last Modified: Thu, 19 Oct 2023 04:06:29 GMT  
		Size: 4.9 MB (4943333 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-git` - unknown; unknown

```console
$ docker pull docker@sha256:65ed97cbd3ef22714b0a305e8307d5f87083d7fbf5e6376676b5fa3c943802c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **761.5 KB (761546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1783abf6e7c52303433757998ff19429c08b9aaeb3ccac7040cd08561fd00567`

```dockerfile
```

-	Layers:
	-	`sha256:08aaa8df3b54134a7b381b45ace0ac59183c9c1ed7a0ee0ab1d7454b19f52e87`  
		Last Modified: Thu, 19 Oct 2023 04:06:28 GMT  
		Size: 748.6 KB (748627 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:68cbef04771d10485635bfb7269952da578567db38de22b31f69ff3230ed6002`  
		Last Modified: Thu, 19 Oct 2023 04:06:28 GMT  
		Size: 12.9 KB (12919 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:ec2b91d49b9ed4c997600e5cee4690bbf12f91fcc6f65820802224dcf0649102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116670835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2018e784dfa20e080841e3eebef1a00d61c9ee949b235eebd7d112f933e43aae`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c183f2f030545a92229eb1d957a3d27a632065fd3e889fc1821df61e705e8e`  
		Last Modified: Thu, 19 Oct 2023 04:44:13 GMT  
		Size: 7.2 MB (7173654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd6749d2a6490b564ea75608c30867d181bee08328b6d9261af8546e213744`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb92ac4eb0bdd3c74efcc1b6a7da46be2c315b825f313701621f05757da245`  
		Last Modified: Thu, 19 Oct 2023 04:44:20 GMT  
		Size: 50.9 MB (50936158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7db9246e2c193486442265643f2a84289eec2df6ada560c67809901314b47`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab1b151f3d0bcd981b77eecf172b682f3474cdc742f366600d378b119a5c9a`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 2.8 KB (2796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cee337b7b489249be7352c134317ce799195091ca6ad9932e7dbb524056e694`  
		Last Modified: Thu, 19 Oct 2023 05:42:21 GMT  
		Size: 4.9 MB (4940593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:3f88c8c70b39ae8f9461ffc542ef86a2fabfdf9ca41f98409d3794bee3100983
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115038908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9eadcbcc6c8f6ff1f8fd987d415935906d56012fe5073c65f8b6f39c0bc851`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04261eaf858b9479a1d7176630c8bbd7196ea372d024b17b1e7354e0d24c16c2`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 6.5 MB (6469635 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34bf6d61289016c22a2a8fd3022160a5358e1ad2d6c72c7dc5cf382cddd15653`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7f6001c2b47951d06a099362aeb56a04176dfd1c1fc0ddc5c1bdb8c0a34474`  
		Last Modified: Thu, 19 Oct 2023 06:54:18 GMT  
		Size: 50.9 MB (50936137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4c99b97523144da18c38ab3adb6cf7c3d7f8b070e5eb9942761666f8fa9d58`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053b0aba8a62b2d1ebadcd710799a63584f106e45cda4ac37ad86a107d7de70f`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 2.8 KB (2797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:faf69bf10977965d99584c9aa00ac2e56fcb290a76eb1b7ba85c0cb17bff1da7`  
		Last Modified: Thu, 19 Oct 2023 07:11:28 GMT  
		Size: 4.5 MB (4492343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-git` - unknown; unknown

```console
$ docker pull docker@sha256:4f879efbd2090c1d2b2cb5380894406c986d9c23d7bf5afab6239796a7a3d66e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.1 KB (764149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d8750ed6e0566af35a64780d09daa5f9efdce8d111bac971ca704db5f52266`

```dockerfile
```

-	Layers:
	-	`sha256:1a0bff8d09f12570e3bdeb2706176068cddb197ab88e9ab2a2c7e7d6420232f0`  
		Last Modified: Thu, 19 Oct 2023 07:11:27 GMT  
		Size: 751.1 KB (751136 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:449e4f641245d33dbfe27dc3896f900ff0e773d282d806a6bdcfc8889b87cd69`  
		Last Modified: Thu, 19 Oct 2023 07:11:26 GMT  
		Size: 13.0 KB (13013 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:56fe9ab697bcb19fac6ddaba066c07156501ee39bb6f3de0098f4e11c834f46a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114877213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba700d423fdbd813634e9f5cd0fe826bf010bb037fe94cd422bef6a228399591`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6fdb8b91a9d574fac2adf6328b5d9d9ca0a3cc3220b38be475464889bb4aabf1`  
		Last Modified: Thu, 19 Oct 2023 09:04:59 GMT  
		Size: 5.0 MB (5037248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-git` - unknown; unknown

```console
$ docker pull docker@sha256:ce3b404e88dabff4445d39b8023e27dbcce575a4557bf486040f25fc0ef2f321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.4 KB (759394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36ec390ccae563be564a2d7970e81cff0ac8913eb61995d0e9afc1794357edee`

```dockerfile
```

-	Layers:
	-	`sha256:3d8c86ce8c5a9620cd072924c764aca54ca673f50ef4b56c47d3d137705c9e6c`  
		Last Modified: Thu, 19 Oct 2023 09:04:57 GMT  
		Size: 748.6 KB (748640 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9176acf5c3f61dc56fed8244db8793faf53232b5ddb1160aaa2478c9fb8ce95d`  
		Last Modified: Thu, 19 Oct 2023 09:04:57 GMT  
		Size: 10.8 KB (10754 bytes)  
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
$ docker pull docker@sha256:0752ca4e936da012c173c119217c0f9599b3b191c1557e53206d5d06d2627580
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0` - linux; amd64

```console
$ docker pull docker@sha256:74e78208fc18da48ddf8b569abe21563730845c312130bd0f0b059746a7e10f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118536604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114405a05c1ea1579eada94100ea1262ec351ce96625fed47684ed05ef48f52f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0` - unknown; unknown

```console
$ docker pull docker@sha256:32bcc64f2342b9b4d239bc563b6136a3f2c8c4ec7c0b1b8a0159ea159131c66d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.0 KB (732982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742d72f2efb6cda226ca77f818decb8c96a54c83fd8a5ee45ebd0f4cb4432493`

```dockerfile
```

-	Layers:
	-	`sha256:dfb66480a0d5e8b3e0f100d57763a66e5f53dd59649388029d7395a9b9e22985`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 702.9 KB (702854 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0a6ef7e7265b4a34b64183232c7c53a3e9d151b070323f48ecc62433addde4f5`  
		Last Modified: Thu, 19 Oct 2023 03:15:28 GMT  
		Size: 30.1 KB (30128 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0` - linux; arm variant v6

```console
$ docker pull docker@sha256:3b9c201a958ca8287e09b71e46d225852effd86c080dbf9bf4bd8887c96bb393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111730242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378ee0fe8270d7a0b77b97ec7144132b710f93b2f605f4d58d7ed903ea921700`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c183f2f030545a92229eb1d957a3d27a632065fd3e889fc1821df61e705e8e`  
		Last Modified: Thu, 19 Oct 2023 04:44:13 GMT  
		Size: 7.2 MB (7173654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd6749d2a6490b564ea75608c30867d181bee08328b6d9261af8546e213744`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb92ac4eb0bdd3c74efcc1b6a7da46be2c315b825f313701621f05757da245`  
		Last Modified: Thu, 19 Oct 2023 04:44:20 GMT  
		Size: 50.9 MB (50936158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7db9246e2c193486442265643f2a84289eec2df6ada560c67809901314b47`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab1b151f3d0bcd981b77eecf172b682f3474cdc742f366600d378b119a5c9a`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 2.8 KB (2796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0` - linux; arm variant v7

```console
$ docker pull docker@sha256:d540c1e08caba133a46bf8d458253158143f00ad92da9a6b41e545da381639bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110546565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83f5a2ae6d81508dcfad2aa9837a2bd5b0fb43a928565a117e6f92a7f1b2052e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04261eaf858b9479a1d7176630c8bbd7196ea372d024b17b1e7354e0d24c16c2`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 6.5 MB (6469635 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34bf6d61289016c22a2a8fd3022160a5358e1ad2d6c72c7dc5cf382cddd15653`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7f6001c2b47951d06a099362aeb56a04176dfd1c1fc0ddc5c1bdb8c0a34474`  
		Last Modified: Thu, 19 Oct 2023 06:54:18 GMT  
		Size: 50.9 MB (50936137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4c99b97523144da18c38ab3adb6cf7c3d7f8b070e5eb9942761666f8fa9d58`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053b0aba8a62b2d1ebadcd710799a63584f106e45cda4ac37ad86a107d7de70f`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 2.8 KB (2797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0` - unknown; unknown

```console
$ docker pull docker@sha256:0fb45f97b44a9fd07d91798156de1c8e5feee9ef91bbcb918dca2552283673b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.3 KB (733269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f05479573db10e995800169c17cc75dc7e02754a961730757f0ab0e57eefa3`

```dockerfile
```

-	Layers:
	-	`sha256:79ed0876afb43b9f34c2ad8abab3df2b215642df1353865e7f19b939f12992cd`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 702.9 KB (702936 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ff33b8332a65e8707424c58afd06e0da9b0c83886d7078e89615993510af5044`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 30.3 KB (30333 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c4f291842cc372be20d42c77bf29c3cc5f302989dfd0b6de574ca75a2a444087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109839965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b3167e27ccfb4dfa4fa0fcaa3fea4c2026e8d09cc3c209d3db8cb8b27224e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0` - unknown; unknown

```console
$ docker pull docker@sha256:9d66b06e4f1158baf427971f83571abe635d5bc5ef22d8cc4344f9c7b5e11fe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.1 KB (733077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625c5a6acfba0dd0de4524db7ddc2c0be3bb531c9febd06badb4e8bf179ba5c5`

```dockerfile
```

-	Layers:
	-	`sha256:53f6704407130f584a1f72df612b15e8dc8092b8dba809328e0a1f83ecd338d6`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 702.9 KB (702879 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3f75f2b4b1808936dcfc233ce3ac1d12741e81d0459cbf547be77385a4aee3dc`  
		Last Modified: Thu, 19 Oct 2023 08:39:22 GMT  
		Size: 30.2 KB (30198 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0-cli`

```console
$ docker pull docker@sha256:4865ba3135696b1c0e1b6bf323a5ef9402013244a69280543cf16aebc1da2b49
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0-cli` - linux; amd64

```console
$ docker pull docker@sha256:789420937a26ebec564c47161164faf74d9de353539273ae7904229a5f3e5b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57099399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b67d930a0cca6847a99b95b85b36a9ac12cee20a21287127b14da64d1946bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-cli` - unknown; unknown

```console
$ docker pull docker@sha256:b5d5d8838c5713859922b1a19a03c004867d85b812ab5e92e1545f84b1234eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 KB (399302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02683e982681bcbf4a1a62ba5f77e9d89b24b9b0bb5fe8237ff69aaadfdb3a04`

```dockerfile
```

-	Layers:
	-	`sha256:14374abf45bae1e3e070c4baa97b47f1475d9a0a928e5bf3cc2f2ea739cb43da`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 363.5 KB (363519 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c6a63e5a737768c94345029588b7b2cbbd160667d93d710f706e40ed91413929`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 35.8 KB (35783 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-cli` - linux; arm variant v6

```console
$ docker pull docker@sha256:ff0fd928e653fa68ef74a55176e13ebb8dd2f8ac47b4f14248f056afe46a2171
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53615303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d70a15d2461e904100529d3d28e6f26d3bdc4ea9bd0ab8993082f5b83fa1d2b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-cli` - linux; arm variant v7

```console
$ docker pull docker@sha256:a26fe5863bb4158d8299df0e9133af0dc97ac7ed7537380d3990fa1e8f5e51bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53135663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b1d618bb96b56678094389031e7c08dce5ebe736b62ff92c7d71b8622c9221`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-cli` - unknown; unknown

```console
$ docker pull docker@sha256:efa475bd4aa53d695ee55df6c73d572d2be01e54e73a49674ed227b469da118d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 KB (399321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a054df93652b09d80b5c38006fbdceb1feaa8075f7428900cedf3a2b791667db`

```dockerfile
```

-	Layers:
	-	`sha256:39396a9f1f54b6de0baaee6a76517409540d0c9fdf05e89e7b24aafa80096638`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 363.6 KB (363561 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ffd4d5053927223f1562259738aeb32f076000d0b6c34f5982815d8e88e92bf1`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 35.8 KB (35760 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:55e2b2dfc3e8cac05521cc6a4f9c8aa97cf1290052cd1f54a45e17136b5aceaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52855252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fa15b6055e9eeaad38c87602b9548b90fda56c3bb21d21d9d03e564ca6f2764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-cli` - unknown; unknown

```console
$ docker pull docker@sha256:0d00e3c266fb4af54c0711d8c022d24ee55d46d9fa5b81fda8d4d33ce991d1c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.2 KB (399163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0095154483d0f23ec2378e28784fa23c02947429d9887390a48470bae96fdf9`

```dockerfile
```

-	Layers:
	-	`sha256:af0e147ec9339cbdc6caa4eef3cea829589eb0ddb71b39c8b80ae52514d3549d`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 363.5 KB (363534 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:279d55a79ed6483042d0e4381f1a5fd0c7d4778230aba7c78f42331aa6b5bb6d`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 35.6 KB (35629 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0-dind`

```console
$ docker pull docker@sha256:0752ca4e936da012c173c119217c0f9599b3b191c1557e53206d5d06d2627580
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:74e78208fc18da48ddf8b569abe21563730845c312130bd0f0b059746a7e10f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118536604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114405a05c1ea1579eada94100ea1262ec351ce96625fed47684ed05ef48f52f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-dind` - unknown; unknown

```console
$ docker pull docker@sha256:32bcc64f2342b9b4d239bc563b6136a3f2c8c4ec7c0b1b8a0159ea159131c66d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.0 KB (732982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742d72f2efb6cda226ca77f818decb8c96a54c83fd8a5ee45ebd0f4cb4432493`

```dockerfile
```

-	Layers:
	-	`sha256:dfb66480a0d5e8b3e0f100d57763a66e5f53dd59649388029d7395a9b9e22985`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 702.9 KB (702854 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0a6ef7e7265b4a34b64183232c7c53a3e9d151b070323f48ecc62433addde4f5`  
		Last Modified: Thu, 19 Oct 2023 03:15:28 GMT  
		Size: 30.1 KB (30128 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:3b9c201a958ca8287e09b71e46d225852effd86c080dbf9bf4bd8887c96bb393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111730242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378ee0fe8270d7a0b77b97ec7144132b710f93b2f605f4d58d7ed903ea921700`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c183f2f030545a92229eb1d957a3d27a632065fd3e889fc1821df61e705e8e`  
		Last Modified: Thu, 19 Oct 2023 04:44:13 GMT  
		Size: 7.2 MB (7173654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd6749d2a6490b564ea75608c30867d181bee08328b6d9261af8546e213744`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb92ac4eb0bdd3c74efcc1b6a7da46be2c315b825f313701621f05757da245`  
		Last Modified: Thu, 19 Oct 2023 04:44:20 GMT  
		Size: 50.9 MB (50936158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7db9246e2c193486442265643f2a84289eec2df6ada560c67809901314b47`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab1b151f3d0bcd981b77eecf172b682f3474cdc742f366600d378b119a5c9a`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 2.8 KB (2796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:d540c1e08caba133a46bf8d458253158143f00ad92da9a6b41e545da381639bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110546565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83f5a2ae6d81508dcfad2aa9837a2bd5b0fb43a928565a117e6f92a7f1b2052e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04261eaf858b9479a1d7176630c8bbd7196ea372d024b17b1e7354e0d24c16c2`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 6.5 MB (6469635 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34bf6d61289016c22a2a8fd3022160a5358e1ad2d6c72c7dc5cf382cddd15653`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7f6001c2b47951d06a099362aeb56a04176dfd1c1fc0ddc5c1bdb8c0a34474`  
		Last Modified: Thu, 19 Oct 2023 06:54:18 GMT  
		Size: 50.9 MB (50936137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4c99b97523144da18c38ab3adb6cf7c3d7f8b070e5eb9942761666f8fa9d58`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053b0aba8a62b2d1ebadcd710799a63584f106e45cda4ac37ad86a107d7de70f`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 2.8 KB (2797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-dind` - unknown; unknown

```console
$ docker pull docker@sha256:0fb45f97b44a9fd07d91798156de1c8e5feee9ef91bbcb918dca2552283673b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.3 KB (733269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f05479573db10e995800169c17cc75dc7e02754a961730757f0ab0e57eefa3`

```dockerfile
```

-	Layers:
	-	`sha256:79ed0876afb43b9f34c2ad8abab3df2b215642df1353865e7f19b939f12992cd`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 702.9 KB (702936 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ff33b8332a65e8707424c58afd06e0da9b0c83886d7078e89615993510af5044`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 30.3 KB (30333 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c4f291842cc372be20d42c77bf29c3cc5f302989dfd0b6de574ca75a2a444087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109839965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b3167e27ccfb4dfa4fa0fcaa3fea4c2026e8d09cc3c209d3db8cb8b27224e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-dind` - unknown; unknown

```console
$ docker pull docker@sha256:9d66b06e4f1158baf427971f83571abe635d5bc5ef22d8cc4344f9c7b5e11fe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.1 KB (733077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625c5a6acfba0dd0de4524db7ddc2c0be3bb531c9febd06badb4e8bf179ba5c5`

```dockerfile
```

-	Layers:
	-	`sha256:53f6704407130f584a1f72df612b15e8dc8092b8dba809328e0a1f83ecd338d6`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 702.9 KB (702879 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3f75f2b4b1808936dcfc233ce3ac1d12741e81d0459cbf547be77385a4aee3dc`  
		Last Modified: Thu, 19 Oct 2023 08:39:22 GMT  
		Size: 30.2 KB (30198 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0-dind-rootless`

```console
$ docker pull docker@sha256:71bee62410f63c1b313d3a6b14f4ed657b448ecacb69a8098deff9ae53010b19
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5e6bef9db0bb59ded0834ccf7953b7ff4fba228c0b62f40d0dd84cf6fb929f6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140560736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6a3d03b4335d3c77905757053aeb7d3b276a299ea360d049ca5319426071b2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
USER rootless
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51331694e511817c7af194b499671898dc666d5a1246478039ac7cbe4b8bb928`  
		Last Modified: Thu, 19 Oct 2023 04:06:27 GMT  
		Size: 1.4 MB (1362179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a05bb47bbc48d4359156ea4ad95b35ed79c5a16503b490d39fde39f5743dd580`  
		Last Modified: Thu, 19 Oct 2023 04:06:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6841788dd624e9c7343e25f901454d5e09cd3ad4b3c0f9418f66c503ac848711`  
		Last Modified: Thu, 19 Oct 2023 04:06:27 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:729437d46a9fe2fe36b282defe38f2a4f0f39bd398b9f47b8a9ac2d5a9f4987c`  
		Last Modified: Thu, 19 Oct 2023 04:06:29 GMT  
		Size: 20.7 MB (20660322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15ae4caf84a6e8590b6225b631a1bfcf10f417ce106af28c49f7eb72196effbe`  
		Last Modified: Thu, 19 Oct 2023 04:06:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:6c000e6ecf7be401312530c955dc48603d0a301b2450302fbf29aba6f5e21623
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **777.1 KB (777130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a26ec4c100e1cb1da7753bee45b48cebc2266ebf28d99d704b0735db7bcbed`

```dockerfile
```

-	Layers:
	-	`sha256:8e41c8d50b467c850c3ff7e4f049fd4a2ce5b3787fd13da5389e4759a8672bb4`  
		Last Modified: Thu, 19 Oct 2023 04:06:26 GMT  
		Size: 746.0 KB (746048 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9de2eee0dcd20e7a1709a88819367161618aea1ed5d944d63dd6427dc419368a`  
		Last Modified: Thu, 19 Oct 2023 04:06:26 GMT  
		Size: 31.1 KB (31082 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:42441ba25e32850da9df550a240c5583e37bf21de7190d1840dc2aeaa70fed6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133703554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2a5f3b9f1aeada90e298c000d285e31ea0b29c4397c4dfaccef88eceb389fe2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
USER rootless
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bca473d3d6cc9b124cd49408a18f60218bcd8cb366e56a3b16e18e934228b2e1`  
		Last Modified: Thu, 19 Oct 2023 09:04:35 GMT  
		Size: 1.4 MB (1413154 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b973c3488b8d0250e2ae2c52cb652304a7abab1644c18e1207d9a3822bd1d17`  
		Last Modified: Thu, 19 Oct 2023 09:04:35 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90f01a8ca69a1582ddbe39d495781d8b154de69989d89ae55e04dab61fb49ccf`  
		Last Modified: Thu, 19 Oct 2023 09:04:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:442dfac109ba1720ef139f23f3b17d5b7f196c11075a86a842966d816b0f36dc`  
		Last Modified: Thu, 19 Oct 2023 09:04:37 GMT  
		Size: 22.4 MB (22448806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6733ab06e49858ad2a4afb9b4f52aeb72694046b855fbec5a8728e4fa51ae8d9`  
		Last Modified: Thu, 19 Oct 2023 09:04:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:34bf7fdd92e10f28722d896db78e5cd89f9251a276dece636173aaeb4c16f65f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **777.2 KB (777203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85afdc700cb054338ac5d23874d67d86ef33460e2762b701dd5c006e0d7a3e`

```dockerfile
```

-	Layers:
	-	`sha256:5f3f7869dda1395b108e38a74799402ec328daa66f758066ebe5c399dddfcb98`  
		Last Modified: Thu, 19 Oct 2023 09:04:34 GMT  
		Size: 746.1 KB (746061 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8950340c6d28e1c91dd6419aa4a01f1690740ed770b0a9efce2e078381919c5d`  
		Last Modified: Thu, 19 Oct 2023 09:04:34 GMT  
		Size: 31.1 KB (31142 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:24.0-git`

```console
$ docker pull docker@sha256:cc2d2f4fca4d5c78508ee85db7af568a08f97559c2e20f69bb91e498b885dde2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24.0-git` - linux; amd64

```console
$ docker pull docker@sha256:00b5b6a006ff69369d3971b2055bb2da7000a8e9971005f36879dab92de4ef98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123479937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be7e484a4dfd5b5dd06b7c0ed89758b50908fe0db096183d8cfdadb98a0b9b4`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6466ad09233589febc284d1c1f41a4c39f0fa0a5b1aa1bea85891ddba7739539`  
		Last Modified: Thu, 19 Oct 2023 04:06:29 GMT  
		Size: 4.9 MB (4943333 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-git` - unknown; unknown

```console
$ docker pull docker@sha256:65ed97cbd3ef22714b0a305e8307d5f87083d7fbf5e6376676b5fa3c943802c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **761.5 KB (761546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1783abf6e7c52303433757998ff19429c08b9aaeb3ccac7040cd08561fd00567`

```dockerfile
```

-	Layers:
	-	`sha256:08aaa8df3b54134a7b381b45ace0ac59183c9c1ed7a0ee0ab1d7454b19f52e87`  
		Last Modified: Thu, 19 Oct 2023 04:06:28 GMT  
		Size: 748.6 KB (748627 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:68cbef04771d10485635bfb7269952da578567db38de22b31f69ff3230ed6002`  
		Last Modified: Thu, 19 Oct 2023 04:06:28 GMT  
		Size: 12.9 KB (12919 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:ec2b91d49b9ed4c997600e5cee4690bbf12f91fcc6f65820802224dcf0649102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116670835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2018e784dfa20e080841e3eebef1a00d61c9ee949b235eebd7d112f933e43aae`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c183f2f030545a92229eb1d957a3d27a632065fd3e889fc1821df61e705e8e`  
		Last Modified: Thu, 19 Oct 2023 04:44:13 GMT  
		Size: 7.2 MB (7173654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd6749d2a6490b564ea75608c30867d181bee08328b6d9261af8546e213744`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb92ac4eb0bdd3c74efcc1b6a7da46be2c315b825f313701621f05757da245`  
		Last Modified: Thu, 19 Oct 2023 04:44:20 GMT  
		Size: 50.9 MB (50936158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7db9246e2c193486442265643f2a84289eec2df6ada560c67809901314b47`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab1b151f3d0bcd981b77eecf172b682f3474cdc742f366600d378b119a5c9a`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 2.8 KB (2796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cee337b7b489249be7352c134317ce799195091ca6ad9932e7dbb524056e694`  
		Last Modified: Thu, 19 Oct 2023 05:42:21 GMT  
		Size: 4.9 MB (4940593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:3f88c8c70b39ae8f9461ffc542ef86a2fabfdf9ca41f98409d3794bee3100983
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115038908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9eadcbcc6c8f6ff1f8fd987d415935906d56012fe5073c65f8b6f39c0bc851`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04261eaf858b9479a1d7176630c8bbd7196ea372d024b17b1e7354e0d24c16c2`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 6.5 MB (6469635 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34bf6d61289016c22a2a8fd3022160a5358e1ad2d6c72c7dc5cf382cddd15653`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7f6001c2b47951d06a099362aeb56a04176dfd1c1fc0ddc5c1bdb8c0a34474`  
		Last Modified: Thu, 19 Oct 2023 06:54:18 GMT  
		Size: 50.9 MB (50936137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4c99b97523144da18c38ab3adb6cf7c3d7f8b070e5eb9942761666f8fa9d58`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053b0aba8a62b2d1ebadcd710799a63584f106e45cda4ac37ad86a107d7de70f`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 2.8 KB (2797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:faf69bf10977965d99584c9aa00ac2e56fcb290a76eb1b7ba85c0cb17bff1da7`  
		Last Modified: Thu, 19 Oct 2023 07:11:28 GMT  
		Size: 4.5 MB (4492343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-git` - unknown; unknown

```console
$ docker pull docker@sha256:4f879efbd2090c1d2b2cb5380894406c986d9c23d7bf5afab6239796a7a3d66e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.1 KB (764149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d8750ed6e0566af35a64780d09daa5f9efdce8d111bac971ca704db5f52266`

```dockerfile
```

-	Layers:
	-	`sha256:1a0bff8d09f12570e3bdeb2706176068cddb197ab88e9ab2a2c7e7d6420232f0`  
		Last Modified: Thu, 19 Oct 2023 07:11:27 GMT  
		Size: 751.1 KB (751136 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:449e4f641245d33dbfe27dc3896f900ff0e773d282d806a6bdcfc8889b87cd69`  
		Last Modified: Thu, 19 Oct 2023 07:11:26 GMT  
		Size: 13.0 KB (13013 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:56fe9ab697bcb19fac6ddaba066c07156501ee39bb6f3de0098f4e11c834f46a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114877213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba700d423fdbd813634e9f5cd0fe826bf010bb037fe94cd422bef6a228399591`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6fdb8b91a9d574fac2adf6328b5d9d9ca0a3cc3220b38be475464889bb4aabf1`  
		Last Modified: Thu, 19 Oct 2023 09:04:59 GMT  
		Size: 5.0 MB (5037248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24.0-git` - unknown; unknown

```console
$ docker pull docker@sha256:ce3b404e88dabff4445d39b8023e27dbcce575a4557bf486040f25fc0ef2f321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.4 KB (759394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36ec390ccae563be564a2d7970e81cff0ac8913eb61995d0e9afc1794357edee`

```dockerfile
```

-	Layers:
	-	`sha256:3d8c86ce8c5a9620cd072924c764aca54ca673f50ef4b56c47d3d137705c9e6c`  
		Last Modified: Thu, 19 Oct 2023 09:04:57 GMT  
		Size: 748.6 KB (748640 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9176acf5c3f61dc56fed8244db8793faf53232b5ddb1160aaa2478c9fb8ce95d`  
		Last Modified: Thu, 19 Oct 2023 09:04:57 GMT  
		Size: 10.8 KB (10754 bytes)  
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

## `docker:24.0.7`

**does not exist** (yet?)

## `docker:24.0.7-alpine3.18`

**does not exist** (yet?)

## `docker:24.0.7-cli`

**does not exist** (yet?)

## `docker:24.0.7-cli-alpine3.18`

**does not exist** (yet?)

## `docker:24.0.7-dind`

**does not exist** (yet?)

## `docker:24.0.7-dind-alpine3.18`

**does not exist** (yet?)

## `docker:24.0.7-dind-rootless`

**does not exist** (yet?)

## `docker:24.0.7-git`

**does not exist** (yet?)

## `docker:24.0.7-windowsservercore`

**does not exist** (yet?)

## `docker:24.0.7-windowsservercore-1809`

**does not exist** (yet?)

## `docker:24.0.7-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `docker:cli`

```console
$ docker pull docker@sha256:4865ba3135696b1c0e1b6bf323a5ef9402013244a69280543cf16aebc1da2b49
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:789420937a26ebec564c47161164faf74d9de353539273ae7904229a5f3e5b54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57099399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b67d930a0cca6847a99b95b85b36a9ac12cee20a21287127b14da64d1946bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:b5d5d8838c5713859922b1a19a03c004867d85b812ab5e92e1545f84b1234eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 KB (399302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02683e982681bcbf4a1a62ba5f77e9d89b24b9b0bb5fe8237ff69aaadfdb3a04`

```dockerfile
```

-	Layers:
	-	`sha256:14374abf45bae1e3e070c4baa97b47f1475d9a0a928e5bf3cc2f2ea739cb43da`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 363.5 KB (363519 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c6a63e5a737768c94345029588b7b2cbbd160667d93d710f706e40ed91413929`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 35.8 KB (35783 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:cli` - linux; arm variant v6

```console
$ docker pull docker@sha256:ff0fd928e653fa68ef74a55176e13ebb8dd2f8ac47b4f14248f056afe46a2171
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53615303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d70a15d2461e904100529d3d28e6f26d3bdc4ea9bd0ab8993082f5b83fa1d2b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:cli` - linux; arm variant v7

```console
$ docker pull docker@sha256:a26fe5863bb4158d8299df0e9133af0dc97ac7ed7537380d3990fa1e8f5e51bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53135663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9b1d618bb96b56678094389031e7c08dce5ebe736b62ff92c7d71b8622c9221`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:efa475bd4aa53d695ee55df6c73d572d2be01e54e73a49674ed227b469da118d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 KB (399321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a054df93652b09d80b5c38006fbdceb1feaa8075f7428900cedf3a2b791667db`

```dockerfile
```

-	Layers:
	-	`sha256:39396a9f1f54b6de0baaee6a76517409540d0c9fdf05e89e7b24aafa80096638`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 363.6 KB (363561 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ffd4d5053927223f1562259738aeb32f076000d0b6c34f5982815d8e88e92bf1`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 35.8 KB (35760 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:55e2b2dfc3e8cac05521cc6a4f9c8aa97cf1290052cd1f54a45e17136b5aceaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52855252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fa15b6055e9eeaad38c87602b9548b90fda56c3bb21d21d9d03e564ca6f2764`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_VERSION=24.0.6
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Wed, 18 Oct 2023 17:04:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 18 Oct 2023 17:04:26 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 18 Oct 2023 17:04:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 17:04:26 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:0d00e3c266fb4af54c0711d8c022d24ee55d46d9fa5b81fda8d4d33ce991d1c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.2 KB (399163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0095154483d0f23ec2378e28784fa23c02947429d9887390a48470bae96fdf9`

```dockerfile
```

-	Layers:
	-	`sha256:af0e147ec9339cbdc6caa4eef3cea829589eb0ddb71b39c8b80ae52514d3549d`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 363.5 KB (363534 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:279d55a79ed6483042d0e4381f1a5fd0c7d4778230aba7c78f42331aa6b5bb6d`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 35.6 KB (35629 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:dind`

```console
$ docker pull docker@sha256:0752ca4e936da012c173c119217c0f9599b3b191c1557e53206d5d06d2627580
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:74e78208fc18da48ddf8b569abe21563730845c312130bd0f0b059746a7e10f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118536604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114405a05c1ea1579eada94100ea1262ec351ce96625fed47684ed05ef48f52f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:32bcc64f2342b9b4d239bc563b6136a3f2c8c4ec7c0b1b8a0159ea159131c66d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.0 KB (732982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742d72f2efb6cda226ca77f818decb8c96a54c83fd8a5ee45ebd0f4cb4432493`

```dockerfile
```

-	Layers:
	-	`sha256:dfb66480a0d5e8b3e0f100d57763a66e5f53dd59649388029d7395a9b9e22985`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 702.9 KB (702854 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0a6ef7e7265b4a34b64183232c7c53a3e9d151b070323f48ecc62433addde4f5`  
		Last Modified: Thu, 19 Oct 2023 03:15:28 GMT  
		Size: 30.1 KB (30128 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:3b9c201a958ca8287e09b71e46d225852effd86c080dbf9bf4bd8887c96bb393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111730242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378ee0fe8270d7a0b77b97ec7144132b710f93b2f605f4d58d7ed903ea921700`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c183f2f030545a92229eb1d957a3d27a632065fd3e889fc1821df61e705e8e`  
		Last Modified: Thu, 19 Oct 2023 04:44:13 GMT  
		Size: 7.2 MB (7173654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd6749d2a6490b564ea75608c30867d181bee08328b6d9261af8546e213744`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb92ac4eb0bdd3c74efcc1b6a7da46be2c315b825f313701621f05757da245`  
		Last Modified: Thu, 19 Oct 2023 04:44:20 GMT  
		Size: 50.9 MB (50936158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7db9246e2c193486442265643f2a84289eec2df6ada560c67809901314b47`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab1b151f3d0bcd981b77eecf172b682f3474cdc742f366600d378b119a5c9a`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 2.8 KB (2796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:d540c1e08caba133a46bf8d458253158143f00ad92da9a6b41e545da381639bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110546565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83f5a2ae6d81508dcfad2aa9837a2bd5b0fb43a928565a117e6f92a7f1b2052e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04261eaf858b9479a1d7176630c8bbd7196ea372d024b17b1e7354e0d24c16c2`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 6.5 MB (6469635 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34bf6d61289016c22a2a8fd3022160a5358e1ad2d6c72c7dc5cf382cddd15653`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7f6001c2b47951d06a099362aeb56a04176dfd1c1fc0ddc5c1bdb8c0a34474`  
		Last Modified: Thu, 19 Oct 2023 06:54:18 GMT  
		Size: 50.9 MB (50936137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4c99b97523144da18c38ab3adb6cf7c3d7f8b070e5eb9942761666f8fa9d58`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053b0aba8a62b2d1ebadcd710799a63584f106e45cda4ac37ad86a107d7de70f`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 2.8 KB (2797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:0fb45f97b44a9fd07d91798156de1c8e5feee9ef91bbcb918dca2552283673b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.3 KB (733269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f05479573db10e995800169c17cc75dc7e02754a961730757f0ab0e57eefa3`

```dockerfile
```

-	Layers:
	-	`sha256:79ed0876afb43b9f34c2ad8abab3df2b215642df1353865e7f19b939f12992cd`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 702.9 KB (702936 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ff33b8332a65e8707424c58afd06e0da9b0c83886d7078e89615993510af5044`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 30.3 KB (30333 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c4f291842cc372be20d42c77bf29c3cc5f302989dfd0b6de574ca75a2a444087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109839965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b3167e27ccfb4dfa4fa0fcaa3fea4c2026e8d09cc3c209d3db8cb8b27224e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:9d66b06e4f1158baf427971f83571abe635d5bc5ef22d8cc4344f9c7b5e11fe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.1 KB (733077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625c5a6acfba0dd0de4524db7ddc2c0be3bb531c9febd06badb4e8bf179ba5c5`

```dockerfile
```

-	Layers:
	-	`sha256:53f6704407130f584a1f72df612b15e8dc8092b8dba809328e0a1f83ecd338d6`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 702.9 KB (702879 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3f75f2b4b1808936dcfc233ce3ac1d12741e81d0459cbf547be77385a4aee3dc`  
		Last Modified: Thu, 19 Oct 2023 08:39:22 GMT  
		Size: 30.2 KB (30198 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:71bee62410f63c1b313d3a6b14f4ed657b448ecacb69a8098deff9ae53010b19
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5e6bef9db0bb59ded0834ccf7953b7ff4fba228c0b62f40d0dd84cf6fb929f6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140560736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6a3d03b4335d3c77905757053aeb7d3b276a299ea360d049ca5319426071b2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
USER rootless
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51331694e511817c7af194b499671898dc666d5a1246478039ac7cbe4b8bb928`  
		Last Modified: Thu, 19 Oct 2023 04:06:27 GMT  
		Size: 1.4 MB (1362179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a05bb47bbc48d4359156ea4ad95b35ed79c5a16503b490d39fde39f5743dd580`  
		Last Modified: Thu, 19 Oct 2023 04:06:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6841788dd624e9c7343e25f901454d5e09cd3ad4b3c0f9418f66c503ac848711`  
		Last Modified: Thu, 19 Oct 2023 04:06:27 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:729437d46a9fe2fe36b282defe38f2a4f0f39bd398b9f47b8a9ac2d5a9f4987c`  
		Last Modified: Thu, 19 Oct 2023 04:06:29 GMT  
		Size: 20.7 MB (20660322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15ae4caf84a6e8590b6225b631a1bfcf10f417ce106af28c49f7eb72196effbe`  
		Last Modified: Thu, 19 Oct 2023 04:06:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:6c000e6ecf7be401312530c955dc48603d0a301b2450302fbf29aba6f5e21623
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **777.1 KB (777130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a26ec4c100e1cb1da7753bee45b48cebc2266ebf28d99d704b0735db7bcbed`

```dockerfile
```

-	Layers:
	-	`sha256:8e41c8d50b467c850c3ff7e4f049fd4a2ce5b3787fd13da5389e4759a8672bb4`  
		Last Modified: Thu, 19 Oct 2023 04:06:26 GMT  
		Size: 746.0 KB (746048 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9de2eee0dcd20e7a1709a88819367161618aea1ed5d944d63dd6427dc419368a`  
		Last Modified: Thu, 19 Oct 2023 04:06:26 GMT  
		Size: 31.1 KB (31082 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:42441ba25e32850da9df550a240c5583e37bf21de7190d1840dc2aeaa70fed6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133703554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2a5f3b9f1aeada90e298c000d285e31ea0b29c4397c4dfaccef88eceb389fe2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
USER rootless
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bca473d3d6cc9b124cd49408a18f60218bcd8cb366e56a3b16e18e934228b2e1`  
		Last Modified: Thu, 19 Oct 2023 09:04:35 GMT  
		Size: 1.4 MB (1413154 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b973c3488b8d0250e2ae2c52cb652304a7abab1644c18e1207d9a3822bd1d17`  
		Last Modified: Thu, 19 Oct 2023 09:04:35 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90f01a8ca69a1582ddbe39d495781d8b154de69989d89ae55e04dab61fb49ccf`  
		Last Modified: Thu, 19 Oct 2023 09:04:35 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:442dfac109ba1720ef139f23f3b17d5b7f196c11075a86a842966d816b0f36dc`  
		Last Modified: Thu, 19 Oct 2023 09:04:37 GMT  
		Size: 22.4 MB (22448806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6733ab06e49858ad2a4afb9b4f52aeb72694046b855fbec5a8728e4fa51ae8d9`  
		Last Modified: Thu, 19 Oct 2023 09:04:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:34bf7fdd92e10f28722d896db78e5cd89f9251a276dece636173aaeb4c16f65f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **777.2 KB (777203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85afdc700cb054338ac5d23874d67d86ef33460e2762b701dd5c006e0d7a3e`

```dockerfile
```

-	Layers:
	-	`sha256:5f3f7869dda1395b108e38a74799402ec328daa66f758066ebe5c399dddfcb98`  
		Last Modified: Thu, 19 Oct 2023 09:04:34 GMT  
		Size: 746.1 KB (746061 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8950340c6d28e1c91dd6419aa4a01f1690740ed770b0a9efce2e078381919c5d`  
		Last Modified: Thu, 19 Oct 2023 09:04:34 GMT  
		Size: 31.1 KB (31142 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:git`

```console
$ docker pull docker@sha256:cc2d2f4fca4d5c78508ee85db7af568a08f97559c2e20f69bb91e498b885dde2
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:00b5b6a006ff69369d3971b2055bb2da7000a8e9971005f36879dab92de4ef98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123479937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be7e484a4dfd5b5dd06b7c0ed89758b50908fe0db096183d8cfdadb98a0b9b4`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6466ad09233589febc284d1c1f41a4c39f0fa0a5b1aa1bea85891ddba7739539`  
		Last Modified: Thu, 19 Oct 2023 04:06:29 GMT  
		Size: 4.9 MB (4943333 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:git` - unknown; unknown

```console
$ docker pull docker@sha256:65ed97cbd3ef22714b0a305e8307d5f87083d7fbf5e6376676b5fa3c943802c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **761.5 KB (761546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1783abf6e7c52303433757998ff19429c08b9aaeb3ccac7040cd08561fd00567`

```dockerfile
```

-	Layers:
	-	`sha256:08aaa8df3b54134a7b381b45ace0ac59183c9c1ed7a0ee0ab1d7454b19f52e87`  
		Last Modified: Thu, 19 Oct 2023 04:06:28 GMT  
		Size: 748.6 KB (748627 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:68cbef04771d10485635bfb7269952da578567db38de22b31f69ff3230ed6002`  
		Last Modified: Thu, 19 Oct 2023 04:06:28 GMT  
		Size: 12.9 KB (12919 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:git` - linux; arm variant v6

```console
$ docker pull docker@sha256:ec2b91d49b9ed4c997600e5cee4690bbf12f91fcc6f65820802224dcf0649102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.7 MB (116670835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2018e784dfa20e080841e3eebef1a00d61c9ee949b235eebd7d112f933e43aae`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c183f2f030545a92229eb1d957a3d27a632065fd3e889fc1821df61e705e8e`  
		Last Modified: Thu, 19 Oct 2023 04:44:13 GMT  
		Size: 7.2 MB (7173654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd6749d2a6490b564ea75608c30867d181bee08328b6d9261af8546e213744`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb92ac4eb0bdd3c74efcc1b6a7da46be2c315b825f313701621f05757da245`  
		Last Modified: Thu, 19 Oct 2023 04:44:20 GMT  
		Size: 50.9 MB (50936158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7db9246e2c193486442265643f2a84289eec2df6ada560c67809901314b47`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab1b151f3d0bcd981b77eecf172b682f3474cdc742f366600d378b119a5c9a`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 2.8 KB (2796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cee337b7b489249be7352c134317ce799195091ca6ad9932e7dbb524056e694`  
		Last Modified: Thu, 19 Oct 2023 05:42:21 GMT  
		Size: 4.9 MB (4940593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm variant v7

```console
$ docker pull docker@sha256:3f88c8c70b39ae8f9461ffc542ef86a2fabfdf9ca41f98409d3794bee3100983
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115038908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9eadcbcc6c8f6ff1f8fd987d415935906d56012fe5073c65f8b6f39c0bc851`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04261eaf858b9479a1d7176630c8bbd7196ea372d024b17b1e7354e0d24c16c2`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 6.5 MB (6469635 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34bf6d61289016c22a2a8fd3022160a5358e1ad2d6c72c7dc5cf382cddd15653`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7f6001c2b47951d06a099362aeb56a04176dfd1c1fc0ddc5c1bdb8c0a34474`  
		Last Modified: Thu, 19 Oct 2023 06:54:18 GMT  
		Size: 50.9 MB (50936137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4c99b97523144da18c38ab3adb6cf7c3d7f8b070e5eb9942761666f8fa9d58`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053b0aba8a62b2d1ebadcd710799a63584f106e45cda4ac37ad86a107d7de70f`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 2.8 KB (2797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:faf69bf10977965d99584c9aa00ac2e56fcb290a76eb1b7ba85c0cb17bff1da7`  
		Last Modified: Thu, 19 Oct 2023 07:11:28 GMT  
		Size: 4.5 MB (4492343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:git` - unknown; unknown

```console
$ docker pull docker@sha256:4f879efbd2090c1d2b2cb5380894406c986d9c23d7bf5afab6239796a7a3d66e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **764.1 KB (764149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d8750ed6e0566af35a64780d09daa5f9efdce8d111bac971ca704db5f52266`

```dockerfile
```

-	Layers:
	-	`sha256:1a0bff8d09f12570e3bdeb2706176068cddb197ab88e9ab2a2c7e7d6420232f0`  
		Last Modified: Thu, 19 Oct 2023 07:11:27 GMT  
		Size: 751.1 KB (751136 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:449e4f641245d33dbfe27dc3896f900ff0e773d282d806a6bdcfc8889b87cd69`  
		Last Modified: Thu, 19 Oct 2023 07:11:26 GMT  
		Size: 13.0 KB (13013 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:56fe9ab697bcb19fac6ddaba066c07156501ee39bb6f3de0098f4e11c834f46a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114877213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba700d423fdbd813634e9f5cd0fe826bf010bb037fe94cd422bef6a228399591`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6fdb8b91a9d574fac2adf6328b5d9d9ca0a3cc3220b38be475464889bb4aabf1`  
		Last Modified: Thu, 19 Oct 2023 09:04:59 GMT  
		Size: 5.0 MB (5037248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:git` - unknown; unknown

```console
$ docker pull docker@sha256:ce3b404e88dabff4445d39b8023e27dbcce575a4557bf486040f25fc0ef2f321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.4 KB (759394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36ec390ccae563be564a2d7970e81cff0ac8913eb61995d0e9afc1794357edee`

```dockerfile
```

-	Layers:
	-	`sha256:3d8c86ce8c5a9620cd072924c764aca54ca673f50ef4b56c47d3d137705c9e6c`  
		Last Modified: Thu, 19 Oct 2023 09:04:57 GMT  
		Size: 748.6 KB (748640 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9176acf5c3f61dc56fed8244db8793faf53232b5ddb1160aaa2478c9fb8ce95d`  
		Last Modified: Thu, 19 Oct 2023 09:04:57 GMT  
		Size: 10.8 KB (10754 bytes)  
		MIME: application/vnd.in-toto+json

## `docker:latest`

```console
$ docker pull docker@sha256:0752ca4e936da012c173c119217c0f9599b3b191c1557e53206d5d06d2627580
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:74e78208fc18da48ddf8b569abe21563730845c312130bd0f0b059746a7e10f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118536604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114405a05c1ea1579eada94100ea1262ec351ce96625fed47684ed05ef48f52f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:636b7876979dd74729cde61aeefc7910a214801d407d5963d4941a61073c17ef`  
		Last Modified: Thu, 19 Oct 2023 01:01:01 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130a3e1e7df5bfc5e27771be7f2de766c978218e4bcde12acc15bb5798bf8389`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60190b130ff22ce63568f555059cb9e2480152ef6e7b3c11ba9f5d8610b0f660`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ce2dbd107eb0b0d892de543863087d986daaf0a2be3d440495854639f1d66e6`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 17.8 MB (17831745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c711618a8d746c257235057f1c751090333eee8d354143f114c2031754f1f45d`  
		Last Modified: Thu, 19 Oct 2023 01:01:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1a9d1fa736bdc93edc03d9308b756d77872cf0e8c3fea6813b0f87e13786c03`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a915d3d782d1ec22c50998481b195e183013951efbafc92a5ca96c82f6263d0`  
		Last Modified: Thu, 19 Oct 2023 01:01:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63fa7f453749db5037378a1c0410def475af9f9c17388276ab96769d4fd1ab24`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 7.1 MB (7080495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce8f4a45972f0ac134ac627a1d206bb0c6f955b02f4fad3f85ec281fdc19bee7`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88060cc894f1bfa624656d65dacffafc1ca354ffec59ba24af907ff01b553b0`  
		Last Modified: Thu, 19 Oct 2023 03:15:32 GMT  
		Size: 54.4 MB (54351587 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09e0ea80a90a76f87fb4f59157ca1269489a9d1ea1754d85209adcffa2cf40fe`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6831f6f9e30f872cbb2439fd3d439c159f11ddda39928ef70e9e7de50b9e9a52`  
		Last Modified: Thu, 19 Oct 2023 03:15:30 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:latest` - unknown; unknown

```console
$ docker pull docker@sha256:32bcc64f2342b9b4d239bc563b6136a3f2c8c4ec7c0b1b8a0159ea159131c66d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.0 KB (732982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742d72f2efb6cda226ca77f818decb8c96a54c83fd8a5ee45ebd0f4cb4432493`

```dockerfile
```

-	Layers:
	-	`sha256:dfb66480a0d5e8b3e0f100d57763a66e5f53dd59649388029d7395a9b9e22985`  
		Last Modified: Thu, 19 Oct 2023 03:15:29 GMT  
		Size: 702.9 KB (702854 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0a6ef7e7265b4a34b64183232c7c53a3e9d151b070323f48ecc62433addde4f5`  
		Last Modified: Thu, 19 Oct 2023 03:15:28 GMT  
		Size: 30.1 KB (30128 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:latest` - linux; arm variant v6

```console
$ docker pull docker@sha256:3b9c201a958ca8287e09b71e46d225852effd86c080dbf9bf4bd8887c96bb393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111730242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378ee0fe8270d7a0b77b97ec7144132b710f93b2f605f4d58d7ed903ea921700`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39949916592345dc6f4df09edd04962a26adc0fedad76569033b48d0722a31`  
		Last Modified: Thu, 19 Oct 2023 04:06:43 GMT  
		Size: 16.9 MB (16854332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ea0a4cf594236dc335a040215f2662ac65c7c43dcfb7e81b2932f1c7d4830f`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499941cc4ad12a961a9f2491706f252f61f9d975f4712c7d096c75a05d274eac`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a440851f80c17571d08a99769e72446aeb133f14f2fc1dd5df4c7a4dc18918`  
		Last Modified: Thu, 19 Oct 2023 04:06:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c183f2f030545a92229eb1d957a3d27a632065fd3e889fc1821df61e705e8e`  
		Last Modified: Thu, 19 Oct 2023 04:44:13 GMT  
		Size: 7.2 MB (7173654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd6749d2a6490b564ea75608c30867d181bee08328b6d9261af8546e213744`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fb92ac4eb0bdd3c74efcc1b6a7da46be2c315b825f313701621f05757da245`  
		Last Modified: Thu, 19 Oct 2023 04:44:20 GMT  
		Size: 50.9 MB (50936158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a7db9246e2c193486442265643f2a84289eec2df6ada560c67809901314b47`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab1b151f3d0bcd981b77eecf172b682f3474cdc742f366600d378b119a5c9a`  
		Last Modified: Thu, 19 Oct 2023 04:44:12 GMT  
		Size: 2.8 KB (2796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm variant v7

```console
$ docker pull docker@sha256:d540c1e08caba133a46bf8d458253158143f00ad92da9a6b41e545da381639bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110546565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83f5a2ae6d81508dcfad2aa9837a2bd5b0fb43a928565a117e6f92a7f1b2052e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ccdd5fc72dda082141bb20af739dc9e0b17caac2d22ca60c7688734ef4782`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 15.1 MB (15118479 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b08f84408a6fc85a923ed90fb093d2eb0d0a510336ad1d6660c54a8a307cf1c`  
		Last Modified: Tue, 03 Oct 2023 00:57:57 GMT  
		Size: 16.4 MB (16400146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea87bdf863709fa91c407a89afe8223bae213163b970ffa2b13f00804f73588d`  
		Last Modified: Thu, 19 Oct 2023 05:55:12 GMT  
		Size: 16.8 MB (16840167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e4a6e3f14d925303103d5df3ada3f2b2d4e97d9d7c768dbf79c47ebfd955e6f`  
		Last Modified: Thu, 19 Oct 2023 05:55:10 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89576f09aece6290f15ec6d0f65de9ae99cbac48abd1383185ac46a690d65a42`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:396aa67c1453d024e3d8c94aae93de361565da8220966bc82c3be3472e7486d8`  
		Last Modified: Thu, 19 Oct 2023 05:55:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04261eaf858b9479a1d7176630c8bbd7196ea372d024b17b1e7354e0d24c16c2`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 6.5 MB (6469635 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34bf6d61289016c22a2a8fd3022160a5358e1ad2d6c72c7dc5cf382cddd15653`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7f6001c2b47951d06a099362aeb56a04176dfd1c1fc0ddc5c1bdb8c0a34474`  
		Last Modified: Thu, 19 Oct 2023 06:54:18 GMT  
		Size: 50.9 MB (50936137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb4c99b97523144da18c38ab3adb6cf7c3d7f8b070e5eb9942761666f8fa9d58`  
		Last Modified: Thu, 19 Oct 2023 06:54:14 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053b0aba8a62b2d1ebadcd710799a63584f106e45cda4ac37ad86a107d7de70f`  
		Last Modified: Thu, 19 Oct 2023 06:54:15 GMT  
		Size: 2.8 KB (2797 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:latest` - unknown; unknown

```console
$ docker pull docker@sha256:0fb45f97b44a9fd07d91798156de1c8e5feee9ef91bbcb918dca2552283673b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.3 KB (733269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45f05479573db10e995800169c17cc75dc7e02754a961730757f0ab0e57eefa3`

```dockerfile
```

-	Layers:
	-	`sha256:79ed0876afb43b9f34c2ad8abab3df2b215642df1353865e7f19b939f12992cd`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 702.9 KB (702936 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ff33b8332a65e8707424c58afd06e0da9b0c83886d7078e89615993510af5044`  
		Last Modified: Thu, 19 Oct 2023 06:54:13 GMT  
		Size: 30.3 KB (30333 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c4f291842cc372be20d42c77bf29c3cc5f302989dfd0b6de574ca75a2a444087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109839965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39b3167e27ccfb4dfa4fa0fcaa3fea4c2026e8d09cc3c209d3db8cb8b27224e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
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
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
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
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df61191e4203819ca143d9ddd941a5130452c32c2bc514644f1791119a3570b1`  
		Last Modified: Thu, 19 Oct 2023 03:14:30 GMT  
		Size: 16.3 MB (16290382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:896e3ce9c2771af693c67bd4f5583b672a3f4d5db71c99447c4e6fa4700d1073`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fdedfe04474cf5b527a9af92a0a6c5bbe45194175b856d1bdceea5b72e0da24`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf03d5960a18af5c810d08d92f517633c4c570b46f936317675110efdce962cb`  
		Last Modified: Thu, 19 Oct 2023 03:14:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c08bbdc8fb7a00d04e813bbd37b05c83fd8fe09a9899f98ace063522fb15727`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 7.3 MB (7291334 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f799874081b87c1008fb6ddada38d54110c3816fe6857dc2b31a1e797c715a1`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95141bf3c415b848a1e2019d05e32b2814903d39516fae7bae08eee16fb163c3`  
		Last Modified: Thu, 19 Oct 2023 08:39:27 GMT  
		Size: 49.7 MB (49688248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d462e62db60bd9a7740ff62b858a0fa684081ba6a6a30e403feadc1863f53a8`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c9928a90e57817b0f8dbde4ff9e5bcb105d9a7ed244ef1e185fa774c29a4be`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 2.8 KB (2799 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:latest` - unknown; unknown

```console
$ docker pull docker@sha256:9d66b06e4f1158baf427971f83571abe635d5bc5ef22d8cc4344f9c7b5e11fe0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **733.1 KB (733077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625c5a6acfba0dd0de4524db7ddc2c0be3bb531c9febd06badb4e8bf179ba5c5`

```dockerfile
```

-	Layers:
	-	`sha256:53f6704407130f584a1f72df612b15e8dc8092b8dba809328e0a1f83ecd338d6`  
		Last Modified: Thu, 19 Oct 2023 08:39:23 GMT  
		Size: 702.9 KB (702879 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3f75f2b4b1808936dcfc233ce3ac1d12741e81d0459cbf547be77385a4aee3dc`  
		Last Modified: Thu, 19 Oct 2023 08:39:22 GMT  
		Size: 30.2 KB (30198 bytes)  
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
