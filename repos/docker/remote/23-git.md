## `docker:23-git`

```console
$ docker pull docker@sha256:e4b8f0ef5483cc2157a1285dfdcf2f55e521d7af7d067ba38ec355d867fd4070
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-git` - linux; amd64

```console
$ docker pull docker@sha256:ed444b0c0e9c1872b0137eb25a36e347e0724c514811d33b633b8c0abede7a74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117689435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3382ba00f1ffc0a469718858082e75935e5ff4d0cf6cbc7d163a478e41e3fa56`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
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
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
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
	-	`sha256:1cd4867cc7bf586ebd914414a5e00dda99b3e26394f16e97a61f2c3fae0510b7`  
		Last Modified: Thu, 11 May 2023 19:24:57 GMT  
		Size: 16.3 MB (16250881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2bf7d3a8593f2bdcef4f9373667ffb7029a7ba14c2cb4422fb0f7080b54748`  
		Last Modified: Tue, 23 May 2023 01:30:28 GMT  
		Size: 16.0 MB (16003306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1a35c9f637fb838e706b264e809583915601afa7043701c8b93e634bddc34a`  
		Last Modified: Tue, 23 May 2023 01:30:28 GMT  
		Size: 16.4 MB (16398971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce0963642fc4818f430d4417d60760b6988a8eaa3924afdde20d4e80fefea2d`  
		Last Modified: Tue, 23 May 2023 01:30:26 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0204df4233e961d9e9d33bd5ba46bb50fe7024df0eab7c343df8588a10893ec`  
		Last Modified: Tue, 23 May 2023 01:30:26 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2eb33358737b1c41f411e98d4be63fef2a52c6676774f6076631e1482f5227`  
		Last Modified: Tue, 23 May 2023 01:30:26 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af107fcb77c0fcf90d303534d747fad609d655df5134aaaec6510fd4747c18b1`  
		Last Modified: Tue, 23 May 2023 01:30:41 GMT  
		Size: 7.0 MB (7025232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aed1e215477d5b53a1b3b38a4d29889752d7646c9a04aaf0abd80a4d7ed11d0`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca224e6224553593369bbd6e0e10b9095b605b3968e2797d2cdfa7c27dd23d31`  
		Last Modified: Tue, 23 May 2023 01:30:47 GMT  
		Size: 51.7 MB (51657474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50356bbe616fdbd798a7db3e4b6b8ba8b33f4fc9d626d144548620b34d2c6953`  
		Last Modified: Wed, 31 May 2023 17:21:21 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed35ad5fb455941e2c9fc969c24f863f67923ed4e137bd3d331530f38adee6e8`  
		Last Modified: Wed, 31 May 2023 17:21:21 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192f397492b0ecef614e75966e8faaf497c521ef412e34ca83ca66a56c90aa9c`  
		Last Modified: Wed, 31 May 2023 17:21:58 GMT  
		Size: 4.9 MB (4934734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:99dac23c3a6d47a1a1fca2dec9c5fa2bb3d796e9ce7c537020f77f9e0c57a01d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109323111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a90933bc8f7e51b957e3bdd447276f035379e00e05888044de390f20f6a1ad2c`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
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
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
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
	-	`sha256:7755db036d15ac84998f2eac830ac44d7e439c03ecb38bd242508a0481efc0fc`  
		Last Modified: Thu, 11 May 2023 19:43:32 GMT  
		Size: 15.3 MB (15325101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9735b02fc1889e598724f7041f4c95dbc80943e2ac54c1597dd972edbe442c7e`  
		Last Modified: Tue, 23 May 2023 00:41:44 GMT  
		Size: 14.4 MB (14442032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b744dab55c2f79376c36be24bd6ff00a2420f6bca8e4338849dea2604ecded`  
		Last Modified: Tue, 23 May 2023 00:41:44 GMT  
		Size: 14.9 MB (14861191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371149722373a833521d428250394ed67d644a47b1a9ab776e342fd3fe6cb4ea`  
		Last Modified: Tue, 23 May 2023 00:41:42 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5eb9dfcfcca465788c80052151ef524347669ce8cefae2597608df36d30d311`  
		Last Modified: Tue, 23 May 2023 00:41:42 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d2e298ab0e7db064fb5ccd6596a516ceb481f89b3ecdddcd799b7dcd48122f`  
		Last Modified: Tue, 23 May 2023 00:41:42 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c046b843a32e8e152d6b79e8dc11edecef65f6b6c59c97bbd30293561a88def8`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 7.2 MB (7245073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f12b24fd5b777af2ccaaadcc5a9819b6959338d9eaabc94e40fe66ffcbe0bff`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4acbb97b9ecc6183ae232d74b3ecd13f07dd42df858583d3146586538b46773`  
		Last Modified: Tue, 23 May 2023 00:42:00 GMT  
		Size: 47.1 MB (47053346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac869107d4977ca983dd8bfb32f27ea5f54ef4f0b3f60565ac6fa4a624eee5b`  
		Last Modified: Wed, 31 May 2023 17:41:01 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eb778079734789cc7570c9e49eead1c9492c65b56583da718c1f543eba46f5`  
		Last Modified: Wed, 31 May 2023 17:41:01 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5fa970041e67b5416d83d2131666014ae82a1763ac5b21cc4d541b54d84790`  
		Last Modified: Wed, 31 May 2023 17:41:37 GMT  
		Size: 5.0 MB (5021998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
