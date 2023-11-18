## `docker:rc-git`

```console
$ docker pull docker@sha256:edf2035b650a9444949c47362a9fb1905c0655b6da7e7d2b80f7e90ada915171
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

### `docker:rc-git` - linux; amd64

```console
$ docker pull docker@sha256:ae55b8b6e50de0f9f0e4feea6a52a79c2e24b7205413ad178d3f0085ab603dc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127303876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d83e63c974564a3c5d8379d27b2880a4476edad1b9c7697b204107a407fd07f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-x86_64'; 			sha256='4f9b5313cf3eb1651b65aa6fc2fe1f59eb3812b7566f7c1b853be429b81bf3ab'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv6'; 			sha256='44b679381da55d1a673e5e638ac6d34f81e38e58ac656c530e27bb57a0ef930d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv7'; 			sha256='347b65d0cec622976bb753550d2708c8c9c760d55c1b5952a6800f5fadd4781c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-aarch64'; 			sha256='27b3cb1f066cdba191c4df96255a3d7178294763c9d67fba528f769968fc2e65'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-ppc64le'; 			sha256='76981fe4b032385752c5bb07144a22a7dfb599da15eca6fa1775e94364833475'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-riscv64'; 			sha256='1ee27dd153bd796686ece5d1829266b9b0db0a2ed67e7dbef023457da6dc5761'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-s390x'; 			sha256='9ee5fd812e7e52c08b95cd59673b956f2248343c2fb51eb8bcf635b02cfcbee4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0258f65a9be730ba25bb29824c8276fa1140a025ff26e89c96111785a3500986`  
		Last Modified: Fri, 17 Nov 2023 19:18:10 GMT  
		Size: 2.0 MB (2014288 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2100942ac8ed2802129da368484acd2c6219727e277e20f60a363029e865ef7e`  
		Last Modified: Fri, 17 Nov 2023 19:18:11 GMT  
		Size: 16.9 MB (16890676 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f3d6cd62916f773f9003515a52be6bcfde9f6c4039a9b5be450d513f6af16a8e`  
		Last Modified: Fri, 17 Nov 2023 19:18:11 GMT  
		Size: 17.2 MB (17195297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2617920b1bfffb2c050e1dc51a4abe663ea56b914f121cf994e5d448d0babeac`  
		Last Modified: Fri, 17 Nov 2023 19:18:11 GMT  
		Size: 17.8 MB (17812795 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34c447b70df81714802438f6014eff40042a8700dadd4f869d4a6396f98ddd0a`  
		Last Modified: Fri, 17 Nov 2023 19:18:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4dc88890e7a54c383c10a72a0a156ce38e012348a2f1ee7820d910c090eccc4c`  
		Last Modified: Fri, 17 Nov 2023 19:18:12 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5af4f2928e91ff893ed1146889ef980f8e1b2fc966541936ff69521ee8ee7a14`  
		Last Modified: Fri, 17 Nov 2023 19:18:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f5adcc57f9eb55501c6720ac21790443420cc2beffd81bbd155ca86c7cc5f954`  
		Last Modified: Fri, 17 Nov 2023 20:16:45 GMT  
		Size: 9.3 MB (9274473 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f10adfb53ce039554bbe3868e327fd9fa964e4965be6c00f5421b01f6321c282`  
		Last Modified: Fri, 17 Nov 2023 20:16:45 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fc1e21ab60304ddead41eb5bb45f28fb8c565d01f54557250136acd8a9c3056`  
		Last Modified: Fri, 17 Nov 2023 20:16:46 GMT  
		Size: 55.8 MB (55764197 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fbe6f47489a8797b5d415582a180d98478411ffd593c05b5bdf2bd397f60929b`  
		Last Modified: Fri, 17 Nov 2023 20:16:45 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a57a8397e7ba23aeaeba5265d0c2625ffae56864f39e9238cc9184308fcc3d5f`  
		Last Modified: Fri, 17 Nov 2023 20:16:46 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:707d1727b8ef05aa82dc205e9eda6e990d790bc18d95c8281725e62d12c08798`  
		Last Modified: Fri, 17 Nov 2023 21:19:33 GMT  
		Size: 4.9 MB (4943354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-git` - unknown; unknown

```console
$ docker pull docker@sha256:a2bf71f5399a903347d45684e24ba4272c4c95155b6862ac8256f7d2ce062c68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **731.5 KB (731465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6dec26950f2d4245d8e1fc97992c2fdc5b00eb24c54459f41e2fd1047efe0d9`

```dockerfile
```

-	Layers:
	-	`sha256:7dfc54ed0f05cb05e49101f9a9e1ac3b4dbb937b12dcfaf419a165c60256ae06`  
		Last Modified: Fri, 17 Nov 2023 21:19:32 GMT  
		Size: 718.8 KB (718802 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:919dca3e1a1200908b710fc86c8fb0af847fbe615ac5f16fb6634f33471f6f5c`  
		Last Modified: Fri, 17 Nov 2023 21:19:32 GMT  
		Size: 12.7 KB (12663 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:rc-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:408c6f2e353725da6991bfca90ad164e1210abb0bba01c741c0c68d1dc9c29e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119552731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06d4d86a24ca2af2d49f2d087f450cb531cf0f6601c7392570d706dde3bf7a3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-x86_64'; 			sha256='4f9b5313cf3eb1651b65aa6fc2fe1f59eb3812b7566f7c1b853be429b81bf3ab'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv6'; 			sha256='44b679381da55d1a673e5e638ac6d34f81e38e58ac656c530e27bb57a0ef930d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv7'; 			sha256='347b65d0cec622976bb753550d2708c8c9c760d55c1b5952a6800f5fadd4781c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-aarch64'; 			sha256='27b3cb1f066cdba191c4df96255a3d7178294763c9d67fba528f769968fc2e65'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-ppc64le'; 			sha256='76981fe4b032385752c5bb07144a22a7dfb599da15eca6fa1775e94364833475'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-riscv64'; 			sha256='1ee27dd153bd796686ece5d1829266b9b0db0a2ed67e7dbef023457da6dc5761'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-s390x'; 			sha256='9ee5fd812e7e52c08b95cd59673b956f2248343c2fb51eb8bcf635b02cfcbee4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749ab9fb78d5310f50a86ca9fc51b51ccfc7c6fb8285aea647b6faa49409ecf2`  
		Last Modified: Tue, 14 Nov 2023 02:37:28 GMT  
		Size: 2.1 MB (2088618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d4f6ffcef8dee3f9bf83e3bdcc8907643c5e1f91d44d8396286b5b8e58a5e1`  
		Last Modified: Tue, 14 Nov 2023 02:37:29 GMT  
		Size: 15.3 MB (15274900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8471a598c6c33331ad7a5058de5738de5952be7f17280bc35a3e18402a588bb`  
		Last Modified: Fri, 17 Nov 2023 19:20:33 GMT  
		Size: 16.1 MB (16099979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fcf04c0bd45d2936c42c84ae370cd336e0121872dddd09ff17540378c0d7bb`  
		Last Modified: Fri, 17 Nov 2023 19:20:34 GMT  
		Size: 16.8 MB (16837132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fac3f91570782edd43faf3ef38e169bff58d34e458a93c176849ac7eb0d00b`  
		Last Modified: Fri, 17 Nov 2023 19:20:31 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ffc07d4b5df7d138c8ea6a9c2c1570fe924850f6f2d975f99751c0cb151b80`  
		Last Modified: Fri, 17 Nov 2023 19:20:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f76e4004739c22e5e5695df1c52a7c1c7fe60ae10d88ef736f7cfda89aa584b`  
		Last Modified: Fri, 17 Nov 2023 19:20:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc801876d2aadac4fc9fffc0184dc040f040cedbd40bb9a02827080481a7723`  
		Last Modified: Fri, 17 Nov 2023 20:19:47 GMT  
		Size: 9.0 MB (9046110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4facc0840b9ba9a832204059b5c2adca83f55b1687fc356fd8d8915ce520302`  
		Last Modified: Fri, 17 Nov 2023 20:19:46 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5fa627a5a3022d7b0396017ba9da9b8851ed8a7502dc290fbbe2e3d7ca51bf`  
		Last Modified: Fri, 17 Nov 2023 20:19:53 GMT  
		Size: 52.1 MB (52113269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b7b1196226b802a515a1976be8c1cd49f73773d02c81e9a31b98c5a6d99536`  
		Last Modified: Fri, 17 Nov 2023 20:19:45 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8864c214ac854b4779ec27cf7f652015315909c6803df29b15a14b029583b8c`  
		Last Modified: Fri, 17 Nov 2023 20:19:45 GMT  
		Size: 2.8 KB (2793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fe3072ce0014251e23995b0ad78e4db88659443f65ecb7777f4f3a9f59690a`  
		Last Modified: Fri, 17 Nov 2023 21:22:56 GMT  
		Size: 4.9 MB (4940599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:7c334783e28e850ea2f107bfe5d46d1bd53fda2bf17ce2b28ef75a014b0b7375
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117781783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3323b05fd9c62d1704c55c2517752734915f95c9b8a90e45894eb948b1ff50`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-x86_64'; 			sha256='4f9b5313cf3eb1651b65aa6fc2fe1f59eb3812b7566f7c1b853be429b81bf3ab'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv6'; 			sha256='44b679381da55d1a673e5e638ac6d34f81e38e58ac656c530e27bb57a0ef930d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv7'; 			sha256='347b65d0cec622976bb753550d2708c8c9c760d55c1b5952a6800f5fadd4781c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-aarch64'; 			sha256='27b3cb1f066cdba191c4df96255a3d7178294763c9d67fba528f769968fc2e65'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-ppc64le'; 			sha256='76981fe4b032385752c5bb07144a22a7dfb599da15eca6fa1775e94364833475'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-riscv64'; 			sha256='1ee27dd153bd796686ece5d1829266b9b0db0a2ed67e7dbef023457da6dc5761'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-s390x'; 			sha256='9ee5fd812e7e52c08b95cd59673b956f2248343c2fb51eb8bcf635b02cfcbee4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
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
	-	`sha256:e4d4284c771adbac8678f485d42c71da5e9465482941db8231f014420c8bd33c`  
		Last Modified: Tue, 14 Nov 2023 05:39:25 GMT  
		Size: 15.3 MB (15269601 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add0974f57e0de4e10c6786a80dc2ac3db50e68d39b46cadaad22aaf65ae911f`  
		Last Modified: Fri, 17 Nov 2023 19:26:29 GMT  
		Size: 16.1 MB (16084089 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b044aa75dd49ab71f7270a756233828338c30f7d9df4236123938c43489d214`  
		Last Modified: Fri, 17 Nov 2023 19:26:29 GMT  
		Size: 16.8 MB (16822969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5bc09fe79b608c29ee0dc537b9d2ebd8a93da2b7dc31ec0a60413b7571e4e4aa`  
		Last Modified: Fri, 17 Nov 2023 19:26:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:474fe5ec47ca6fa03e16012e6552a4369328135371ae2d450af8523fb01e0ed4`  
		Last Modified: Fri, 17 Nov 2023 19:26:28 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d0ca5f65458b233e38879e78b924d9b076b4a9d1f2649ca3d409335e83a84d2`  
		Last Modified: Fri, 17 Nov 2023 19:26:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf693400c72272b1b7fa4615d66ac6c90a5ad08f6b519a5ee51954ee0517676b`  
		Last Modified: Fri, 17 Nov 2023 20:25:48 GMT  
		Size: 8.2 MB (8217520 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ccefd875a4aceda207d13f108d8763e4a9c537f2d8fce8eefdf4d688978913e6`  
		Last Modified: Fri, 17 Nov 2023 20:25:47 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58f568a7bae6f4c771592fe57f3077baebc21acb04b1ac03fca4f5433c8cb281`  
		Last Modified: Fri, 17 Nov 2023 20:25:49 GMT  
		Size: 52.1 MB (52113254 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7c259ff1398a6e13e06e1c2e8fad8fa72ade1b62747249e50ec4ff4478b3ff0`  
		Last Modified: Fri, 17 Nov 2023 20:25:47 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c15bcc7ffa406534bccd739bb25ce32416b98578a2180b6410d795d6f45d70da`  
		Last Modified: Fri, 17 Nov 2023 20:25:48 GMT  
		Size: 2.8 KB (2793 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9914da9d34cc161c8ea37dfc4806e695ee2abed4228fb772a04511ea4fe42268`  
		Last Modified: Fri, 17 Nov 2023 21:28:47 GMT  
		Size: 4.5 MB (4492362 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-git` - unknown; unknown

```console
$ docker pull docker@sha256:17213d4619699d5991572d54ed0e666f6a56fcfc11a86c2d0273a6b0ebdf9dca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **734.1 KB (734053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19efee076d40515b148216c2c5fb3d33da9e4ed85c68ab2722a39a9d42c31570`

```dockerfile
```

-	Layers:
	-	`sha256:7655dacc053b50d3e62b34929616c9ee0de3196ce3f1ee534c0e1332e719c1fd`  
		Last Modified: Fri, 17 Nov 2023 21:28:46 GMT  
		Size: 721.3 KB (721306 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ce712a84f8446388a15f914d0653649d66aae98aa6edb3e41e360b280cb146b0`  
		Last Modified: Fri, 17 Nov 2023 21:28:46 GMT  
		Size: 12.7 KB (12747 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8d112ab60cf7f7b596c0b774f9ddd58c75b61bb92dc76204c23c04834a29d03d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118956044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9309ba224d78a42cd159240bc9e97b910076e4f775c140bd32d4dfff0921754`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-x86_64'; 			sha256='4f9b5313cf3eb1651b65aa6fc2fe1f59eb3812b7566f7c1b853be429b81bf3ab'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv6'; 			sha256='44b679381da55d1a673e5e638ac6d34f81e38e58ac656c530e27bb57a0ef930d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv7'; 			sha256='347b65d0cec622976bb753550d2708c8c9c760d55c1b5952a6800f5fadd4781c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-aarch64'; 			sha256='27b3cb1f066cdba191c4df96255a3d7178294763c9d67fba528f769968fc2e65'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-ppc64le'; 			sha256='76981fe4b032385752c5bb07144a22a7dfb599da15eca6fa1775e94364833475'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-riscv64'; 			sha256='1ee27dd153bd796686ece5d1829266b9b0db0a2ed67e7dbef023457da6dc5761'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-s390x'; 			sha256='9ee5fd812e7e52c08b95cd59673b956f2248343c2fb51eb8bcf635b02cfcbee4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
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
	-	`sha256:b751039a3d1e1f4c5da518d2c0ab210d9dde6bb4b882239669c537ca0cca4750`  
		Last Modified: Tue, 14 Nov 2023 02:44:03 GMT  
		Size: 15.9 MB (15893478 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7628bbe10bd17a4da8529f7b50fad49a8ad91dd1fceb4aed606780b6729c45fc`  
		Last Modified: Fri, 17 Nov 2023 19:27:03 GMT  
		Size: 15.6 MB (15640603 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:35c7294792d785d30ab9eea6455359fb54983efac18dd0c9b27e60a31f9cbe6b`  
		Last Modified: Fri, 17 Nov 2023 19:27:04 GMT  
		Size: 16.3 MB (16270055 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94527330b884c45a96c4dbebfb2d9f7f8804889dc9c510677fa14b052634d318`  
		Last Modified: Fri, 17 Nov 2023 19:27:03 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:094bad732e20509665dcb6d9b9cc7bf0aa67ce42b21af3662df1b08e962ac284`  
		Last Modified: Fri, 17 Nov 2023 19:27:03 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1263bf3518124a31d04efae8287b5dde8596eff1039961fe69247fec746057ac`  
		Last Modified: Fri, 17 Nov 2023 19:27:04 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d2ff5764b1e6572821caf7bc40c75b80f0da7b111b52739fbe128d31df9abb38`  
		Last Modified: Fri, 17 Nov 2023 20:26:22 GMT  
		Size: 9.4 MB (9362873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e05639b9185c0f208902cb0e51c450d8694521e788f262ece202ea46fbb2169`  
		Last Modified: Fri, 17 Nov 2023 20:26:21 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7695721bba20680d94d6944d6cd73d71132e0d54f48838e49a7931c529dc971b`  
		Last Modified: Fri, 17 Nov 2023 20:26:25 GMT  
		Size: 51.4 MB (51388553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1eed8b16573b73f5551de19e3c3ca5af42de69cea12d56fb65ef6b9482346fd2`  
		Last Modified: Fri, 17 Nov 2023 20:26:21 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5864b72f995ccfc0fd74116d0942c54bc9e04f541883ea94101bb02124d95493`  
		Last Modified: Fri, 17 Nov 2023 20:26:23 GMT  
		Size: 2.8 KB (2794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5774a4122243aa9d3d55f2391b8755dcef0155bc0e17db82c98f002b170a8794`  
		Last Modified: Fri, 17 Nov 2023 21:30:50 GMT  
		Size: 5.0 MB (5037269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-git` - unknown; unknown

```console
$ docker pull docker@sha256:fcdb3b73de984edbe490c4be581ac848809a8f6b89e2c817d09a1cb00e3166b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **729.3 KB (729307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5b313951824014f3a6e0da125e58762fb031ac9c0363e2d166ad55c1482150f`

```dockerfile
```

-	Layers:
	-	`sha256:48b92a7688a7f1f92966b1963aa86e4a3ae86eae608f31d1b43d1f721efef2d3`  
		Last Modified: Fri, 17 Nov 2023 21:30:50 GMT  
		Size: 718.8 KB (718811 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:041c52df5aeda470be7ec5f8664e73925734a151323f10ec846cf11ed0194c58`  
		Last Modified: Fri, 17 Nov 2023 21:30:50 GMT  
		Size: 10.5 KB (10496 bytes)  
		MIME: application/vnd.in-toto+json
