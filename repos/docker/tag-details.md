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
-	[`docker:24.0.2`](#docker2402)
-	[`docker:24.0.2-alpine3.18`](#docker2402-alpine318)
-	[`docker:24.0.2-cli`](#docker2402-cli)
-	[`docker:24.0.2-cli-alpine3.18`](#docker2402-cli-alpine318)
-	[`docker:24.0.2-dind`](#docker2402-dind)
-	[`docker:24.0.2-dind-alpine3.18`](#docker2402-dind-alpine318)
-	[`docker:24.0.2-dind-rootless`](#docker2402-dind-rootless)
-	[`docker:24.0.2-git`](#docker2402-git)
-	[`docker:24.0.2-windowsservercore`](#docker2402-windowsservercore)
-	[`docker:24.0.2-windowsservercore-1809`](#docker2402-windowsservercore-1809)
-	[`docker:24.0.2-windowsservercore-ltsc2022`](#docker2402-windowsservercore-ltsc2022)
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
$ docker pull docker@sha256:0e0a13763a8f205f4fabbd50aa27a8d45e6ce912bbf22d81891747c025ad0435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23` - linux; amd64

```console
$ docker pull docker@sha256:8dabbbecf95953382f0c6e06731aa3e7066fd294456e5cd4b63980905c988ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112754695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042873844fa732b947ab125a5c4289e9182bcd776c7eaaba6e619a031ec09ffc`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5aa2e8ff6975e8917a1405ea2e4c661f5922cc1a632e0c70d8e2c5fb435c1059
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104301108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e94ded36c2428fbbf66e5644cfbaea58a21682b9729bf21260a479ec6d9539`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-cli`

```console
$ docker pull docker@sha256:b4c0173a2c0a2ddd55b70c5aaa8d39e10b1e67d2d97d32ea2f6c0559b23d57c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-cli` - linux; amd64

```console
$ docker pull docker@sha256:2268c14a72187fa6fa1dfa389189dcf3ef89adbcf2cfa4f15a9491594f4496e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54066828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3881fc1266148372f542994988546021911ed074ce929bbae6ea3f006c222c8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

### `docker:23-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:05ca23f1798f1b83b1261848b347677b76cbbb4347493d09936e55bae1440089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (49997530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c5622b9da61ebbe73a78e34e0725769263d9ecce510f8b21f04a81a8c53573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

## `docker:23-dind`

```console
$ docker pull docker@sha256:0e0a13763a8f205f4fabbd50aa27a8d45e6ce912bbf22d81891747c025ad0435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-dind` - linux; amd64

```console
$ docker pull docker@sha256:8dabbbecf95953382f0c6e06731aa3e7066fd294456e5cd4b63980905c988ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112754695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042873844fa732b947ab125a5c4289e9182bcd776c7eaaba6e619a031ec09ffc`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5aa2e8ff6975e8917a1405ea2e4c661f5922cc1a632e0c70d8e2c5fb435c1059
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104301108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e94ded36c2428fbbf66e5644cfbaea58a21682b9729bf21260a479ec6d9539`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-dind-rootless`

```console
$ docker pull docker@sha256:cc699bde5ec4e456bb88351bdbb944147cb45230dedd4fb0cb39a9eeef9a9ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:d761895dc5f9aa6e87d2899fe4f693e18ac367bf901001cd6dc809c783d64bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134465841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb075d1c418b139e3f3e4c026a902f543b29ef92a4d8ed517f48bbe52e2648cf`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:04:13 GMT
USER rootless
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183a81df7074af37fef47bad0bf3689a97675bf0f29f684e99eb2e138a7fe923`  
		Last Modified: Tue, 23 May 2023 01:31:11 GMT  
		Size: 1.4 MB (1362321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f042cc93b88f9da7c33d210d3d5e514b98dda97776be88f6bcb077f9885e3b`  
		Last Modified: Tue, 23 May 2023 01:31:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6b19692c9c41512fd105e4cb801243265b53619da977e3481abc1a137c36ce`  
		Last Modified: Tue, 23 May 2023 01:31:10 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f6cd43f046fa8a453e36f5b0e09ac988704baeb649609512fd59bb6ffc607a`  
		Last Modified: Tue, 23 May 2023 01:31:14 GMT  
		Size: 20.3 MB (20347085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1105de0a7b65861fc384209c88744c4b17a453c46e189d6870372a93a4a1a574`  
		Last Modified: Tue, 23 May 2023 01:31:10 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6a20405976113067e58b2350402efc4125df9856eb9bb5051fc76bf9a58606f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127957082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16a6661d1f938a3670469c70932e9d3b374b35002fd218cb1195055349d2792`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:04:13 GMT
USER rootless
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a221c052d8f4d947d27bcb519230f627c66ffd9c56eef7c7ed8ae32b17ecd`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 1.4 MB (1413234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b366c3261134398156def9cf688e0dff7d8245510633d1250b63768a10c8570`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ee6309005434997742616afbfeab419b320650a8fd298b13d028e1312d2cad`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce60664ecf82dbfaba8e838928543d25be7920e830cbd4769f8314e2cfe08462`  
		Last Modified: Tue, 23 May 2023 00:42:25 GMT  
		Size: 22.2 MB (22241002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5080c898affabeb5c0f542e468195366b360db7b6f487b210d0e52c7ce77055c`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-git`

```console
$ docker pull docker@sha256:b338d9671e91de405727a46299f0e5e09285d7b774ed92830dd9f5ef7f05e181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-git` - linux; amd64

```console
$ docker pull docker@sha256:976676d9a2d7913effce51ca5e4a2566afafe088214383b2be53d35ba7ee5814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117690898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f884d03a70972d5e8a85462748ccdcc26223a475a3a4424cbb6b92434250e49`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a19ad78c6a43a465489ac7c03a1d7107e09dc878cc11c42d37e0685f8b20855`  
		Last Modified: Tue, 23 May 2023 01:31:26 GMT  
		Size: 4.9 MB (4936203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a051918fa248b7a0783b0da0440a14980091164d9fd51144c8b8c84c7e1939ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109323095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542ac1d59c8e828780951585daf29fe742e8804326506a762e886294be27a451`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ddd17db46fbe8b408cef594756cacc789e6d941b0a689863231307e09747de`  
		Last Modified: Tue, 23 May 2023 00:42:36 GMT  
		Size: 5.0 MB (5021987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore`

```console
$ docker pull docker@sha256:37a53bc81b6bab367a86f1c90e1899ff8bf5da034ea59a6a09a1aa5eb84b3902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `docker:23-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:364433d2b1bee777551a4b6779b0dd8b8132b1fccf3134e4d32a84a37c5c7cc3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826092276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b29bc2769bda71a53814c9ccc2383659cb031973e0c33db6abe1d6784310f5d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:24:47 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:24:48 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:25:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:18:59 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:19:27 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:19:29 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:19:55 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e927fbd88402bacc902c2a4593f281068b2a6657c7f8b4e53ac01f8e636901`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165e88795de1230f78ac3b0186a534bd16fad90474fddb00254443f5440c8c65`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438806a743132696d59ff6500d80c1c45b0742da1613dbde135436ef14f725af`  
		Last Modified: Wed, 10 May 2023 07:12:05 GMT  
		Size: 17.3 MB (17316446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417a1edd59934c95c4868f309ce4bd3a9a118aa715175b458b58a35cc1d3e69`  
		Last Modified: Tue, 23 May 2023 01:23:58 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd3977cea96c5c0118f0d34ef8ba6fc71301b74c38d39e7f15f7dcdb69e1121`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54725b68c251ce31613b171528908d72d35d3215608b6f432106bd0c89fd09d`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fd6daf68cdb9ac02732b4bc36377df7d2f63dbd5895badf87cb752e4e45b9a`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.5 MB (16478754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420f8ee3234484fb8f90ced11de46a4b0a8b7fc3cb5f780d1afec5a5de6e0140`  
		Last Modified: Tue, 23 May 2023 01:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d4770e7ab12298d99f71bed561ebf178867b7334ce2af75f237a87075e2f0c`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e907c88699d119d767495b663709d88859d0b84f2a185720f0d165d1571ba`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c95f872c776b4819132fef9832663b2a016e299293b42dae162232eb0956b`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.9 MB (16855888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:17719a45a40b20e31856f9d0018b74309c2ed9bcee055a8720da3bcc9d2ad23d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123215918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3985a943db5c8a91e7819b97867bea926b75f762728894aed317d8851153720f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:26:29 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:26:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:27:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:20:11 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:21:24 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:21:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:21:25 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:21:26 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:22:38 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470efce6095b6077dfd4d6bac6f6e2010f4d5bcdf636e954d0c3e9051baa7a30`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf94d195dbf8bcb75f6433208dda2b0af64c556bf5eed006468d61cccf49971`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f57c72aed2637dc5fc359ff575642812168a390b96d73791c2e00a8aa6c341`  
		Last Modified: Wed, 10 May 2023 07:12:25 GMT  
		Size: 17.3 MB (17330027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e8210888899a756f382a39956b49d936c3b3cc971c774ce106ea7c8ba79242`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761df73e02dadef61574b35ea93d0e12a71dddedfc2dd753cd779a11357c70`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d36348f928d37d3f3e668f8e40784a2d752409a2ab7d5ede9ec734c9d3e42dc`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e6a84fd41f60c1e053b947d5c121e87c9470ad2286b9da138f18743834c865`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.5 MB (16508243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2e0d76930bfb9e698b63a3a4c38d6e31a80d1885e764818ab2d3f7c6fd52b6`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1a0bf4e1377e52d886720ca9ed0a40b713374b1199aded6392ccb26454da12`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c690caa81cfd8344dfa4e473cc140c0052d2c5089c7a3f44c2b0c22ac146e29`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7120d2bb370c638876227ff5daaf5733d38f7bd0ce70787c17036c82d3ab1b94`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.9 MB (16878148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore-1809`

```console
$ docker pull docker@sha256:b76a54c14230c028a765839be85ba9f81c771ffa41f2daee9839abaf48d00c66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `docker:23-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:17719a45a40b20e31856f9d0018b74309c2ed9bcee055a8720da3bcc9d2ad23d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123215918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3985a943db5c8a91e7819b97867bea926b75f762728894aed317d8851153720f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:26:29 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:26:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:27:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:20:11 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:21:24 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:21:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:21:25 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:21:26 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:22:38 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470efce6095b6077dfd4d6bac6f6e2010f4d5bcdf636e954d0c3e9051baa7a30`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf94d195dbf8bcb75f6433208dda2b0af64c556bf5eed006468d61cccf49971`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f57c72aed2637dc5fc359ff575642812168a390b96d73791c2e00a8aa6c341`  
		Last Modified: Wed, 10 May 2023 07:12:25 GMT  
		Size: 17.3 MB (17330027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e8210888899a756f382a39956b49d936c3b3cc971c774ce106ea7c8ba79242`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761df73e02dadef61574b35ea93d0e12a71dddedfc2dd753cd779a11357c70`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d36348f928d37d3f3e668f8e40784a2d752409a2ab7d5ede9ec734c9d3e42dc`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e6a84fd41f60c1e053b947d5c121e87c9470ad2286b9da138f18743834c865`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.5 MB (16508243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2e0d76930bfb9e698b63a3a4c38d6e31a80d1885e764818ab2d3f7c6fd52b6`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1a0bf4e1377e52d886720ca9ed0a40b713374b1199aded6392ccb26454da12`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c690caa81cfd8344dfa4e473cc140c0052d2c5089c7a3f44c2b0c22ac146e29`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7120d2bb370c638876227ff5daaf5733d38f7bd0ce70787c17036c82d3ab1b94`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.9 MB (16878148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:dedc3189f736ae43f2abc035c0d9df0ac5279c4fef6e0b8816359c4936943f8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `docker:23-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:364433d2b1bee777551a4b6779b0dd8b8132b1fccf3134e4d32a84a37c5c7cc3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826092276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b29bc2769bda71a53814c9ccc2383659cb031973e0c33db6abe1d6784310f5d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:24:47 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:24:48 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:25:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:18:59 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:19:27 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:19:29 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:19:55 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e927fbd88402bacc902c2a4593f281068b2a6657c7f8b4e53ac01f8e636901`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165e88795de1230f78ac3b0186a534bd16fad90474fddb00254443f5440c8c65`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438806a743132696d59ff6500d80c1c45b0742da1613dbde135436ef14f725af`  
		Last Modified: Wed, 10 May 2023 07:12:05 GMT  
		Size: 17.3 MB (17316446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417a1edd59934c95c4868f309ce4bd3a9a118aa715175b458b58a35cc1d3e69`  
		Last Modified: Tue, 23 May 2023 01:23:58 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd3977cea96c5c0118f0d34ef8ba6fc71301b74c38d39e7f15f7dcdb69e1121`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54725b68c251ce31613b171528908d72d35d3215608b6f432106bd0c89fd09d`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fd6daf68cdb9ac02732b4bc36377df7d2f63dbd5895badf87cb752e4e45b9a`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.5 MB (16478754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420f8ee3234484fb8f90ced11de46a4b0a8b7fc3cb5f780d1afec5a5de6e0140`  
		Last Modified: Tue, 23 May 2023 01:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d4770e7ab12298d99f71bed561ebf178867b7334ce2af75f237a87075e2f0c`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e907c88699d119d767495b663709d88859d0b84f2a185720f0d165d1571ba`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c95f872c776b4819132fef9832663b2a016e299293b42dae162232eb0956b`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.9 MB (16855888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0`

```console
$ docker pull docker@sha256:0e0a13763a8f205f4fabbd50aa27a8d45e6ce912bbf22d81891747c025ad0435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0` - linux; amd64

```console
$ docker pull docker@sha256:8dabbbecf95953382f0c6e06731aa3e7066fd294456e5cd4b63980905c988ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112754695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042873844fa732b947ab125a5c4289e9182bcd776c7eaaba6e619a031ec09ffc`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5aa2e8ff6975e8917a1405ea2e4c661f5922cc1a632e0c70d8e2c5fb435c1059
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104301108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e94ded36c2428fbbf66e5644cfbaea58a21682b9729bf21260a479ec6d9539`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-cli`

```console
$ docker pull docker@sha256:b4c0173a2c0a2ddd55b70c5aaa8d39e10b1e67d2d97d32ea2f6c0559b23d57c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-cli` - linux; amd64

```console
$ docker pull docker@sha256:2268c14a72187fa6fa1dfa389189dcf3ef89adbcf2cfa4f15a9491594f4496e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54066828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3881fc1266148372f542994988546021911ed074ce929bbae6ea3f006c222c8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

### `docker:23.0-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:05ca23f1798f1b83b1261848b347677b76cbbb4347493d09936e55bae1440089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (49997530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c5622b9da61ebbe73a78e34e0725769263d9ecce510f8b21f04a81a8c53573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

## `docker:23.0-dind`

```console
$ docker pull docker@sha256:0e0a13763a8f205f4fabbd50aa27a8d45e6ce912bbf22d81891747c025ad0435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:8dabbbecf95953382f0c6e06731aa3e7066fd294456e5cd4b63980905c988ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112754695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042873844fa732b947ab125a5c4289e9182bcd776c7eaaba6e619a031ec09ffc`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5aa2e8ff6975e8917a1405ea2e4c661f5922cc1a632e0c70d8e2c5fb435c1059
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104301108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e94ded36c2428fbbf66e5644cfbaea58a21682b9729bf21260a479ec6d9539`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-dind-rootless`

```console
$ docker pull docker@sha256:cc699bde5ec4e456bb88351bdbb944147cb45230dedd4fb0cb39a9eeef9a9ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:d761895dc5f9aa6e87d2899fe4f693e18ac367bf901001cd6dc809c783d64bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134465841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb075d1c418b139e3f3e4c026a902f543b29ef92a4d8ed517f48bbe52e2648cf`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:04:13 GMT
USER rootless
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183a81df7074af37fef47bad0bf3689a97675bf0f29f684e99eb2e138a7fe923`  
		Last Modified: Tue, 23 May 2023 01:31:11 GMT  
		Size: 1.4 MB (1362321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f042cc93b88f9da7c33d210d3d5e514b98dda97776be88f6bcb077f9885e3b`  
		Last Modified: Tue, 23 May 2023 01:31:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6b19692c9c41512fd105e4cb801243265b53619da977e3481abc1a137c36ce`  
		Last Modified: Tue, 23 May 2023 01:31:10 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f6cd43f046fa8a453e36f5b0e09ac988704baeb649609512fd59bb6ffc607a`  
		Last Modified: Tue, 23 May 2023 01:31:14 GMT  
		Size: 20.3 MB (20347085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1105de0a7b65861fc384209c88744c4b17a453c46e189d6870372a93a4a1a574`  
		Last Modified: Tue, 23 May 2023 01:31:10 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6a20405976113067e58b2350402efc4125df9856eb9bb5051fc76bf9a58606f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127957082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16a6661d1f938a3670469c70932e9d3b374b35002fd218cb1195055349d2792`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:04:13 GMT
USER rootless
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a221c052d8f4d947d27bcb519230f627c66ffd9c56eef7c7ed8ae32b17ecd`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 1.4 MB (1413234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b366c3261134398156def9cf688e0dff7d8245510633d1250b63768a10c8570`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ee6309005434997742616afbfeab419b320650a8fd298b13d028e1312d2cad`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce60664ecf82dbfaba8e838928543d25be7920e830cbd4769f8314e2cfe08462`  
		Last Modified: Tue, 23 May 2023 00:42:25 GMT  
		Size: 22.2 MB (22241002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5080c898affabeb5c0f542e468195366b360db7b6f487b210d0e52c7ce77055c`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-git`

```console
$ docker pull docker@sha256:b338d9671e91de405727a46299f0e5e09285d7b774ed92830dd9f5ef7f05e181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-git` - linux; amd64

```console
$ docker pull docker@sha256:976676d9a2d7913effce51ca5e4a2566afafe088214383b2be53d35ba7ee5814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117690898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f884d03a70972d5e8a85462748ccdcc26223a475a3a4424cbb6b92434250e49`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a19ad78c6a43a465489ac7c03a1d7107e09dc878cc11c42d37e0685f8b20855`  
		Last Modified: Tue, 23 May 2023 01:31:26 GMT  
		Size: 4.9 MB (4936203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a051918fa248b7a0783b0da0440a14980091164d9fd51144c8b8c84c7e1939ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109323095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542ac1d59c8e828780951585daf29fe742e8804326506a762e886294be27a451`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ddd17db46fbe8b408cef594756cacc789e6d941b0a689863231307e09747de`  
		Last Modified: Tue, 23 May 2023 00:42:36 GMT  
		Size: 5.0 MB (5021987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore`

```console
$ docker pull docker@sha256:37a53bc81b6bab367a86f1c90e1899ff8bf5da034ea59a6a09a1aa5eb84b3902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `docker:23.0-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:364433d2b1bee777551a4b6779b0dd8b8132b1fccf3134e4d32a84a37c5c7cc3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826092276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b29bc2769bda71a53814c9ccc2383659cb031973e0c33db6abe1d6784310f5d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:24:47 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:24:48 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:25:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:18:59 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:19:27 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:19:29 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:19:55 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e927fbd88402bacc902c2a4593f281068b2a6657c7f8b4e53ac01f8e636901`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165e88795de1230f78ac3b0186a534bd16fad90474fddb00254443f5440c8c65`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438806a743132696d59ff6500d80c1c45b0742da1613dbde135436ef14f725af`  
		Last Modified: Wed, 10 May 2023 07:12:05 GMT  
		Size: 17.3 MB (17316446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417a1edd59934c95c4868f309ce4bd3a9a118aa715175b458b58a35cc1d3e69`  
		Last Modified: Tue, 23 May 2023 01:23:58 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd3977cea96c5c0118f0d34ef8ba6fc71301b74c38d39e7f15f7dcdb69e1121`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54725b68c251ce31613b171528908d72d35d3215608b6f432106bd0c89fd09d`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fd6daf68cdb9ac02732b4bc36377df7d2f63dbd5895badf87cb752e4e45b9a`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.5 MB (16478754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420f8ee3234484fb8f90ced11de46a4b0a8b7fc3cb5f780d1afec5a5de6e0140`  
		Last Modified: Tue, 23 May 2023 01:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d4770e7ab12298d99f71bed561ebf178867b7334ce2af75f237a87075e2f0c`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e907c88699d119d767495b663709d88859d0b84f2a185720f0d165d1571ba`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c95f872c776b4819132fef9832663b2a016e299293b42dae162232eb0956b`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.9 MB (16855888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:17719a45a40b20e31856f9d0018b74309c2ed9bcee055a8720da3bcc9d2ad23d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123215918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3985a943db5c8a91e7819b97867bea926b75f762728894aed317d8851153720f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:26:29 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:26:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:27:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:20:11 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:21:24 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:21:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:21:25 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:21:26 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:22:38 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470efce6095b6077dfd4d6bac6f6e2010f4d5bcdf636e954d0c3e9051baa7a30`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf94d195dbf8bcb75f6433208dda2b0af64c556bf5eed006468d61cccf49971`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f57c72aed2637dc5fc359ff575642812168a390b96d73791c2e00a8aa6c341`  
		Last Modified: Wed, 10 May 2023 07:12:25 GMT  
		Size: 17.3 MB (17330027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e8210888899a756f382a39956b49d936c3b3cc971c774ce106ea7c8ba79242`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761df73e02dadef61574b35ea93d0e12a71dddedfc2dd753cd779a11357c70`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d36348f928d37d3f3e668f8e40784a2d752409a2ab7d5ede9ec734c9d3e42dc`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e6a84fd41f60c1e053b947d5c121e87c9470ad2286b9da138f18743834c865`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.5 MB (16508243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2e0d76930bfb9e698b63a3a4c38d6e31a80d1885e764818ab2d3f7c6fd52b6`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1a0bf4e1377e52d886720ca9ed0a40b713374b1199aded6392ccb26454da12`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c690caa81cfd8344dfa4e473cc140c0052d2c5089c7a3f44c2b0c22ac146e29`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7120d2bb370c638876227ff5daaf5733d38f7bd0ce70787c17036c82d3ab1b94`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.9 MB (16878148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore-1809`

```console
$ docker pull docker@sha256:b76a54c14230c028a765839be85ba9f81c771ffa41f2daee9839abaf48d00c66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `docker:23.0-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:17719a45a40b20e31856f9d0018b74309c2ed9bcee055a8720da3bcc9d2ad23d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123215918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3985a943db5c8a91e7819b97867bea926b75f762728894aed317d8851153720f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:26:29 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:26:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:27:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:20:11 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:21:24 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:21:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:21:25 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:21:26 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:22:38 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470efce6095b6077dfd4d6bac6f6e2010f4d5bcdf636e954d0c3e9051baa7a30`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf94d195dbf8bcb75f6433208dda2b0af64c556bf5eed006468d61cccf49971`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f57c72aed2637dc5fc359ff575642812168a390b96d73791c2e00a8aa6c341`  
		Last Modified: Wed, 10 May 2023 07:12:25 GMT  
		Size: 17.3 MB (17330027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e8210888899a756f382a39956b49d936c3b3cc971c774ce106ea7c8ba79242`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761df73e02dadef61574b35ea93d0e12a71dddedfc2dd753cd779a11357c70`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d36348f928d37d3f3e668f8e40784a2d752409a2ab7d5ede9ec734c9d3e42dc`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e6a84fd41f60c1e053b947d5c121e87c9470ad2286b9da138f18743834c865`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.5 MB (16508243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2e0d76930bfb9e698b63a3a4c38d6e31a80d1885e764818ab2d3f7c6fd52b6`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1a0bf4e1377e52d886720ca9ed0a40b713374b1199aded6392ccb26454da12`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c690caa81cfd8344dfa4e473cc140c0052d2c5089c7a3f44c2b0c22ac146e29`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7120d2bb370c638876227ff5daaf5733d38f7bd0ce70787c17036c82d3ab1b94`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.9 MB (16878148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:dedc3189f736ae43f2abc035c0d9df0ac5279c4fef6e0b8816359c4936943f8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `docker:23.0-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:364433d2b1bee777551a4b6779b0dd8b8132b1fccf3134e4d32a84a37c5c7cc3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826092276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b29bc2769bda71a53814c9ccc2383659cb031973e0c33db6abe1d6784310f5d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:24:47 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:24:48 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:25:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:18:59 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:19:27 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:19:29 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:19:55 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e927fbd88402bacc902c2a4593f281068b2a6657c7f8b4e53ac01f8e636901`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165e88795de1230f78ac3b0186a534bd16fad90474fddb00254443f5440c8c65`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438806a743132696d59ff6500d80c1c45b0742da1613dbde135436ef14f725af`  
		Last Modified: Wed, 10 May 2023 07:12:05 GMT  
		Size: 17.3 MB (17316446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417a1edd59934c95c4868f309ce4bd3a9a118aa715175b458b58a35cc1d3e69`  
		Last Modified: Tue, 23 May 2023 01:23:58 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd3977cea96c5c0118f0d34ef8ba6fc71301b74c38d39e7f15f7dcdb69e1121`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54725b68c251ce31613b171528908d72d35d3215608b6f432106bd0c89fd09d`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fd6daf68cdb9ac02732b4bc36377df7d2f63dbd5895badf87cb752e4e45b9a`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.5 MB (16478754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420f8ee3234484fb8f90ced11de46a4b0a8b7fc3cb5f780d1afec5a5de6e0140`  
		Last Modified: Tue, 23 May 2023 01:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d4770e7ab12298d99f71bed561ebf178867b7334ce2af75f237a87075e2f0c`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e907c88699d119d767495b663709d88859d0b84f2a185720f0d165d1571ba`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c95f872c776b4819132fef9832663b2a016e299293b42dae162232eb0956b`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.9 MB (16855888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6`

```console
$ docker pull docker@sha256:0e0a13763a8f205f4fabbd50aa27a8d45e6ce912bbf22d81891747c025ad0435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6` - linux; amd64

```console
$ docker pull docker@sha256:8dabbbecf95953382f0c6e06731aa3e7066fd294456e5cd4b63980905c988ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112754695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042873844fa732b947ab125a5c4289e9182bcd776c7eaaba6e619a031ec09ffc`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5aa2e8ff6975e8917a1405ea2e4c661f5922cc1a632e0c70d8e2c5fb435c1059
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104301108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e94ded36c2428fbbf66e5644cfbaea58a21682b9729bf21260a479ec6d9539`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-alpine3.18`

```console
$ docker pull docker@sha256:0e0a13763a8f205f4fabbd50aa27a8d45e6ce912bbf22d81891747c025ad0435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:8dabbbecf95953382f0c6e06731aa3e7066fd294456e5cd4b63980905c988ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112754695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042873844fa732b947ab125a5c4289e9182bcd776c7eaaba6e619a031ec09ffc`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5aa2e8ff6975e8917a1405ea2e4c661f5922cc1a632e0c70d8e2c5fb435c1059
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104301108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e94ded36c2428fbbf66e5644cfbaea58a21682b9729bf21260a479ec6d9539`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-cli`

```console
$ docker pull docker@sha256:b4c0173a2c0a2ddd55b70c5aaa8d39e10b1e67d2d97d32ea2f6c0559b23d57c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-cli` - linux; amd64

```console
$ docker pull docker@sha256:2268c14a72187fa6fa1dfa389189dcf3ef89adbcf2cfa4f15a9491594f4496e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54066828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3881fc1266148372f542994988546021911ed074ce929bbae6ea3f006c222c8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

### `docker:23.0.6-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:05ca23f1798f1b83b1261848b347677b76cbbb4347493d09936e55bae1440089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (49997530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c5622b9da61ebbe73a78e34e0725769263d9ecce510f8b21f04a81a8c53573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

## `docker:23.0.6-cli-alpine3.18`

```console
$ docker pull docker@sha256:b4c0173a2c0a2ddd55b70c5aaa8d39e10b1e67d2d97d32ea2f6c0559b23d57c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-cli-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:2268c14a72187fa6fa1dfa389189dcf3ef89adbcf2cfa4f15a9491594f4496e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54066828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3881fc1266148372f542994988546021911ed074ce929bbae6ea3f006c222c8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

### `docker:23.0.6-cli-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:05ca23f1798f1b83b1261848b347677b76cbbb4347493d09936e55bae1440089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (49997530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c5622b9da61ebbe73a78e34e0725769263d9ecce510f8b21f04a81a8c53573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

## `docker:23.0.6-dind`

```console
$ docker pull docker@sha256:0e0a13763a8f205f4fabbd50aa27a8d45e6ce912bbf22d81891747c025ad0435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-dind` - linux; amd64

```console
$ docker pull docker@sha256:8dabbbecf95953382f0c6e06731aa3e7066fd294456e5cd4b63980905c988ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112754695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042873844fa732b947ab125a5c4289e9182bcd776c7eaaba6e619a031ec09ffc`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5aa2e8ff6975e8917a1405ea2e4c661f5922cc1a632e0c70d8e2c5fb435c1059
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104301108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e94ded36c2428fbbf66e5644cfbaea58a21682b9729bf21260a479ec6d9539`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-dind-alpine3.18`

```console
$ docker pull docker@sha256:0e0a13763a8f205f4fabbd50aa27a8d45e6ce912bbf22d81891747c025ad0435
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-dind-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:8dabbbecf95953382f0c6e06731aa3e7066fd294456e5cd4b63980905c988ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112754695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042873844fa732b947ab125a5c4289e9182bcd776c7eaaba6e619a031ec09ffc`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-dind-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5aa2e8ff6975e8917a1405ea2e4c661f5922cc1a632e0c70d8e2c5fb435c1059
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104301108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e94ded36c2428fbbf66e5644cfbaea58a21682b9729bf21260a479ec6d9539`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-dind-rootless`

```console
$ docker pull docker@sha256:cc699bde5ec4e456bb88351bdbb944147cb45230dedd4fb0cb39a9eeef9a9ff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:d761895dc5f9aa6e87d2899fe4f693e18ac367bf901001cd6dc809c783d64bc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134465841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb075d1c418b139e3f3e4c026a902f543b29ef92a4d8ed517f48bbe52e2648cf`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:04:13 GMT
USER rootless
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183a81df7074af37fef47bad0bf3689a97675bf0f29f684e99eb2e138a7fe923`  
		Last Modified: Tue, 23 May 2023 01:31:11 GMT  
		Size: 1.4 MB (1362321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f042cc93b88f9da7c33d210d3d5e514b98dda97776be88f6bcb077f9885e3b`  
		Last Modified: Tue, 23 May 2023 01:31:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6b19692c9c41512fd105e4cb801243265b53619da977e3481abc1a137c36ce`  
		Last Modified: Tue, 23 May 2023 01:31:10 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f6cd43f046fa8a453e36f5b0e09ac988704baeb649609512fd59bb6ffc607a`  
		Last Modified: Tue, 23 May 2023 01:31:14 GMT  
		Size: 20.3 MB (20347085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1105de0a7b65861fc384209c88744c4b17a453c46e189d6870372a93a4a1a574`  
		Last Modified: Tue, 23 May 2023 01:31:10 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:6a20405976113067e58b2350402efc4125df9856eb9bb5051fc76bf9a58606f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127957082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16a6661d1f938a3670469c70932e9d3b374b35002fd218cb1195055349d2792`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:04:13 GMT
USER rootless
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a221c052d8f4d947d27bcb519230f627c66ffd9c56eef7c7ed8ae32b17ecd`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 1.4 MB (1413234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b366c3261134398156def9cf688e0dff7d8245510633d1250b63768a10c8570`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ee6309005434997742616afbfeab419b320650a8fd298b13d028e1312d2cad`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce60664ecf82dbfaba8e838928543d25be7920e830cbd4769f8314e2cfe08462`  
		Last Modified: Tue, 23 May 2023 00:42:25 GMT  
		Size: 22.2 MB (22241002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5080c898affabeb5c0f542e468195366b360db7b6f487b210d0e52c7ce77055c`  
		Last Modified: Tue, 23 May 2023 00:42:22 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-git`

```console
$ docker pull docker@sha256:b338d9671e91de405727a46299f0e5e09285d7b774ed92830dd9f5ef7f05e181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-git` - linux; amd64

```console
$ docker pull docker@sha256:976676d9a2d7913effce51ca5e4a2566afafe088214383b2be53d35ba7ee5814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117690898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f884d03a70972d5e8a85462748ccdcc26223a475a3a4424cbb6b92434250e49`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
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
	-	`sha256:af073b9a77d2e8e3956715cafc7e1b9eeaa375ce78bca4d775a23dbea074132d`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4847a5dae97a4c356369e13e5aba7d266a885fff53f140ee446ac1c6fadc9a50`  
		Last Modified: Tue, 23 May 2023 01:30:40 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a19ad78c6a43a465489ac7c03a1d7107e09dc878cc11c42d37e0685f8b20855`  
		Last Modified: Tue, 23 May 2023 01:31:26 GMT  
		Size: 4.9 MB (4936203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a051918fa248b7a0783b0da0440a14980091164d9fd51144c8b8c84c7e1939ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109323095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542ac1d59c8e828780951585daf29fe742e8804326506a762e886294be27a451`
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
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:04:13 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:04:13 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:04:13 GMT
CMD []
# Mon, 22 May 2023 23:04:13 GMT
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
	-	`sha256:ae1280f16201c7f3080108f7eb9176c8c6b72a59138458cec26417d19e7e0820`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0bb7925531acdec5e41409c726eef651fa17bd41f7377fb4fd2ef44b1d621b`  
		Last Modified: Tue, 23 May 2023 00:41:56 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ddd17db46fbe8b408cef594756cacc789e6d941b0a689863231307e09747de`  
		Last Modified: Tue, 23 May 2023 00:42:36 GMT  
		Size: 5.0 MB (5021987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-windowsservercore`

```console
$ docker pull docker@sha256:37a53bc81b6bab367a86f1c90e1899ff8bf5da034ea59a6a09a1aa5eb84b3902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `docker:23.0.6-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:364433d2b1bee777551a4b6779b0dd8b8132b1fccf3134e4d32a84a37c5c7cc3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826092276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b29bc2769bda71a53814c9ccc2383659cb031973e0c33db6abe1d6784310f5d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:24:47 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:24:48 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:25:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:18:59 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:19:27 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:19:29 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:19:55 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e927fbd88402bacc902c2a4593f281068b2a6657c7f8b4e53ac01f8e636901`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165e88795de1230f78ac3b0186a534bd16fad90474fddb00254443f5440c8c65`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438806a743132696d59ff6500d80c1c45b0742da1613dbde135436ef14f725af`  
		Last Modified: Wed, 10 May 2023 07:12:05 GMT  
		Size: 17.3 MB (17316446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417a1edd59934c95c4868f309ce4bd3a9a118aa715175b458b58a35cc1d3e69`  
		Last Modified: Tue, 23 May 2023 01:23:58 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd3977cea96c5c0118f0d34ef8ba6fc71301b74c38d39e7f15f7dcdb69e1121`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54725b68c251ce31613b171528908d72d35d3215608b6f432106bd0c89fd09d`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fd6daf68cdb9ac02732b4bc36377df7d2f63dbd5895badf87cb752e4e45b9a`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.5 MB (16478754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420f8ee3234484fb8f90ced11de46a4b0a8b7fc3cb5f780d1afec5a5de6e0140`  
		Last Modified: Tue, 23 May 2023 01:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d4770e7ab12298d99f71bed561ebf178867b7334ce2af75f237a87075e2f0c`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e907c88699d119d767495b663709d88859d0b84f2a185720f0d165d1571ba`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c95f872c776b4819132fef9832663b2a016e299293b42dae162232eb0956b`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.9 MB (16855888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:17719a45a40b20e31856f9d0018b74309c2ed9bcee055a8720da3bcc9d2ad23d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123215918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3985a943db5c8a91e7819b97867bea926b75f762728894aed317d8851153720f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:26:29 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:26:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:27:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:20:11 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:21:24 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:21:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:21:25 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:21:26 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:22:38 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470efce6095b6077dfd4d6bac6f6e2010f4d5bcdf636e954d0c3e9051baa7a30`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf94d195dbf8bcb75f6433208dda2b0af64c556bf5eed006468d61cccf49971`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f57c72aed2637dc5fc359ff575642812168a390b96d73791c2e00a8aa6c341`  
		Last Modified: Wed, 10 May 2023 07:12:25 GMT  
		Size: 17.3 MB (17330027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e8210888899a756f382a39956b49d936c3b3cc971c774ce106ea7c8ba79242`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761df73e02dadef61574b35ea93d0e12a71dddedfc2dd753cd779a11357c70`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d36348f928d37d3f3e668f8e40784a2d752409a2ab7d5ede9ec734c9d3e42dc`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e6a84fd41f60c1e053b947d5c121e87c9470ad2286b9da138f18743834c865`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.5 MB (16508243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2e0d76930bfb9e698b63a3a4c38d6e31a80d1885e764818ab2d3f7c6fd52b6`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1a0bf4e1377e52d886720ca9ed0a40b713374b1199aded6392ccb26454da12`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c690caa81cfd8344dfa4e473cc140c0052d2c5089c7a3f44c2b0c22ac146e29`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7120d2bb370c638876227ff5daaf5733d38f7bd0ce70787c17036c82d3ab1b94`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.9 MB (16878148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-windowsservercore-1809`

```console
$ docker pull docker@sha256:b76a54c14230c028a765839be85ba9f81c771ffa41f2daee9839abaf48d00c66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `docker:23.0.6-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:17719a45a40b20e31856f9d0018b74309c2ed9bcee055a8720da3bcc9d2ad23d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123215918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3985a943db5c8a91e7819b97867bea926b75f762728894aed317d8851153720f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:26:29 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:26:30 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:27:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:20:11 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:20:12 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:21:24 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:21:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:21:25 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:21:26 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:22:38 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470efce6095b6077dfd4d6bac6f6e2010f4d5bcdf636e954d0c3e9051baa7a30`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf94d195dbf8bcb75f6433208dda2b0af64c556bf5eed006468d61cccf49971`  
		Last Modified: Wed, 10 May 2023 07:12:22 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f57c72aed2637dc5fc359ff575642812168a390b96d73791c2e00a8aa6c341`  
		Last Modified: Wed, 10 May 2023 07:12:25 GMT  
		Size: 17.3 MB (17330027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e8210888899a756f382a39956b49d936c3b3cc971c774ce106ea7c8ba79242`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761df73e02dadef61574b35ea93d0e12a71dddedfc2dd753cd779a11357c70`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d36348f928d37d3f3e668f8e40784a2d752409a2ab7d5ede9ec734c9d3e42dc`  
		Last Modified: Tue, 23 May 2023 01:24:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e6a84fd41f60c1e053b947d5c121e87c9470ad2286b9da138f18743834c865`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.5 MB (16508243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2e0d76930bfb9e698b63a3a4c38d6e31a80d1885e764818ab2d3f7c6fd52b6`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1a0bf4e1377e52d886720ca9ed0a40b713374b1199aded6392ccb26454da12`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c690caa81cfd8344dfa4e473cc140c0052d2c5089c7a3f44c2b0c22ac146e29`  
		Last Modified: Tue, 23 May 2023 01:24:12 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7120d2bb370c638876227ff5daaf5733d38f7bd0ce70787c17036c82d3ab1b94`  
		Last Modified: Tue, 23 May 2023 01:24:16 GMT  
		Size: 16.9 MB (16878148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:dedc3189f736ae43f2abc035c0d9df0ac5279c4fef6e0b8816359c4936943f8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `docker:23.0.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:364433d2b1bee777551a4b6779b0dd8b8132b1fccf3134e4d32a84a37c5c7cc3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826092276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b29bc2769bda71a53814c9ccc2383659cb031973e0c33db6abe1d6784310f5d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 03:24:47 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 10 May 2023 03:24:48 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Wed, 10 May 2023 03:25:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:18:58 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:18:59 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:19:27 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:19:28 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:19:29 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:19:55 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e927fbd88402bacc902c2a4593f281068b2a6657c7f8b4e53ac01f8e636901`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165e88795de1230f78ac3b0186a534bd16fad90474fddb00254443f5440c8c65`  
		Last Modified: Wed, 10 May 2023 07:12:02 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438806a743132696d59ff6500d80c1c45b0742da1613dbde135436ef14f725af`  
		Last Modified: Wed, 10 May 2023 07:12:05 GMT  
		Size: 17.3 MB (17316446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417a1edd59934c95c4868f309ce4bd3a9a118aa715175b458b58a35cc1d3e69`  
		Last Modified: Tue, 23 May 2023 01:23:58 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd3977cea96c5c0118f0d34ef8ba6fc71301b74c38d39e7f15f7dcdb69e1121`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54725b68c251ce31613b171528908d72d35d3215608b6f432106bd0c89fd09d`  
		Last Modified: Tue, 23 May 2023 01:23:57 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fd6daf68cdb9ac02732b4bc36377df7d2f63dbd5895badf87cb752e4e45b9a`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.5 MB (16478754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420f8ee3234484fb8f90ced11de46a4b0a8b7fc3cb5f780d1afec5a5de6e0140`  
		Last Modified: Tue, 23 May 2023 01:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d4770e7ab12298d99f71bed561ebf178867b7334ce2af75f237a87075e2f0c`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e907c88699d119d767495b663709d88859d0b84f2a185720f0d165d1571ba`  
		Last Modified: Tue, 23 May 2023 01:23:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c95f872c776b4819132fef9832663b2a016e299293b42dae162232eb0956b`  
		Last Modified: Tue, 23 May 2023 01:24:00 GMT  
		Size: 16.9 MB (16855888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24`

```console
$ docker pull docker@sha256:99f37b72d498f19dcb9473b3e6dc58b7009bff129fb96bfa096e1b3b080b3df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24` - linux; amd64

```console
$ docker pull docker@sha256:22679c5c3a1967133f1e817c3ba187024375205d1ef084be7aecf6b0d4599c99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115370841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d614d42cf981bd9981fad62de07de3687a1076092a884c394fc5c7ad5d92dbb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:68bc5a121fb395329f577979d3dc87ba524bf0eb6c19523f69f7480d432dff05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106800843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9daef13c2cca5e99754957193975aeba73cb261d2e05b37a8480040cdb5905a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-cli`

```console
$ docker pull docker@sha256:b5c62557d265b22e064f1f7f50d7e4c108ed3660fed2b7a6896f76d0d7b191a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24-cli` - linux; amd64

```console
$ docker pull docker@sha256:9ae670d0f572c933e1140f2bd9f9d4826f8fd95c8ad6f4300714d9b011ca0c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54192095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:909a92cc2c6fac6442505f59d3a12243c8ab83fd02d4de9e6daa17ffb8fd3d21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:92adf22920d3e3c47ab67aa845e4cd979ede76f28200d84135753a96927c47c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50095084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce031b062a3757f551ea1bac26acc62a14aa9bfd14fbc27dca1af0335396cdc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-dind`

```console
$ docker pull docker@sha256:99f37b72d498f19dcb9473b3e6dc58b7009bff129fb96bfa096e1b3b080b3df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24-dind` - linux; amd64

```console
$ docker pull docker@sha256:22679c5c3a1967133f1e817c3ba187024375205d1ef084be7aecf6b0d4599c99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115370841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d614d42cf981bd9981fad62de07de3687a1076092a884c394fc5c7ad5d92dbb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:68bc5a121fb395329f577979d3dc87ba524bf0eb6c19523f69f7480d432dff05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106800843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9daef13c2cca5e99754957193975aeba73cb261d2e05b37a8480040cdb5905a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-dind-rootless`

```console
$ docker pull docker@sha256:1e1e1c1f616b3550d969aaa5327b6cf10682164ce795ab5a445fe5eade17fb04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:1c01c9222da337e3920330c55c8c4c0bfb1b222111a3ab0b6dbb1fec1d59f15e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137383026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3977335037be4ce3015b34eeac21c1dcc6b77e8037b67b5d45470c07f4acb7ac`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:05:39 GMT
USER rootless
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7b7a8d521f676ac3ddc012e4682ee16b17f01938e01cb7bb9992b62b01693`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 1.4 MB (1362349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef042b65f646f14101f1b532c3455eb6c6075ab83e8417f95777c8894773785f`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b58cb1d6879da102fdf09ab6a7aaa4b22b4dfdea6ee5f1e53f4b2c6f30d4db`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f56120e82417552006ed7bb211c298a839bde5ae959167128d388a92e520d`  
		Last Modified: Tue, 23 May 2023 01:29:55 GMT  
		Size: 20.6 MB (20648097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2565fe7f5be844e967124b1edc8f9c0545a94339785a36562602712d9b626b32`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:334a575e406465fb993bab4738690c3a0da6d01c85393b104bf2cdb8ab1ac888
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130663068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ebf9b2706719fa1dd4c402a7d1caacba98bf6e3de1ebc61d8b75e79e4d9059`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:05:39 GMT
USER rootless
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61e30747408a11549260b7396bfa879196eeef18215a312a5a1d43bc087563`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 1.4 MB (1413219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc11e300f1422ff6fbdfdc33b9c3277961ba99dcd57c58fe58d0e5bfa9586593`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a68a49501432b599714b542dd84b7553d914097a3750fd7c3a92a32a7ef51`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e554ae37c29650c4d40d2cc2cf6c322e6234b696c8ba25ed50dc7f4c1ef88`  
		Last Modified: Tue, 23 May 2023 00:41:16 GMT  
		Size: 22.4 MB (22447267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3d00c33b848f221e69fe7b5d17bb4a4b586f97ee0175fc127b6e265a56b46`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-git`

```console
$ docker pull docker@sha256:3975ebfa0bb9c77959e3a2c5d77c1587d6a9f06f65da15e24ab21a071d0750e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24-git` - linux; amd64

```console
$ docker pull docker@sha256:6c972e42fa691d9aed7f48482ca78bf29a060f70494bc9b84bf97afe98da4a40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120307052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa1be8f7f210ad03dffbd6ed366338375ec7bd19acd467971ccd4f05384a06e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45fe0bb60df432a7b087e8c9788c18352055837f1dac75b8416ba60629e4354`  
		Last Modified: Tue, 23 May 2023 01:30:09 GMT  
		Size: 4.9 MB (4936211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:33654f749f914498fb2d8c7f681bdb6823b10ac29b2d211b2ece7e786c6c5abe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341cf752342f4903ce6251f07fdd0ca7e67edc19d821611a6a0bb7a81af4d75e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe1c11a5fa1611e5c44e8d667dcfaa36d9b61136349fdca93f5d7d101e36e38`  
		Last Modified: Tue, 23 May 2023 00:41:30 GMT  
		Size: 5.0 MB (5021969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-windowsservercore`

```console
$ docker pull docker@sha256:1d78f6f0a1ecccf970857572dd6a514e8b3ca8ed3450bd42fe76c7bd32d07ab5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `docker:24-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:a990a4f1fffd513fbb0354826eadedc7162904ed5657e0c1677ffe9328a21d5a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826215665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d92f7a694bb5fff886f0f4c376f2632727e68fd5519870bac08797533cdeda`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:15:04 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:15:05 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:15:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:02 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:15:03 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:15:04 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:15:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:15:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:16:01 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc754386dea5721554d4320fc581c4e83b653a954952515a5aaa5b52dbd4a574`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b527d00cccb03bd30e17bc04e2372d8e5e57fa44fef30266f060c71f63954`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b76accff37953841e1a00f8907a6abdb623e594e68784f932194d7dfad253`  
		Last Modified: Sat, 20 May 2023 02:15:37 GMT  
		Size: 17.4 MB (17442937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22811ed980a194a32b7f991db121c816d41a2f9ed42421253cedc81b7471ff3d`  
		Last Modified: Tue, 23 May 2023 01:23:21 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13423d9367df853b5b71f649a9ed032b074a113032b4145d15c95869e75bfb74`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9551a597f4845d99fe72d1e9855c2c500c5b8df9ca518a1b4ae0bba59bfe28e8`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625d6a58bb92a0b4248d9836bd902fcffcb7dabf30eb4348c40bf552180f063`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.5 MB (16475300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f649be4312f54b778373c6ad7f856dddae81b7606fec596f2d6bdebf2c4af7c`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ba2e268969eb8e02fd84e72477996f5668f50a5e03966f602a10cebc38fd6`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c454de9855bf96eb772c11c0664f35a5bcb0de98bbfd3cd08913f189e59c9c8e`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e2c3d7edc4f0e36805d2852db1bc041000d9ad6ba91b96e50d0b85e7764bde`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.9 MB (16856366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:821ae435c38f25d20ea96be3fb194295c58e6b181820c159efcee3f7328bcd53
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123344587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977d42b593cdab1bfe7f8f2a56ace414efbb193e061ab8209ef70e26ca07e7c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:16:15 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:16:16 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:16:17 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:17:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:17:31 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:17:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:17:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:18:44 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a611bc5b3f6eb35800b14c663f2bfcabfecead6ab4a7216fdcdd4081fb9354f5`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3413fb41d65eaa6e11c31655a25a3dafe7a78a2dcfd9b3b9fb712a200e3cce35`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514407c6475908d93aa56dbf8187ffeeb77b8f66de5e83d217200d7a095dfd9a`  
		Last Modified: Sat, 20 May 2023 02:15:58 GMT  
		Size: 17.5 MB (17474830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53167037e2315751aa8e06465eb799d83c1c6939106c827b272c72578699db6c`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f3a8c479644ca63d52ed172ebc922c3f5a56e4ad88332a3ba3a052839360f`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba00296054cd4a13b7ff959420b66d4e86fa2aa8bdafe0f01cb3f91f609136a`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b204fbf0455b0452d3b0c4a21b6e15d7a5c3b5a9d1f34e81be67f5b11b506c`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.5 MB (16496465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baa660d406b62bed7d4ce723b0fcb3e855790ad0d2b8ff95533109ae3254855`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d6ab177afed853c8629165517469a6c210f96ba94a6a6a2384d40713f08c8`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9ce3c49056e3bb078dd3ba8f72e29bfa9027d41ecb171713b3ba73818f5ab5`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323c62c8c1f681922488afd95e44ecac331015a691d7c573d23d28099689cd`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.9 MB (16873896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-windowsservercore-1809`

```console
$ docker pull docker@sha256:d06a2a062d39be1fc5ea2e3ae234d423e521f738b531890d7e1a2dfbfe07580c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `docker:24-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:821ae435c38f25d20ea96be3fb194295c58e6b181820c159efcee3f7328bcd53
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123344587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977d42b593cdab1bfe7f8f2a56ace414efbb193e061ab8209ef70e26ca07e7c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:16:15 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:16:16 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:16:17 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:17:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:17:31 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:17:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:17:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:18:44 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a611bc5b3f6eb35800b14c663f2bfcabfecead6ab4a7216fdcdd4081fb9354f5`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3413fb41d65eaa6e11c31655a25a3dafe7a78a2dcfd9b3b9fb712a200e3cce35`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514407c6475908d93aa56dbf8187ffeeb77b8f66de5e83d217200d7a095dfd9a`  
		Last Modified: Sat, 20 May 2023 02:15:58 GMT  
		Size: 17.5 MB (17474830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53167037e2315751aa8e06465eb799d83c1c6939106c827b272c72578699db6c`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f3a8c479644ca63d52ed172ebc922c3f5a56e4ad88332a3ba3a052839360f`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba00296054cd4a13b7ff959420b66d4e86fa2aa8bdafe0f01cb3f91f609136a`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b204fbf0455b0452d3b0c4a21b6e15d7a5c3b5a9d1f34e81be67f5b11b506c`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.5 MB (16496465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baa660d406b62bed7d4ce723b0fcb3e855790ad0d2b8ff95533109ae3254855`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d6ab177afed853c8629165517469a6c210f96ba94a6a6a2384d40713f08c8`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9ce3c49056e3bb078dd3ba8f72e29bfa9027d41ecb171713b3ba73818f5ab5`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323c62c8c1f681922488afd95e44ecac331015a691d7c573d23d28099689cd`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.9 MB (16873896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:883ce580efdc7b6813465965104378d5145e190bfd7a5b4481ef6e81b03c66da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `docker:24-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:a990a4f1fffd513fbb0354826eadedc7162904ed5657e0c1677ffe9328a21d5a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826215665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d92f7a694bb5fff886f0f4c376f2632727e68fd5519870bac08797533cdeda`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:15:04 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:15:05 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:15:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:02 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:15:03 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:15:04 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:15:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:15:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:16:01 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc754386dea5721554d4320fc581c4e83b653a954952515a5aaa5b52dbd4a574`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b527d00cccb03bd30e17bc04e2372d8e5e57fa44fef30266f060c71f63954`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b76accff37953841e1a00f8907a6abdb623e594e68784f932194d7dfad253`  
		Last Modified: Sat, 20 May 2023 02:15:37 GMT  
		Size: 17.4 MB (17442937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22811ed980a194a32b7f991db121c816d41a2f9ed42421253cedc81b7471ff3d`  
		Last Modified: Tue, 23 May 2023 01:23:21 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13423d9367df853b5b71f649a9ed032b074a113032b4145d15c95869e75bfb74`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9551a597f4845d99fe72d1e9855c2c500c5b8df9ca518a1b4ae0bba59bfe28e8`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625d6a58bb92a0b4248d9836bd902fcffcb7dabf30eb4348c40bf552180f063`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.5 MB (16475300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f649be4312f54b778373c6ad7f856dddae81b7606fec596f2d6bdebf2c4af7c`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ba2e268969eb8e02fd84e72477996f5668f50a5e03966f602a10cebc38fd6`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c454de9855bf96eb772c11c0664f35a5bcb0de98bbfd3cd08913f189e59c9c8e`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e2c3d7edc4f0e36805d2852db1bc041000d9ad6ba91b96e50d0b85e7764bde`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.9 MB (16856366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0`

```console
$ docker pull docker@sha256:99f37b72d498f19dcb9473b3e6dc58b7009bff129fb96bfa096e1b3b080b3df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0` - linux; amd64

```console
$ docker pull docker@sha256:22679c5c3a1967133f1e817c3ba187024375205d1ef084be7aecf6b0d4599c99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115370841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d614d42cf981bd9981fad62de07de3687a1076092a884c394fc5c7ad5d92dbb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:68bc5a121fb395329f577979d3dc87ba524bf0eb6c19523f69f7480d432dff05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106800843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9daef13c2cca5e99754957193975aeba73cb261d2e05b37a8480040cdb5905a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-cli`

```console
$ docker pull docker@sha256:b5c62557d265b22e064f1f7f50d7e4c108ed3660fed2b7a6896f76d0d7b191a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0-cli` - linux; amd64

```console
$ docker pull docker@sha256:9ae670d0f572c933e1140f2bd9f9d4826f8fd95c8ad6f4300714d9b011ca0c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54192095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:909a92cc2c6fac6442505f59d3a12243c8ab83fd02d4de9e6daa17ffb8fd3d21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:92adf22920d3e3c47ab67aa845e4cd979ede76f28200d84135753a96927c47c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50095084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce031b062a3757f551ea1bac26acc62a14aa9bfd14fbc27dca1af0335396cdc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-dind`

```console
$ docker pull docker@sha256:99f37b72d498f19dcb9473b3e6dc58b7009bff129fb96bfa096e1b3b080b3df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:22679c5c3a1967133f1e817c3ba187024375205d1ef084be7aecf6b0d4599c99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115370841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d614d42cf981bd9981fad62de07de3687a1076092a884c394fc5c7ad5d92dbb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:68bc5a121fb395329f577979d3dc87ba524bf0eb6c19523f69f7480d432dff05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106800843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9daef13c2cca5e99754957193975aeba73cb261d2e05b37a8480040cdb5905a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-dind-rootless`

```console
$ docker pull docker@sha256:1e1e1c1f616b3550d969aaa5327b6cf10682164ce795ab5a445fe5eade17fb04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:1c01c9222da337e3920330c55c8c4c0bfb1b222111a3ab0b6dbb1fec1d59f15e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137383026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3977335037be4ce3015b34eeac21c1dcc6b77e8037b67b5d45470c07f4acb7ac`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:05:39 GMT
USER rootless
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7b7a8d521f676ac3ddc012e4682ee16b17f01938e01cb7bb9992b62b01693`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 1.4 MB (1362349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef042b65f646f14101f1b532c3455eb6c6075ab83e8417f95777c8894773785f`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b58cb1d6879da102fdf09ab6a7aaa4b22b4dfdea6ee5f1e53f4b2c6f30d4db`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f56120e82417552006ed7bb211c298a839bde5ae959167128d388a92e520d`  
		Last Modified: Tue, 23 May 2023 01:29:55 GMT  
		Size: 20.6 MB (20648097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2565fe7f5be844e967124b1edc8f9c0545a94339785a36562602712d9b626b32`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:334a575e406465fb993bab4738690c3a0da6d01c85393b104bf2cdb8ab1ac888
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130663068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ebf9b2706719fa1dd4c402a7d1caacba98bf6e3de1ebc61d8b75e79e4d9059`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:05:39 GMT
USER rootless
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61e30747408a11549260b7396bfa879196eeef18215a312a5a1d43bc087563`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 1.4 MB (1413219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc11e300f1422ff6fbdfdc33b9c3277961ba99dcd57c58fe58d0e5bfa9586593`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a68a49501432b599714b542dd84b7553d914097a3750fd7c3a92a32a7ef51`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e554ae37c29650c4d40d2cc2cf6c322e6234b696c8ba25ed50dc7f4c1ef88`  
		Last Modified: Tue, 23 May 2023 00:41:16 GMT  
		Size: 22.4 MB (22447267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3d00c33b848f221e69fe7b5d17bb4a4b586f97ee0175fc127b6e265a56b46`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-git`

```console
$ docker pull docker@sha256:3975ebfa0bb9c77959e3a2c5d77c1587d6a9f06f65da15e24ab21a071d0750e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0-git` - linux; amd64

```console
$ docker pull docker@sha256:6c972e42fa691d9aed7f48482ca78bf29a060f70494bc9b84bf97afe98da4a40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120307052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa1be8f7f210ad03dffbd6ed366338375ec7bd19acd467971ccd4f05384a06e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45fe0bb60df432a7b087e8c9788c18352055837f1dac75b8416ba60629e4354`  
		Last Modified: Tue, 23 May 2023 01:30:09 GMT  
		Size: 4.9 MB (4936211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:33654f749f914498fb2d8c7f681bdb6823b10ac29b2d211b2ece7e786c6c5abe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341cf752342f4903ce6251f07fdd0ca7e67edc19d821611a6a0bb7a81af4d75e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe1c11a5fa1611e5c44e8d667dcfaa36d9b61136349fdca93f5d7d101e36e38`  
		Last Modified: Tue, 23 May 2023 00:41:30 GMT  
		Size: 5.0 MB (5021969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-windowsservercore`

```console
$ docker pull docker@sha256:1d78f6f0a1ecccf970857572dd6a514e8b3ca8ed3450bd42fe76c7bd32d07ab5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `docker:24.0-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:a990a4f1fffd513fbb0354826eadedc7162904ed5657e0c1677ffe9328a21d5a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826215665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d92f7a694bb5fff886f0f4c376f2632727e68fd5519870bac08797533cdeda`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:15:04 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:15:05 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:15:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:02 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:15:03 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:15:04 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:15:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:15:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:16:01 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc754386dea5721554d4320fc581c4e83b653a954952515a5aaa5b52dbd4a574`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b527d00cccb03bd30e17bc04e2372d8e5e57fa44fef30266f060c71f63954`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b76accff37953841e1a00f8907a6abdb623e594e68784f932194d7dfad253`  
		Last Modified: Sat, 20 May 2023 02:15:37 GMT  
		Size: 17.4 MB (17442937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22811ed980a194a32b7f991db121c816d41a2f9ed42421253cedc81b7471ff3d`  
		Last Modified: Tue, 23 May 2023 01:23:21 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13423d9367df853b5b71f649a9ed032b074a113032b4145d15c95869e75bfb74`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9551a597f4845d99fe72d1e9855c2c500c5b8df9ca518a1b4ae0bba59bfe28e8`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625d6a58bb92a0b4248d9836bd902fcffcb7dabf30eb4348c40bf552180f063`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.5 MB (16475300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f649be4312f54b778373c6ad7f856dddae81b7606fec596f2d6bdebf2c4af7c`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ba2e268969eb8e02fd84e72477996f5668f50a5e03966f602a10cebc38fd6`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c454de9855bf96eb772c11c0664f35a5bcb0de98bbfd3cd08913f189e59c9c8e`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e2c3d7edc4f0e36805d2852db1bc041000d9ad6ba91b96e50d0b85e7764bde`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.9 MB (16856366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:821ae435c38f25d20ea96be3fb194295c58e6b181820c159efcee3f7328bcd53
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123344587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977d42b593cdab1bfe7f8f2a56ace414efbb193e061ab8209ef70e26ca07e7c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:16:15 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:16:16 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:16:17 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:17:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:17:31 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:17:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:17:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:18:44 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a611bc5b3f6eb35800b14c663f2bfcabfecead6ab4a7216fdcdd4081fb9354f5`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3413fb41d65eaa6e11c31655a25a3dafe7a78a2dcfd9b3b9fb712a200e3cce35`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514407c6475908d93aa56dbf8187ffeeb77b8f66de5e83d217200d7a095dfd9a`  
		Last Modified: Sat, 20 May 2023 02:15:58 GMT  
		Size: 17.5 MB (17474830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53167037e2315751aa8e06465eb799d83c1c6939106c827b272c72578699db6c`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f3a8c479644ca63d52ed172ebc922c3f5a56e4ad88332a3ba3a052839360f`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba00296054cd4a13b7ff959420b66d4e86fa2aa8bdafe0f01cb3f91f609136a`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b204fbf0455b0452d3b0c4a21b6e15d7a5c3b5a9d1f34e81be67f5b11b506c`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.5 MB (16496465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baa660d406b62bed7d4ce723b0fcb3e855790ad0d2b8ff95533109ae3254855`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d6ab177afed853c8629165517469a6c210f96ba94a6a6a2384d40713f08c8`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9ce3c49056e3bb078dd3ba8f72e29bfa9027d41ecb171713b3ba73818f5ab5`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323c62c8c1f681922488afd95e44ecac331015a691d7c573d23d28099689cd`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.9 MB (16873896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-windowsservercore-1809`

```console
$ docker pull docker@sha256:d06a2a062d39be1fc5ea2e3ae234d423e521f738b531890d7e1a2dfbfe07580c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `docker:24.0-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:821ae435c38f25d20ea96be3fb194295c58e6b181820c159efcee3f7328bcd53
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123344587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977d42b593cdab1bfe7f8f2a56ace414efbb193e061ab8209ef70e26ca07e7c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:16:15 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:16:16 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:16:17 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:17:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:17:31 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:17:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:17:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:18:44 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a611bc5b3f6eb35800b14c663f2bfcabfecead6ab4a7216fdcdd4081fb9354f5`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3413fb41d65eaa6e11c31655a25a3dafe7a78a2dcfd9b3b9fb712a200e3cce35`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514407c6475908d93aa56dbf8187ffeeb77b8f66de5e83d217200d7a095dfd9a`  
		Last Modified: Sat, 20 May 2023 02:15:58 GMT  
		Size: 17.5 MB (17474830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53167037e2315751aa8e06465eb799d83c1c6939106c827b272c72578699db6c`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f3a8c479644ca63d52ed172ebc922c3f5a56e4ad88332a3ba3a052839360f`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba00296054cd4a13b7ff959420b66d4e86fa2aa8bdafe0f01cb3f91f609136a`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b204fbf0455b0452d3b0c4a21b6e15d7a5c3b5a9d1f34e81be67f5b11b506c`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.5 MB (16496465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baa660d406b62bed7d4ce723b0fcb3e855790ad0d2b8ff95533109ae3254855`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d6ab177afed853c8629165517469a6c210f96ba94a6a6a2384d40713f08c8`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9ce3c49056e3bb078dd3ba8f72e29bfa9027d41ecb171713b3ba73818f5ab5`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323c62c8c1f681922488afd95e44ecac331015a691d7c573d23d28099689cd`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.9 MB (16873896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:883ce580efdc7b6813465965104378d5145e190bfd7a5b4481ef6e81b03c66da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `docker:24.0-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:a990a4f1fffd513fbb0354826eadedc7162904ed5657e0c1677ffe9328a21d5a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826215665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d92f7a694bb5fff886f0f4c376f2632727e68fd5519870bac08797533cdeda`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:15:04 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:15:05 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:15:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:02 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:15:03 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:15:04 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:15:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:15:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:16:01 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc754386dea5721554d4320fc581c4e83b653a954952515a5aaa5b52dbd4a574`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b527d00cccb03bd30e17bc04e2372d8e5e57fa44fef30266f060c71f63954`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b76accff37953841e1a00f8907a6abdb623e594e68784f932194d7dfad253`  
		Last Modified: Sat, 20 May 2023 02:15:37 GMT  
		Size: 17.4 MB (17442937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22811ed980a194a32b7f991db121c816d41a2f9ed42421253cedc81b7471ff3d`  
		Last Modified: Tue, 23 May 2023 01:23:21 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13423d9367df853b5b71f649a9ed032b074a113032b4145d15c95869e75bfb74`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9551a597f4845d99fe72d1e9855c2c500c5b8df9ca518a1b4ae0bba59bfe28e8`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625d6a58bb92a0b4248d9836bd902fcffcb7dabf30eb4348c40bf552180f063`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.5 MB (16475300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f649be4312f54b778373c6ad7f856dddae81b7606fec596f2d6bdebf2c4af7c`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ba2e268969eb8e02fd84e72477996f5668f50a5e03966f602a10cebc38fd6`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c454de9855bf96eb772c11c0664f35a5bcb0de98bbfd3cd08913f189e59c9c8e`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e2c3d7edc4f0e36805d2852db1bc041000d9ad6ba91b96e50d0b85e7764bde`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.9 MB (16856366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0.2`

**does not exist** (yet?)

## `docker:24.0.2-alpine3.18`

**does not exist** (yet?)

## `docker:24.0.2-cli`

**does not exist** (yet?)

## `docker:24.0.2-cli-alpine3.18`

**does not exist** (yet?)

## `docker:24.0.2-dind`

**does not exist** (yet?)

## `docker:24.0.2-dind-alpine3.18`

**does not exist** (yet?)

## `docker:24.0.2-dind-rootless`

**does not exist** (yet?)

## `docker:24.0.2-git`

**does not exist** (yet?)

## `docker:24.0.2-windowsservercore`

**does not exist** (yet?)

## `docker:24.0.2-windowsservercore-1809`

**does not exist** (yet?)

## `docker:24.0.2-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `docker:cli`

```console
$ docker pull docker@sha256:b5c62557d265b22e064f1f7f50d7e4c108ed3660fed2b7a6896f76d0d7b191a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:9ae670d0f572c933e1140f2bd9f9d4826f8fd95c8ad6f4300714d9b011ca0c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54192095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:909a92cc2c6fac6442505f59d3a12243c8ab83fd02d4de9e6daa17ffb8fd3d21`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:92adf22920d3e3c47ab67aa845e4cd979ede76f28200d84135753a96927c47c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50095084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce031b062a3757f551ea1bac26acc62a14aa9bfd14fbc27dca1af0335396cdc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:99f37b72d498f19dcb9473b3e6dc58b7009bff129fb96bfa096e1b3b080b3df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:22679c5c3a1967133f1e817c3ba187024375205d1ef084be7aecf6b0d4599c99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115370841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d614d42cf981bd9981fad62de07de3687a1076092a884c394fc5c7ad5d92dbb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:68bc5a121fb395329f577979d3dc87ba524bf0eb6c19523f69f7480d432dff05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106800843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9daef13c2cca5e99754957193975aeba73cb261d2e05b37a8480040cdb5905a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:1e1e1c1f616b3550d969aaa5327b6cf10682164ce795ab5a445fe5eade17fb04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:1c01c9222da337e3920330c55c8c4c0bfb1b222111a3ab0b6dbb1fec1d59f15e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137383026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3977335037be4ce3015b34eeac21c1dcc6b77e8037b67b5d45470c07f4acb7ac`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:05:39 GMT
USER rootless
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7b7a8d521f676ac3ddc012e4682ee16b17f01938e01cb7bb9992b62b01693`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 1.4 MB (1362349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef042b65f646f14101f1b532c3455eb6c6075ab83e8417f95777c8894773785f`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b58cb1d6879da102fdf09ab6a7aaa4b22b4dfdea6ee5f1e53f4b2c6f30d4db`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f56120e82417552006ed7bb211c298a839bde5ae959167128d388a92e520d`  
		Last Modified: Tue, 23 May 2023 01:29:55 GMT  
		Size: 20.6 MB (20648097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2565fe7f5be844e967124b1edc8f9c0545a94339785a36562602712d9b626b32`  
		Last Modified: Tue, 23 May 2023 01:29:52 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:334a575e406465fb993bab4738690c3a0da6d01c85393b104bf2cdb8ab1ac888
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130663068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95ebf9b2706719fa1dd4c402a7d1caacba98bf6e3de1ebc61d8b75e79e4d9059`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 22 May 2023 23:05:39 GMT
USER rootless
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61e30747408a11549260b7396bfa879196eeef18215a312a5a1d43bc087563`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 1.4 MB (1413219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc11e300f1422ff6fbdfdc33b9c3277961ba99dcd57c58fe58d0e5bfa9586593`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a68a49501432b599714b542dd84b7553d914097a3750fd7c3a92a32a7ef51`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3e554ae37c29650c4d40d2cc2cf6c322e6234b696c8ba25ed50dc7f4c1ef88`  
		Last Modified: Tue, 23 May 2023 00:41:16 GMT  
		Size: 22.4 MB (22447267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3d00c33b848f221e69fe7b5d17bb4a4b586f97ee0175fc127b6e265a56b46`  
		Last Modified: Tue, 23 May 2023 00:41:13 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:3975ebfa0bb9c77959e3a2c5d77c1587d6a9f06f65da15e24ab21a071d0750e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:6c972e42fa691d9aed7f48482ca78bf29a060f70494bc9b84bf97afe98da4a40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120307052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa1be8f7f210ad03dffbd6ed366338375ec7bd19acd467971ccd4f05384a06e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45fe0bb60df432a7b087e8c9788c18352055837f1dac75b8416ba60629e4354`  
		Last Modified: Tue, 23 May 2023 01:30:09 GMT  
		Size: 4.9 MB (4936211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:33654f749f914498fb2d8c7f681bdb6823b10ac29b2d211b2ece7e786c6c5abe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341cf752342f4903ce6251f07fdd0ca7e67edc19d821611a6a0bb7a81af4d75e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
# Mon, 22 May 2023 23:05:39 GMT
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe1c11a5fa1611e5c44e8d667dcfaa36d9b61136349fdca93f5d7d101e36e38`  
		Last Modified: Tue, 23 May 2023 00:41:30 GMT  
		Size: 5.0 MB (5021969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:99f37b72d498f19dcb9473b3e6dc58b7009bff129fb96bfa096e1b3b080b3df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:22679c5c3a1967133f1e817c3ba187024375205d1ef084be7aecf6b0d4599c99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115370841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d614d42cf981bd9981fad62de07de3687a1076092a884c394fc5c7ad5d92dbb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:75039dcfa57a7b4e9405dbd4aa6d212ea4202c813e54a727ccd1e54d545afc28`  
		Last Modified: Sat, 20 May 2023 00:20:31 GMT  
		Size: 16.4 MB (16376152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867a08cc62aba90b08b1da3ef9ec49bc28d26e61fe5d11dd876855dc8e85b2a`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.0 MB (16003304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c97d93d5c3e3a47e69b213f3b39c2593c7c49f4c0b49e79f2a34bceab398`  
		Last Modified: Tue, 23 May 2023 01:29:04 GMT  
		Size: 16.4 MB (16398969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5893dfdf02699e20fb56be75a304867d4fec743b9eac91f0a063a5cb09cdfe24`  
		Last Modified: Tue, 23 May 2023 01:29:01 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd0f5addfbf9728ca04b0dea382dc8e4b950648089413635c64277f0bfc44b2`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3364461d2a2d8174b06d66820c387e9f5e2b1d551114d865ee58292a6313f81`  
		Last Modified: Tue, 23 May 2023 01:29:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63b390fabeb872b583734d1517576a6318107fc70d9c713765732d33dda261`  
		Last Modified: Tue, 23 May 2023 01:29:19 GMT  
		Size: 7.0 MB (7025225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a256d559fb8adfa83be30ad368d83212bd98330aa37b171415be89ea9b0d1`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36549cf8e4b803d03ea7f6c3926d54f3479a5591686a4f60437c5e381d00d22`  
		Last Modified: Tue, 23 May 2023 01:29:25 GMT  
		Size: 54.1 MB (54148363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135f01648aa4bd90a15ab5392d49ed1504f2927999f4fae1a947ac73a0bc0e28`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9804e6a84f9c66c5cf3770c679b656ff06839fb9f5b809483e821f128c06c17`  
		Last Modified: Tue, 23 May 2023 01:29:18 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:68bc5a121fb395329f577979d3dc87ba524bf0eb6c19523f69f7480d432dff05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106800843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9daef13c2cca5e99754957193975aeba73cb261d2e05b37a8480040cdb5905a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_VERSION=24.0.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-amd64'; 			sha256='2f1995ee6c4e7d75668ff38242ce3381da71bd30a8ca1f648f077b0a066c742b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v6'; 			sha256='cd8d8b3fe02b07d60d323af27da53c72c35516e7c8a52e649e3a68582e113e76'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm-v7'; 			sha256='a10b60d9c541b30c8f46ed2c8e671c1c775125d6b71ff0b1787204c11ae84ba9'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-arm64'; 			sha256='a60d2dfb46cbe66e7fa75c8fd4fc730bcf052e08b8e236df254c24600db388a9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-ppc64le'; 			sha256='1c1ac2bcad35a7d423e093bceba04e3f0d3f4381e534b64e1fb67e0dc932c973'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-riscv64'; 			sha256='f2da6e8ac73b00bafac1f4ecd76e126e8a3f6740adfcd04fbad0094d30274a55'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.linux-s390x'; 			sha256='9a64f9248a8fa6d5b114d5599018814a1fc950f1910aa73e4fb9d012ca9bcbe6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-x86_64'; 			sha256='b4e6aff14c30f82ce26e94d37686b5598b3f870ce1e053927c853b4f4b128575'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv6'; 			sha256='34430890fe8ab68fe091a2907ebff174d1d6dcfc3d4e87f8c50bb105a2ac8b5f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-armv7'; 			sha256='cced34fc17c3689b5e0760b115ef481014eb004370a7b9380fc25eeef55570bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-aarch64'; 			sha256='6d1784542f74806ef0ed4e798d31c91604453eb06b86448b4c60d7df5d5b7afb'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-ppc64le'; 			sha256='baa21ead951f0b0a0dc191e4dc7718e584961d0fcbb5969004bdcf1950203cde'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-riscv64'; 			sha256='2e84879a8677bcebda18d7772a86fa107f3745ba693f7c9c397b9fede355e3f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-linux-s390x'; 			sha256='e8d5669b5f11212310d080d239348fe293b783c7357bb1085728fbed69e519c9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 22 May 2023 23:05:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD ["sh"]
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 22 May 2023 23:05:39 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 22 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 22 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 22 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Mon, 22 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 22 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 22 May 2023 23:05:39 GMT
CMD []
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
	-	`sha256:2e7805c665c512c9144fc4fa17be125272b027a57c3af9ecc374e51f661e6330`  
		Last Modified: Sat, 20 May 2023 00:40:13 GMT  
		Size: 15.4 MB (15422660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560067f77f099c33ab9ac4d490af6caedf4474196068e213add2a102025646e5`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.4 MB (14442035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87854ced1808bf388bcbd9a9b2a956151473b3a7abcc519ba469e2432b6ebace`  
		Last Modified: Tue, 23 May 2023 00:40:25 GMT  
		Size: 14.9 MB (14861184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb23a4dee6cb394a99b52e73920f116ab1efbe2ed070b1d3d80c9167b87b94ff`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f440641682c4d09e912afe09a756938d740c58674f1a99ca84503b8439cc543`  
		Last Modified: Tue, 23 May 2023 00:40:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5751f9f360d11197a0752125a6dd05fe7a989ef5a2ce837e4b0479183df4f83`  
		Last Modified: Tue, 23 May 2023 00:40:24 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b4d37fd2038b073826db64a8d0f1a310d5ec7d10259855823ad26b153bfc70`  
		Last Modified: Tue, 23 May 2023 00:40:40 GMT  
		Size: 7.2 MB (7245009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b4cd8a6de66ff46630a2f0f8ca847fc8304b51c84de93f8e8367653a12e35`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b8b8583a6ef26d94916f6ed39951bbb2135f9f74acd6aee3d10eec599707e1`  
		Last Modified: Tue, 23 May 2023 00:40:45 GMT  
		Size: 49.5 MB (49455587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5363e21a005c57c15179a087edb9d371ffbe2ade9e13e2750ed85be226541b71`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56ef98c0a7035b1975b506b28b854abd5d38d834f2d40669ee794d747f186e4`  
		Last Modified: Tue, 23 May 2023 00:40:39 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:1d78f6f0a1ecccf970857572dd6a514e8b3ca8ed3450bd42fe76c7bd32d07ab5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `docker:windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:a990a4f1fffd513fbb0354826eadedc7162904ed5657e0c1677ffe9328a21d5a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826215665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d92f7a694bb5fff886f0f4c376f2632727e68fd5519870bac08797533cdeda`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:15:04 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:15:05 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:15:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:02 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:15:03 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:15:04 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:15:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:15:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:16:01 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc754386dea5721554d4320fc581c4e83b653a954952515a5aaa5b52dbd4a574`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b527d00cccb03bd30e17bc04e2372d8e5e57fa44fef30266f060c71f63954`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b76accff37953841e1a00f8907a6abdb623e594e68784f932194d7dfad253`  
		Last Modified: Sat, 20 May 2023 02:15:37 GMT  
		Size: 17.4 MB (17442937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22811ed980a194a32b7f991db121c816d41a2f9ed42421253cedc81b7471ff3d`  
		Last Modified: Tue, 23 May 2023 01:23:21 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13423d9367df853b5b71f649a9ed032b074a113032b4145d15c95869e75bfb74`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9551a597f4845d99fe72d1e9855c2c500c5b8df9ca518a1b4ae0bba59bfe28e8`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625d6a58bb92a0b4248d9836bd902fcffcb7dabf30eb4348c40bf552180f063`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.5 MB (16475300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f649be4312f54b778373c6ad7f856dddae81b7606fec596f2d6bdebf2c4af7c`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ba2e268969eb8e02fd84e72477996f5668f50a5e03966f602a10cebc38fd6`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c454de9855bf96eb772c11c0664f35a5bcb0de98bbfd3cd08913f189e59c9c8e`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e2c3d7edc4f0e36805d2852db1bc041000d9ad6ba91b96e50d0b85e7764bde`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.9 MB (16856366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:821ae435c38f25d20ea96be3fb194295c58e6b181820c159efcee3f7328bcd53
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123344587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977d42b593cdab1bfe7f8f2a56ace414efbb193e061ab8209ef70e26ca07e7c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:16:15 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:16:16 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:16:17 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:17:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:17:31 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:17:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:17:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:18:44 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a611bc5b3f6eb35800b14c663f2bfcabfecead6ab4a7216fdcdd4081fb9354f5`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3413fb41d65eaa6e11c31655a25a3dafe7a78a2dcfd9b3b9fb712a200e3cce35`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514407c6475908d93aa56dbf8187ffeeb77b8f66de5e83d217200d7a095dfd9a`  
		Last Modified: Sat, 20 May 2023 02:15:58 GMT  
		Size: 17.5 MB (17474830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53167037e2315751aa8e06465eb799d83c1c6939106c827b272c72578699db6c`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f3a8c479644ca63d52ed172ebc922c3f5a56e4ad88332a3ba3a052839360f`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba00296054cd4a13b7ff959420b66d4e86fa2aa8bdafe0f01cb3f91f609136a`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b204fbf0455b0452d3b0c4a21b6e15d7a5c3b5a9d1f34e81be67f5b11b506c`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.5 MB (16496465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baa660d406b62bed7d4ce723b0fcb3e855790ad0d2b8ff95533109ae3254855`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d6ab177afed853c8629165517469a6c210f96ba94a6a6a2384d40713f08c8`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9ce3c49056e3bb078dd3ba8f72e29bfa9027d41ecb171713b3ba73818f5ab5`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323c62c8c1f681922488afd95e44ecac331015a691d7c573d23d28099689cd`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.9 MB (16873896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:d06a2a062d39be1fc5ea2e3ae234d423e521f738b531890d7e1a2dfbfe07580c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull docker@sha256:821ae435c38f25d20ea96be3fb194295c58e6b181820c159efcee3f7328bcd53
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2123344587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:977d42b593cdab1bfe7f8f2a56ace414efbb193e061ab8209ef70e26ca07e7c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:16:42 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:16:46 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:18:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:16:15 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:16:16 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:16:17 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:17:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:17:31 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:17:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:17:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:18:44 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a0b27170ed378e5d22763ab388eaf4a9dbd91cb7eaee4cef7d8639a2ff74`  
		Last Modified: Wed, 10 May 2023 07:11:47 GMT  
		Size: 451.5 KB (451506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a611bc5b3f6eb35800b14c663f2bfcabfecead6ab4a7216fdcdd4081fb9354f5`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3413fb41d65eaa6e11c31655a25a3dafe7a78a2dcfd9b3b9fb712a200e3cce35`  
		Last Modified: Sat, 20 May 2023 02:15:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514407c6475908d93aa56dbf8187ffeeb77b8f66de5e83d217200d7a095dfd9a`  
		Last Modified: Sat, 20 May 2023 02:15:58 GMT  
		Size: 17.5 MB (17474830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53167037e2315751aa8e06465eb799d83c1c6939106c827b272c72578699db6c`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f3a8c479644ca63d52ed172ebc922c3f5a56e4ad88332a3ba3a052839360f`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba00296054cd4a13b7ff959420b66d4e86fa2aa8bdafe0f01cb3f91f609136a`  
		Last Modified: Tue, 23 May 2023 01:23:39 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b204fbf0455b0452d3b0c4a21b6e15d7a5c3b5a9d1f34e81be67f5b11b506c`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.5 MB (16496465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0baa660d406b62bed7d4ce723b0fcb3e855790ad0d2b8ff95533109ae3254855`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2d6ab177afed853c8629165517469a6c210f96ba94a6a6a2384d40713f08c8`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9ce3c49056e3bb078dd3ba8f72e29bfa9027d41ecb171713b3ba73818f5ab5`  
		Last Modified: Tue, 23 May 2023 01:23:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4323c62c8c1f681922488afd95e44ecac331015a691d7c573d23d28099689cd`  
		Last Modified: Tue, 23 May 2023 01:23:41 GMT  
		Size: 16.9 MB (16873896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:883ce580efdc7b6813465965104378d5145e190bfd7a5b4481ef6e81b03c66da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull docker@sha256:a990a4f1fffd513fbb0354826eadedc7162904ed5657e0c1677ffe9328a21d5a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1826215665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d92f7a694bb5fff886f0f4c376f2632727e68fd5519870bac08797533cdeda`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:13:39 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 20 May 2023 01:15:04 GMT
ENV DOCKER_VERSION=24.0.1
# Sat, 20 May 2023 01:15:05 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.1.zip
# Sat, 20 May 2023 01:15:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:02 GMT
ENV DOCKER_BUILDX_VERSION=0.10.5
# Tue, 23 May 2023 01:15:03 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.10.5/buildx-v0.10.5.windows-amd64.exe
# Tue, 23 May 2023 01:15:04 GMT
ENV DOCKER_BUILDX_SHA256=9dbb9ab9b8f2aba21d2a9ea9113b98bebeed886a7df358dcdfe08bca1fd3ddb7
# Tue, 23 May 2023 01:15:31 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.18.1
# Tue, 23 May 2023 01:15:32 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.18.1/docker-compose-windows-x86_64.exe
# Tue, 23 May 2023 01:15:33 GMT
ENV DOCKER_COMPOSE_SHA256=6083a9057010a6a048d83c94318d254657abee48600baca2402fbe887d0b7ec4
# Tue, 23 May 2023 01:16:01 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94bc80e6c1e6606bc432e9fa1ebc3ed83fe3ceb5a176e0a7b2c8334bf863c53`  
		Last Modified: Wed, 10 May 2023 07:11:29 GMT  
		Size: 446.9 KB (446946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc754386dea5721554d4320fc581c4e83b653a954952515a5aaa5b52dbd4a574`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641b527d00cccb03bd30e17bc04e2372d8e5e57fa44fef30266f060c71f63954`  
		Last Modified: Sat, 20 May 2023 02:15:35 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b76accff37953841e1a00f8907a6abdb623e594e68784f932194d7dfad253`  
		Last Modified: Sat, 20 May 2023 02:15:37 GMT  
		Size: 17.4 MB (17442937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22811ed980a194a32b7f991db121c816d41a2f9ed42421253cedc81b7471ff3d`  
		Last Modified: Tue, 23 May 2023 01:23:21 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13423d9367df853b5b71f649a9ed032b074a113032b4145d15c95869e75bfb74`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9551a597f4845d99fe72d1e9855c2c500c5b8df9ca518a1b4ae0bba59bfe28e8`  
		Last Modified: Tue, 23 May 2023 01:23:19 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625d6a58bb92a0b4248d9836bd902fcffcb7dabf30eb4348c40bf552180f063`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.5 MB (16475300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f649be4312f54b778373c6ad7f856dddae81b7606fec596f2d6bdebf2c4af7c`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37ba2e268969eb8e02fd84e72477996f5668f50a5e03966f602a10cebc38fd6`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c454de9855bf96eb772c11c0664f35a5bcb0de98bbfd3cd08913f189e59c9c8e`  
		Last Modified: Tue, 23 May 2023 01:23:17 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e2c3d7edc4f0e36805d2852db1bc041000d9ad6ba91b96e50d0b85e7764bde`  
		Last Modified: Tue, 23 May 2023 01:23:22 GMT  
		Size: 16.9 MB (16856366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
