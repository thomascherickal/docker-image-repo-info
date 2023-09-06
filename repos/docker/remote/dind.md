## `docker:dind`

```console
$ docker pull docker@sha256:9e6dbb25d3c0e1e2d222c8a3f074cb8240d1a716d0c6868f76eb3d5a4dfb174c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:16bf88576270f0d6f9f5f541fedda46d52e94b72bec2efe072f96ef9987d564b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118530847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a2a87562699c0b18562f778157be5e134a1f8df903f0a7cb5aa91f8b97980a4`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

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
	-	`sha256:433699f847492b5117d720534b6d291fe8b8003e28222b240e299036030e3e8f`  
		Last Modified: Wed, 06 Sep 2023 01:52:10 GMT  
		Size: 7.1 MB (7080285 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e5c5f3a87be2111d1f2974817722d6e4afc5c60df1e19e2a8cd69dae7487205`  
		Last Modified: Wed, 06 Sep 2023 01:52:09 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:389d589ce89a7935fd94fbc36b80e1d80df6432a4bb6bd4f7baf47510833d4a8`  
		Last Modified: Wed, 06 Sep 2023 01:52:13 GMT  
		Size: 54.4 MB (54351538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43e1216f5007c0c68117a0efc85b32d626695b6bd8033f0cdddb9ea42b39195`  
		Last Modified: Wed, 06 Sep 2023 01:52:10 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2c2a8ce1e4eb61e848643542841eb7812139251a70a79857d4660904d5d1b404`  
		Last Modified: Wed, 06 Sep 2023 01:52:11 GMT  
		Size: 2.8 KB (2788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:95933b1594ed75184a3837dd21df1caf0416c0916d3e922fc7f04128868bedba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **962.0 KB (961995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ffc8c90f8099e363c17d984ef3d2c9cd1117e0fdfced31fdfe6a8f3991063f`

```dockerfile
```

-	Layers:
	-	`sha256:41f7de19a9f6aa9e44efc1fc9a7c55ca4f6b3c33c5833cd087935d9e2d3f323c`  
		Last Modified: Wed, 06 Sep 2023 01:52:09 GMT  
		Size: 931.9 KB (931857 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2587117166530cd2a105d4ecf022184f8f6a7e010bb75c3a812d95c02fc66e41`  
		Last Modified: Wed, 06 Sep 2023 01:52:09 GMT  
		Size: 30.1 KB (30138 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5d24f7bbfe68556d4494c0719e1d1c0d23092f3251bd1d8d28e24c9b1b70ee81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109832113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26fd1c34bf500da20cb0e1ce0cc53fbae1813eb234a4e4741c3f33b5a85d7654`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

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
	-	`sha256:8cf3fdb5711b2ab00d9fd53b7881b79dd713ff4bb4e241b66cbd7cc9f3d46273`  
		Last Modified: Wed, 06 Sep 2023 01:57:51 GMT  
		Size: 7.3 MB (7291231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36ac283ad2d49278a77b95e0a0e5df2e26c0193887c9ce298229b60de6761e51`  
		Last Modified: Wed, 06 Sep 2023 01:57:50 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f3c41fd9ebb0e13ce99e76fd7377067508922b4147b10b2552a88981b3adfdf`  
		Last Modified: Wed, 06 Sep 2023 01:57:52 GMT  
		Size: 49.7 MB (49688275 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29a5074801a269765b60ab3e7b4ecfa7b62596a2ee41ae6e43d8e5e71427956e`  
		Last Modified: Wed, 06 Sep 2023 01:57:50 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a0cc6640ec8f561f319bc4ac94c8b144841e2017b0186063aca4a506e7533b2`  
		Last Modified: Wed, 06 Sep 2023 01:57:51 GMT  
		Size: 2.8 KB (2788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:222ae150b437210f381245f086de3de6d200595b7104152c9e524c75c44653d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **962.3 KB (962296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fda399b12b89d10e4d57fec08c9df373e1613431ab2beea9394d57e20f141bce`

```dockerfile
```

-	Layers:
	-	`sha256:a2b64fc42404117abd9f23bff68d779f1dc57f7a92c70d4869e0cff879b90ff2`  
		Last Modified: Wed, 06 Sep 2023 01:57:50 GMT  
		Size: 932.1 KB (932088 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0004d39758fe245b2564520c732b7b7d712f1e77f6eb47fbf7115d0238d323b2`  
		Last Modified: Wed, 06 Sep 2023 01:57:49 GMT  
		Size: 30.2 KB (30208 bytes)  
		MIME: application/vnd.in-toto+json
