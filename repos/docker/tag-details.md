<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:19`](#docker19)
-	[`docker:19.03`](#docker1903)
-	[`docker:19.03.8`](#docker19038)
-	[`docker:19.03.8-dind`](#docker19038-dind)
-	[`docker:19.03.8-dind-rootless`](#docker19038-dind-rootless)
-	[`docker:19.03.8-git`](#docker19038-git)
-	[`docker:19.03-dind`](#docker1903-dind)
-	[`docker:19.03-dind-rootless`](#docker1903-dind-rootless)
-	[`docker:19.03-git`](#docker1903-git)
-	[`docker:19-dind`](#docker19-dind)
-	[`docker:19-dind-rootless`](#docker19-dind-rootless)
-	[`docker:19-git`](#docker19-git)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:stable`](#dockerstable)
-	[`docker:stable-dind`](#dockerstable-dind)
-	[`docker:stable-dind-rootless`](#dockerstable-dind-rootless)
-	[`docker:stable-git`](#dockerstable-git)
-	[`docker:test`](#dockertest)
-	[`docker:test-dind`](#dockertest-dind)
-	[`docker:test-dind-rootless`](#dockertest-dind-rootless)
-	[`docker:test-git`](#dockertest-git)

## `docker:19`

```console
$ docker pull docker@sha256:5bca19bb6d8f0aea380902af97be841d5841353c04e3eda5f87b4e932a509e94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19` - linux; amd64

```console
$ docker pull docker@sha256:bc7f740e2c0a8a9ec43b009b7cd35aafb10e69488a017110ad723003fbd3a7ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69447967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e036013d6d102186aa6871f4f1e579665b906b955ea86e3c60796b38a0ece73d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm variant v6

```console
$ docker pull docker@sha256:7905d808d76e6a5c380835e1c8b6b3776109d1ddd752dedcfbbd11a97672c2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64901295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd663210d571253c59a7d7f847a144e0fbffc0a060383b38b1c10e1d15dcfcea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm variant v7

```console
$ docker pull docker@sha256:5615028ebe8b6124e0b88a0aba8a81fa9958dfd3ceab4d30a66693e674374c81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64602290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:921bdeb870012309cc1967e84ec93b77e4dc07f8fa84677be447c1d00f7d516d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:52c7cadb9acebe940888680e1fbdecdaba35216df6011266f14618ae4ac88103
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62553330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e340fb5cba1fad5ee4330f067203231736c79e8c35e9f10d2d17c4b38feb0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03`

```console
$ docker pull docker@sha256:5bca19bb6d8f0aea380902af97be841d5841353c04e3eda5f87b4e932a509e94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03` - linux; amd64

```console
$ docker pull docker@sha256:bc7f740e2c0a8a9ec43b009b7cd35aafb10e69488a017110ad723003fbd3a7ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69447967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e036013d6d102186aa6871f4f1e579665b906b955ea86e3c60796b38a0ece73d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm variant v6

```console
$ docker pull docker@sha256:7905d808d76e6a5c380835e1c8b6b3776109d1ddd752dedcfbbd11a97672c2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64901295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd663210d571253c59a7d7f847a144e0fbffc0a060383b38b1c10e1d15dcfcea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm variant v7

```console
$ docker pull docker@sha256:5615028ebe8b6124e0b88a0aba8a81fa9958dfd3ceab4d30a66693e674374c81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64602290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:921bdeb870012309cc1967e84ec93b77e4dc07f8fa84677be447c1d00f7d516d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:52c7cadb9acebe940888680e1fbdecdaba35216df6011266f14618ae4ac88103
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62553330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e340fb5cba1fad5ee4330f067203231736c79e8c35e9f10d2d17c4b38feb0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.8`

**does not exist** (yet?)

## `docker:19.03.8-dind`

**does not exist** (yet?)

## `docker:19.03.8-dind-rootless`

**does not exist** (yet?)

## `docker:19.03.8-git`

**does not exist** (yet?)

## `docker:19.03-dind`

```console
$ docker pull docker@sha256:2683fcdf7480ea101415833f7793fb058c5f20227890a953b0a70bfc350af5bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-dind` - linux; amd64

```console
$ docker pull docker@sha256:5b45c3565b02cb453fc0ef33e3d082006293d5d002d9cfd06d6ff290724c2d37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75050940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14af3ba31e635475ec8f7fbe17470424514777621e627a91c41bbbe028dbae16`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:2a615eb1dc6677ebdf20646beb8afd4e2419e051cefe1d8e395e612ed4a2968e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68121303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f68b30bcf053ad30bf0a564ec194dad492285a808fba299f3b0293d6c24dffa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 16:53:07 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 16:53:08 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 16:53:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 16:53:11 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:53:12 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 16:53:13 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 16:53:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 16:53:15 GMT
CMD []
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40557879ffe943eb8e24d35fdffacc8e191846570cc62c4f545215dff3f0211f`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 3.2 MB (3215410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9dc691059c744fc0d04e4fed9a6a20ca299cf1a2591deccb8afbca2c6e1bff`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab043553c4c05caec0405af3f57bdc6a208c6c47f1d8d2059baf0c0835123337`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 753.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1661e9c50e15404cec22ab62a81f256da3238473a7948bffd46075be3548f6cb`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:bd459ffa862cf1e3f5f55d028beb215afc4849856c1c7d15faf9263c5f760d64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67485433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff47ffebc83552ef2fe050646ba9ec118d128b03bb2bb8944dad39a72890cb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:01:12 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:01:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:01:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:01:16 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:01:17 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:01:18 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:01:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:20 GMT
CMD []
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9aafce06341928f96c1fb32eb50696a7bb09092385be9a977d768bce9ea812`  
		Last Modified: Wed, 04 Mar 2020 17:02:23 GMT  
		Size: 2.9 MB (2878541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49644602064019ff980a601efa45cd917d5e289510064ea3b5a1b4029989bb0d`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171068e1f4d25ad29273ad0eea56151005e9b4d74e01aa778bc15c07219f3c59`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbb3759639a3b253b9032bc3860907f3096ceadb0017ebe0f270cbf1950ddd4`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5bdd9af013c6e1f3ae98cb960be78e3fc359cb4eec00a166bac03f3e60bc2391
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68158841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb46e7fa9917f26a4c9d905dbb70503744ef499e5b9503135212c05213a09528`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:42:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:42:51 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:42:52 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:42:54 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:55 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:42:55 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:42:56 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:57 GMT
CMD []
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4487e178cbccb6041e7684fb62891d947417a6d5cc3ff5e8bcf281bdcc0eda30`  
		Last Modified: Wed, 04 Mar 2020 17:43:51 GMT  
		Size: 5.6 MB (5600909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7243885bd041ab6cb79b00709fa2577d854d09ec44a5082a9787f14fc5b16cd`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9df0ad8a06746d4d9a242e875d8af1f312aa0915a3cd603870c49f2cb609d62`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce53b5c76c98febda467d08e9de090dbda090eb3b289c9345a79a2378929db0`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind-rootless`

```console
$ docker pull docker@sha256:1fcc48420e7c2c216f0c32923267fe471a134270c8405156c67f2c4c5d72e6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:e4353296f241b85976ea7f1885b00fed7be4ea44268d5fbd22b7c302b7b17710
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97580840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88504cd9a3f192922c817319508a9c5f9f5b506682835c320873b17dd12deee`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
# Wed, 04 Mar 2020 17:22:12 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Mar 2020 17:22:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Mar 2020 17:22:14 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Wed, 04 Mar 2020 17:22:16 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Wed, 04 Mar 2020 17:22:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Wed, 04 Mar 2020 17:22:28 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Mar 2020 17:22:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Mar 2020 17:22:28 GMT
USER rootless
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6141bfb617c1af01bc7c06529965c74d87e42d2f1443c7dc1800432e7cae3bf4`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 796.0 KB (796001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e93580a4ad9de8706bd94bb723c6c88b0c9fefe97965c822a7afcc7c259fea`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a16432e12743b944b3536a0a26cc715e7ebf954b1d13168d2723ed2560e9fd`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101f55e0075f21e2509937b9e1efb80a044ca9a085e09bf91a939c6bc474ae45`  
		Last Modified: Wed, 04 Mar 2020 17:23:20 GMT  
		Size: 9.1 MB (9109450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b21c4fce4a8090f3cc6a3c39b8d9c1832f8e3c146e33fb8eb4ee2a18e3ca3`  
		Last Modified: Wed, 04 Mar 2020 17:23:19 GMT  
		Size: 12.6 MB (12622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0682ee4c01c0d29e92f148d15eaec72f7aaad9552eb1063b3698498d12436fc7`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-git`

```console
$ docker pull docker@sha256:1f5e9a7d1a98ad80877f94ad9608bb636519385471f5ab54cbeaa654bbed70c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-git` - linux; amd64

```console
$ docker pull docker@sha256:27cdcf8663b0a5ea26b19878f60627deb2bc9fe0e071432f7d5dc1a132ae16ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77661883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b07c76f69789275285e37277861497724fec9ef91933183d21746098859a8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:33 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d456abaf46087e2c5698ee23380c7c7b8a4ec6bd3fa4765a85c31c67deee0e7`  
		Last Modified: Wed, 04 Mar 2020 17:23:28 GMT  
		Size: 8.2 MB (8213916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:086ea37f53337b5c71cf2ffc855d60f2af967581ddf4024ad6572239218bd2e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72736501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3698bb9df531e442934d7ec0057f602695171096f72904f861166911858484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:26 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11810f158f4db8b344ddf5d1be7216ec75164370b3a0fa8fad13344e2476afa1`  
		Last Modified: Wed, 04 Mar 2020 16:54:38 GMT  
		Size: 7.8 MB (7835206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:e38fa9700b8fc5f13543eb1da67affd268615cdaa2eda921414d8bbc04580e33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71675090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2c1f0cc0fcb80213f9306c6cc21bc45a4090d7e1a14e5d7d738b4752e3621c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a454bad18d5b57a19de767c777a68f66edf4aac14a7d388d9abe8ef3067e51`  
		Last Modified: Wed, 04 Mar 2020 17:02:41 GMT  
		Size: 7.1 MB (7072800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1a1e5818eacf93746d60ac517c71e5604e79e3f5d9868d3e15f3409485f02bdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70959381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0ae4bf2dfa420c176634742a8923bd5c00bc2ed399a80b3f971011a3ab68201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:43:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dbf38487840206e7943626accb2820553c0696f2a00483ed01fff916be6aa4`  
		Last Modified: Wed, 04 Mar 2020 17:44:10 GMT  
		Size: 8.4 MB (8406051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind`

```console
$ docker pull docker@sha256:2683fcdf7480ea101415833f7793fb058c5f20227890a953b0a70bfc350af5bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-dind` - linux; amd64

```console
$ docker pull docker@sha256:5b45c3565b02cb453fc0ef33e3d082006293d5d002d9cfd06d6ff290724c2d37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75050940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14af3ba31e635475ec8f7fbe17470424514777621e627a91c41bbbe028dbae16`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:2a615eb1dc6677ebdf20646beb8afd4e2419e051cefe1d8e395e612ed4a2968e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68121303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f68b30bcf053ad30bf0a564ec194dad492285a808fba299f3b0293d6c24dffa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 16:53:07 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 16:53:08 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 16:53:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 16:53:11 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:53:12 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 16:53:13 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 16:53:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 16:53:15 GMT
CMD []
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40557879ffe943eb8e24d35fdffacc8e191846570cc62c4f545215dff3f0211f`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 3.2 MB (3215410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9dc691059c744fc0d04e4fed9a6a20ca299cf1a2591deccb8afbca2c6e1bff`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab043553c4c05caec0405af3f57bdc6a208c6c47f1d8d2059baf0c0835123337`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 753.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1661e9c50e15404cec22ab62a81f256da3238473a7948bffd46075be3548f6cb`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:bd459ffa862cf1e3f5f55d028beb215afc4849856c1c7d15faf9263c5f760d64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67485433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff47ffebc83552ef2fe050646ba9ec118d128b03bb2bb8944dad39a72890cb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:01:12 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:01:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:01:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:01:16 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:01:17 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:01:18 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:01:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:20 GMT
CMD []
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9aafce06341928f96c1fb32eb50696a7bb09092385be9a977d768bce9ea812`  
		Last Modified: Wed, 04 Mar 2020 17:02:23 GMT  
		Size: 2.9 MB (2878541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49644602064019ff980a601efa45cd917d5e289510064ea3b5a1b4029989bb0d`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171068e1f4d25ad29273ad0eea56151005e9b4d74e01aa778bc15c07219f3c59`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbb3759639a3b253b9032bc3860907f3096ceadb0017ebe0f270cbf1950ddd4`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5bdd9af013c6e1f3ae98cb960be78e3fc359cb4eec00a166bac03f3e60bc2391
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68158841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb46e7fa9917f26a4c9d905dbb70503744ef499e5b9503135212c05213a09528`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:42:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:42:51 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:42:52 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:42:54 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:55 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:42:55 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:42:56 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:57 GMT
CMD []
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4487e178cbccb6041e7684fb62891d947417a6d5cc3ff5e8bcf281bdcc0eda30`  
		Last Modified: Wed, 04 Mar 2020 17:43:51 GMT  
		Size: 5.6 MB (5600909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7243885bd041ab6cb79b00709fa2577d854d09ec44a5082a9787f14fc5b16cd`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9df0ad8a06746d4d9a242e875d8af1f312aa0915a3cd603870c49f2cb609d62`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce53b5c76c98febda467d08e9de090dbda090eb3b289c9345a79a2378929db0`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:1fcc48420e7c2c216f0c32923267fe471a134270c8405156c67f2c4c5d72e6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:e4353296f241b85976ea7f1885b00fed7be4ea44268d5fbd22b7c302b7b17710
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97580840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88504cd9a3f192922c817319508a9c5f9f5b506682835c320873b17dd12deee`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
# Wed, 04 Mar 2020 17:22:12 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Mar 2020 17:22:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Mar 2020 17:22:14 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Wed, 04 Mar 2020 17:22:16 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Wed, 04 Mar 2020 17:22:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Wed, 04 Mar 2020 17:22:28 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Mar 2020 17:22:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Mar 2020 17:22:28 GMT
USER rootless
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6141bfb617c1af01bc7c06529965c74d87e42d2f1443c7dc1800432e7cae3bf4`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 796.0 KB (796001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e93580a4ad9de8706bd94bb723c6c88b0c9fefe97965c822a7afcc7c259fea`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a16432e12743b944b3536a0a26cc715e7ebf954b1d13168d2723ed2560e9fd`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101f55e0075f21e2509937b9e1efb80a044ca9a085e09bf91a939c6bc474ae45`  
		Last Modified: Wed, 04 Mar 2020 17:23:20 GMT  
		Size: 9.1 MB (9109450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b21c4fce4a8090f3cc6a3c39b8d9c1832f8e3c146e33fb8eb4ee2a18e3ca3`  
		Last Modified: Wed, 04 Mar 2020 17:23:19 GMT  
		Size: 12.6 MB (12622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0682ee4c01c0d29e92f148d15eaec72f7aaad9552eb1063b3698498d12436fc7`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-git`

```console
$ docker pull docker@sha256:1f5e9a7d1a98ad80877f94ad9608bb636519385471f5ab54cbeaa654bbed70c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-git` - linux; amd64

```console
$ docker pull docker@sha256:27cdcf8663b0a5ea26b19878f60627deb2bc9fe0e071432f7d5dc1a132ae16ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77661883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b07c76f69789275285e37277861497724fec9ef91933183d21746098859a8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:33 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d456abaf46087e2c5698ee23380c7c7b8a4ec6bd3fa4765a85c31c67deee0e7`  
		Last Modified: Wed, 04 Mar 2020 17:23:28 GMT  
		Size: 8.2 MB (8213916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:086ea37f53337b5c71cf2ffc855d60f2af967581ddf4024ad6572239218bd2e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72736501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3698bb9df531e442934d7ec0057f602695171096f72904f861166911858484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:26 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11810f158f4db8b344ddf5d1be7216ec75164370b3a0fa8fad13344e2476afa1`  
		Last Modified: Wed, 04 Mar 2020 16:54:38 GMT  
		Size: 7.8 MB (7835206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:e38fa9700b8fc5f13543eb1da67affd268615cdaa2eda921414d8bbc04580e33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71675090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2c1f0cc0fcb80213f9306c6cc21bc45a4090d7e1a14e5d7d738b4752e3621c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a454bad18d5b57a19de767c777a68f66edf4aac14a7d388d9abe8ef3067e51`  
		Last Modified: Wed, 04 Mar 2020 17:02:41 GMT  
		Size: 7.1 MB (7072800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1a1e5818eacf93746d60ac517c71e5604e79e3f5d9868d3e15f3409485f02bdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70959381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0ae4bf2dfa420c176634742a8923bd5c00bc2ed399a80b3f971011a3ab68201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:43:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dbf38487840206e7943626accb2820553c0696f2a00483ed01fff916be6aa4`  
		Last Modified: Wed, 04 Mar 2020 17:44:10 GMT  
		Size: 8.4 MB (8406051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:2683fcdf7480ea101415833f7793fb058c5f20227890a953b0a70bfc350af5bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:5b45c3565b02cb453fc0ef33e3d082006293d5d002d9cfd06d6ff290724c2d37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75050940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14af3ba31e635475ec8f7fbe17470424514777621e627a91c41bbbe028dbae16`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:2a615eb1dc6677ebdf20646beb8afd4e2419e051cefe1d8e395e612ed4a2968e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68121303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f68b30bcf053ad30bf0a564ec194dad492285a808fba299f3b0293d6c24dffa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 16:53:07 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 16:53:08 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 16:53:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 16:53:11 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:53:12 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 16:53:13 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 16:53:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 16:53:15 GMT
CMD []
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40557879ffe943eb8e24d35fdffacc8e191846570cc62c4f545215dff3f0211f`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 3.2 MB (3215410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9dc691059c744fc0d04e4fed9a6a20ca299cf1a2591deccb8afbca2c6e1bff`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab043553c4c05caec0405af3f57bdc6a208c6c47f1d8d2059baf0c0835123337`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 753.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1661e9c50e15404cec22ab62a81f256da3238473a7948bffd46075be3548f6cb`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:bd459ffa862cf1e3f5f55d028beb215afc4849856c1c7d15faf9263c5f760d64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67485433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff47ffebc83552ef2fe050646ba9ec118d128b03bb2bb8944dad39a72890cb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:01:12 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:01:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:01:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:01:16 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:01:17 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:01:18 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:01:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:20 GMT
CMD []
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9aafce06341928f96c1fb32eb50696a7bb09092385be9a977d768bce9ea812`  
		Last Modified: Wed, 04 Mar 2020 17:02:23 GMT  
		Size: 2.9 MB (2878541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49644602064019ff980a601efa45cd917d5e289510064ea3b5a1b4029989bb0d`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171068e1f4d25ad29273ad0eea56151005e9b4d74e01aa778bc15c07219f3c59`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbb3759639a3b253b9032bc3860907f3096ceadb0017ebe0f270cbf1950ddd4`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5bdd9af013c6e1f3ae98cb960be78e3fc359cb4eec00a166bac03f3e60bc2391
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68158841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb46e7fa9917f26a4c9d905dbb70503744ef499e5b9503135212c05213a09528`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:42:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:42:51 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:42:52 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:42:54 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:55 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:42:55 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:42:56 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:57 GMT
CMD []
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4487e178cbccb6041e7684fb62891d947417a6d5cc3ff5e8bcf281bdcc0eda30`  
		Last Modified: Wed, 04 Mar 2020 17:43:51 GMT  
		Size: 5.6 MB (5600909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7243885bd041ab6cb79b00709fa2577d854d09ec44a5082a9787f14fc5b16cd`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9df0ad8a06746d4d9a242e875d8af1f312aa0915a3cd603870c49f2cb609d62`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce53b5c76c98febda467d08e9de090dbda090eb3b289c9345a79a2378929db0`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:1fcc48420e7c2c216f0c32923267fe471a134270c8405156c67f2c4c5d72e6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:e4353296f241b85976ea7f1885b00fed7be4ea44268d5fbd22b7c302b7b17710
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97580840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88504cd9a3f192922c817319508a9c5f9f5b506682835c320873b17dd12deee`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
# Wed, 04 Mar 2020 17:22:12 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Mar 2020 17:22:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Mar 2020 17:22:14 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Wed, 04 Mar 2020 17:22:16 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Wed, 04 Mar 2020 17:22:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Wed, 04 Mar 2020 17:22:28 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Mar 2020 17:22:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Mar 2020 17:22:28 GMT
USER rootless
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6141bfb617c1af01bc7c06529965c74d87e42d2f1443c7dc1800432e7cae3bf4`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 796.0 KB (796001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e93580a4ad9de8706bd94bb723c6c88b0c9fefe97965c822a7afcc7c259fea`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a16432e12743b944b3536a0a26cc715e7ebf954b1d13168d2723ed2560e9fd`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101f55e0075f21e2509937b9e1efb80a044ca9a085e09bf91a939c6bc474ae45`  
		Last Modified: Wed, 04 Mar 2020 17:23:20 GMT  
		Size: 9.1 MB (9109450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b21c4fce4a8090f3cc6a3c39b8d9c1832f8e3c146e33fb8eb4ee2a18e3ca3`  
		Last Modified: Wed, 04 Mar 2020 17:23:19 GMT  
		Size: 12.6 MB (12622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0682ee4c01c0d29e92f148d15eaec72f7aaad9552eb1063b3698498d12436fc7`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:1f5e9a7d1a98ad80877f94ad9608bb636519385471f5ab54cbeaa654bbed70c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:27cdcf8663b0a5ea26b19878f60627deb2bc9fe0e071432f7d5dc1a132ae16ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77661883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b07c76f69789275285e37277861497724fec9ef91933183d21746098859a8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:33 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d456abaf46087e2c5698ee23380c7c7b8a4ec6bd3fa4765a85c31c67deee0e7`  
		Last Modified: Wed, 04 Mar 2020 17:23:28 GMT  
		Size: 8.2 MB (8213916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm variant v6

```console
$ docker pull docker@sha256:086ea37f53337b5c71cf2ffc855d60f2af967581ddf4024ad6572239218bd2e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72736501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3698bb9df531e442934d7ec0057f602695171096f72904f861166911858484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:26 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11810f158f4db8b344ddf5d1be7216ec75164370b3a0fa8fad13344e2476afa1`  
		Last Modified: Wed, 04 Mar 2020 16:54:38 GMT  
		Size: 7.8 MB (7835206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm variant v7

```console
$ docker pull docker@sha256:e38fa9700b8fc5f13543eb1da67affd268615cdaa2eda921414d8bbc04580e33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71675090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2c1f0cc0fcb80213f9306c6cc21bc45a4090d7e1a14e5d7d738b4752e3621c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a454bad18d5b57a19de767c777a68f66edf4aac14a7d388d9abe8ef3067e51`  
		Last Modified: Wed, 04 Mar 2020 17:02:41 GMT  
		Size: 7.1 MB (7072800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1a1e5818eacf93746d60ac517c71e5604e79e3f5d9868d3e15f3409485f02bdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70959381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0ae4bf2dfa420c176634742a8923bd5c00bc2ed399a80b3f971011a3ab68201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:43:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dbf38487840206e7943626accb2820553c0696f2a00483ed01fff916be6aa4`  
		Last Modified: Wed, 04 Mar 2020 17:44:10 GMT  
		Size: 8.4 MB (8406051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:5bca19bb6d8f0aea380902af97be841d5841353c04e3eda5f87b4e932a509e94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:bc7f740e2c0a8a9ec43b009b7cd35aafb10e69488a017110ad723003fbd3a7ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69447967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e036013d6d102186aa6871f4f1e579665b906b955ea86e3c60796b38a0ece73d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm variant v6

```console
$ docker pull docker@sha256:7905d808d76e6a5c380835e1c8b6b3776109d1ddd752dedcfbbd11a97672c2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64901295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd663210d571253c59a7d7f847a144e0fbffc0a060383b38b1c10e1d15dcfcea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm variant v7

```console
$ docker pull docker@sha256:5615028ebe8b6124e0b88a0aba8a81fa9958dfd3ceab4d30a66693e674374c81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64602290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:921bdeb870012309cc1967e84ec93b77e4dc07f8fa84677be447c1d00f7d516d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:52c7cadb9acebe940888680e1fbdecdaba35216df6011266f14618ae4ac88103
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62553330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e340fb5cba1fad5ee4330f067203231736c79e8c35e9f10d2d17c4b38feb0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable`

```console
$ docker pull docker@sha256:5bca19bb6d8f0aea380902af97be841d5841353c04e3eda5f87b4e932a509e94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:stable` - linux; amd64

```console
$ docker pull docker@sha256:bc7f740e2c0a8a9ec43b009b7cd35aafb10e69488a017110ad723003fbd3a7ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69447967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e036013d6d102186aa6871f4f1e579665b906b955ea86e3c60796b38a0ece73d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable` - linux; arm variant v6

```console
$ docker pull docker@sha256:7905d808d76e6a5c380835e1c8b6b3776109d1ddd752dedcfbbd11a97672c2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64901295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd663210d571253c59a7d7f847a144e0fbffc0a060383b38b1c10e1d15dcfcea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable` - linux; arm variant v7

```console
$ docker pull docker@sha256:5615028ebe8b6124e0b88a0aba8a81fa9958dfd3ceab4d30a66693e674374c81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64602290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:921bdeb870012309cc1967e84ec93b77e4dc07f8fa84677be447c1d00f7d516d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:52c7cadb9acebe940888680e1fbdecdaba35216df6011266f14618ae4ac88103
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62553330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e340fb5cba1fad5ee4330f067203231736c79e8c35e9f10d2d17c4b38feb0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable-dind`

```console
$ docker pull docker@sha256:2683fcdf7480ea101415833f7793fb058c5f20227890a953b0a70bfc350af5bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:stable-dind` - linux; amd64

```console
$ docker pull docker@sha256:5b45c3565b02cb453fc0ef33e3d082006293d5d002d9cfd06d6ff290724c2d37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75050940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14af3ba31e635475ec8f7fbe17470424514777621e627a91c41bbbe028dbae16`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:2a615eb1dc6677ebdf20646beb8afd4e2419e051cefe1d8e395e612ed4a2968e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68121303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f68b30bcf053ad30bf0a564ec194dad492285a808fba299f3b0293d6c24dffa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 16:53:07 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 16:53:08 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 16:53:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 16:53:11 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:53:12 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 16:53:13 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 16:53:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 16:53:15 GMT
CMD []
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40557879ffe943eb8e24d35fdffacc8e191846570cc62c4f545215dff3f0211f`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 3.2 MB (3215410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9dc691059c744fc0d04e4fed9a6a20ca299cf1a2591deccb8afbca2c6e1bff`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab043553c4c05caec0405af3f57bdc6a208c6c47f1d8d2059baf0c0835123337`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 753.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1661e9c50e15404cec22ab62a81f256da3238473a7948bffd46075be3548f6cb`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:bd459ffa862cf1e3f5f55d028beb215afc4849856c1c7d15faf9263c5f760d64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67485433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff47ffebc83552ef2fe050646ba9ec118d128b03bb2bb8944dad39a72890cb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:01:12 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:01:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:01:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:01:16 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:01:17 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:01:18 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:01:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:20 GMT
CMD []
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9aafce06341928f96c1fb32eb50696a7bb09092385be9a977d768bce9ea812`  
		Last Modified: Wed, 04 Mar 2020 17:02:23 GMT  
		Size: 2.9 MB (2878541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49644602064019ff980a601efa45cd917d5e289510064ea3b5a1b4029989bb0d`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171068e1f4d25ad29273ad0eea56151005e9b4d74e01aa778bc15c07219f3c59`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbb3759639a3b253b9032bc3860907f3096ceadb0017ebe0f270cbf1950ddd4`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5bdd9af013c6e1f3ae98cb960be78e3fc359cb4eec00a166bac03f3e60bc2391
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68158841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb46e7fa9917f26a4c9d905dbb70503744ef499e5b9503135212c05213a09528`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:42:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:42:51 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:42:52 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:42:54 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:55 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:42:55 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:42:56 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:57 GMT
CMD []
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4487e178cbccb6041e7684fb62891d947417a6d5cc3ff5e8bcf281bdcc0eda30`  
		Last Modified: Wed, 04 Mar 2020 17:43:51 GMT  
		Size: 5.6 MB (5600909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7243885bd041ab6cb79b00709fa2577d854d09ec44a5082a9787f14fc5b16cd`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9df0ad8a06746d4d9a242e875d8af1f312aa0915a3cd603870c49f2cb609d62`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce53b5c76c98febda467d08e9de090dbda090eb3b289c9345a79a2378929db0`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable-dind-rootless`

```console
$ docker pull docker@sha256:1fcc48420e7c2c216f0c32923267fe471a134270c8405156c67f2c4c5d72e6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:stable-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:e4353296f241b85976ea7f1885b00fed7be4ea44268d5fbd22b7c302b7b17710
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97580840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88504cd9a3f192922c817319508a9c5f9f5b506682835c320873b17dd12deee`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
# Wed, 04 Mar 2020 17:22:12 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Mar 2020 17:22:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Mar 2020 17:22:14 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Wed, 04 Mar 2020 17:22:16 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Wed, 04 Mar 2020 17:22:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Wed, 04 Mar 2020 17:22:28 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Mar 2020 17:22:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Mar 2020 17:22:28 GMT
USER rootless
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6141bfb617c1af01bc7c06529965c74d87e42d2f1443c7dc1800432e7cae3bf4`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 796.0 KB (796001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e93580a4ad9de8706bd94bb723c6c88b0c9fefe97965c822a7afcc7c259fea`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a16432e12743b944b3536a0a26cc715e7ebf954b1d13168d2723ed2560e9fd`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101f55e0075f21e2509937b9e1efb80a044ca9a085e09bf91a939c6bc474ae45`  
		Last Modified: Wed, 04 Mar 2020 17:23:20 GMT  
		Size: 9.1 MB (9109450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b21c4fce4a8090f3cc6a3c39b8d9c1832f8e3c146e33fb8eb4ee2a18e3ca3`  
		Last Modified: Wed, 04 Mar 2020 17:23:19 GMT  
		Size: 12.6 MB (12622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0682ee4c01c0d29e92f148d15eaec72f7aaad9552eb1063b3698498d12436fc7`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable-git`

```console
$ docker pull docker@sha256:1f5e9a7d1a98ad80877f94ad9608bb636519385471f5ab54cbeaa654bbed70c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:stable-git` - linux; amd64

```console
$ docker pull docker@sha256:27cdcf8663b0a5ea26b19878f60627deb2bc9fe0e071432f7d5dc1a132ae16ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77661883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b07c76f69789275285e37277861497724fec9ef91933183d21746098859a8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:33 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d456abaf46087e2c5698ee23380c7c7b8a4ec6bd3fa4765a85c31c67deee0e7`  
		Last Modified: Wed, 04 Mar 2020 17:23:28 GMT  
		Size: 8.2 MB (8213916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:086ea37f53337b5c71cf2ffc855d60f2af967581ddf4024ad6572239218bd2e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72736501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3698bb9df531e442934d7ec0057f602695171096f72904f861166911858484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:26 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11810f158f4db8b344ddf5d1be7216ec75164370b3a0fa8fad13344e2476afa1`  
		Last Modified: Wed, 04 Mar 2020 16:54:38 GMT  
		Size: 7.8 MB (7835206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:e38fa9700b8fc5f13543eb1da67affd268615cdaa2eda921414d8bbc04580e33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71675090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2c1f0cc0fcb80213f9306c6cc21bc45a4090d7e1a14e5d7d738b4752e3621c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a454bad18d5b57a19de767c777a68f66edf4aac14a7d388d9abe8ef3067e51`  
		Last Modified: Wed, 04 Mar 2020 17:02:41 GMT  
		Size: 7.1 MB (7072800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1a1e5818eacf93746d60ac517c71e5604e79e3f5d9868d3e15f3409485f02bdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70959381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0ae4bf2dfa420c176634742a8923bd5c00bc2ed399a80b3f971011a3ab68201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:43:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dbf38487840206e7943626accb2820553c0696f2a00483ed01fff916be6aa4`  
		Last Modified: Wed, 04 Mar 2020 17:44:10 GMT  
		Size: 8.4 MB (8406051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test`

```console
$ docker pull docker@sha256:5bca19bb6d8f0aea380902af97be841d5841353c04e3eda5f87b4e932a509e94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test` - linux; amd64

```console
$ docker pull docker@sha256:bc7f740e2c0a8a9ec43b009b7cd35aafb10e69488a017110ad723003fbd3a7ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69447967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e036013d6d102186aa6871f4f1e579665b906b955ea86e3c60796b38a0ece73d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm variant v6

```console
$ docker pull docker@sha256:7905d808d76e6a5c380835e1c8b6b3776109d1ddd752dedcfbbd11a97672c2c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64901295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd663210d571253c59a7d7f847a144e0fbffc0a060383b38b1c10e1d15dcfcea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm variant v7

```console
$ docker pull docker@sha256:5615028ebe8b6124e0b88a0aba8a81fa9958dfd3ceab4d30a66693e674374c81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64602290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:921bdeb870012309cc1967e84ec93b77e4dc07f8fa84677be447c1d00f7d516d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:52c7cadb9acebe940888680e1fbdecdaba35216df6011266f14618ae4ac88103
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62553330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e340fb5cba1fad5ee4330f067203231736c79e8c35e9f10d2d17c4b38feb0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-dind`

```console
$ docker pull docker@sha256:2683fcdf7480ea101415833f7793fb058c5f20227890a953b0a70bfc350af5bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test-dind` - linux; amd64

```console
$ docker pull docker@sha256:5b45c3565b02cb453fc0ef33e3d082006293d5d002d9cfd06d6ff290724c2d37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75050940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14af3ba31e635475ec8f7fbe17470424514777621e627a91c41bbbe028dbae16`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:2a615eb1dc6677ebdf20646beb8afd4e2419e051cefe1d8e395e612ed4a2968e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68121303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f68b30bcf053ad30bf0a564ec194dad492285a808fba299f3b0293d6c24dffa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 16:53:07 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 16:53:08 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 16:53:10 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 16:53:11 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:53:12 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 16:53:13 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 16:53:14 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 16:53:15 GMT
CMD []
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40557879ffe943eb8e24d35fdffacc8e191846570cc62c4f545215dff3f0211f`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 3.2 MB (3215410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9dc691059c744fc0d04e4fed9a6a20ca299cf1a2591deccb8afbca2c6e1bff`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab043553c4c05caec0405af3f57bdc6a208c6c47f1d8d2059baf0c0835123337`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 753.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1661e9c50e15404cec22ab62a81f256da3238473a7948bffd46075be3548f6cb`  
		Last Modified: Wed, 04 Mar 2020 16:54:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:bd459ffa862cf1e3f5f55d028beb215afc4849856c1c7d15faf9263c5f760d64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.5 MB (67485433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff47ffebc83552ef2fe050646ba9ec118d128b03bb2bb8944dad39a72890cb8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:01:12 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:01:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:01:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:01:16 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:01:17 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:01:18 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:01:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:20 GMT
CMD []
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9aafce06341928f96c1fb32eb50696a7bb09092385be9a977d768bce9ea812`  
		Last Modified: Wed, 04 Mar 2020 17:02:23 GMT  
		Size: 2.9 MB (2878541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49644602064019ff980a601efa45cd917d5e289510064ea3b5a1b4029989bb0d`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171068e1f4d25ad29273ad0eea56151005e9b4d74e01aa778bc15c07219f3c59`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbb3759639a3b253b9032bc3860907f3096ceadb0017ebe0f270cbf1950ddd4`  
		Last Modified: Wed, 04 Mar 2020 17:02:22 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5bdd9af013c6e1f3ae98cb960be78e3fc359cb4eec00a166bac03f3e60bc2391
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68158841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb46e7fa9917f26a4c9d905dbb70503744ef499e5b9503135212c05213a09528`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:42:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:42:51 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:42:52 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:42:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:42:54 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:55 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:42:55 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:42:56 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:57 GMT
CMD []
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4487e178cbccb6041e7684fb62891d947417a6d5cc3ff5e8bcf281bdcc0eda30`  
		Last Modified: Wed, 04 Mar 2020 17:43:51 GMT  
		Size: 5.6 MB (5600909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7243885bd041ab6cb79b00709fa2577d854d09ec44a5082a9787f14fc5b16cd`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9df0ad8a06746d4d9a242e875d8af1f312aa0915a3cd603870c49f2cb609d62`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce53b5c76c98febda467d08e9de090dbda090eb3b289c9345a79a2378929db0`  
		Last Modified: Wed, 04 Mar 2020 17:43:50 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-dind-rootless`

```console
$ docker pull docker@sha256:1fcc48420e7c2c216f0c32923267fe471a134270c8405156c67f2c4c5d72e6ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:test-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:e4353296f241b85976ea7f1885b00fed7be4ea44268d5fbd22b7c302b7b17710
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97580840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88504cd9a3f192922c817319508a9c5f9f5b506682835c320873b17dd12deee`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 04 Mar 2020 17:22:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 04 Mar 2020 17:22:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 04 Mar 2020 17:22:07 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:22:07 GMT
VOLUME [/var/lib/docker]
# Wed, 04 Mar 2020 17:22:07 GMT
EXPOSE 2375 2376
# Wed, 04 Mar 2020 17:22:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 04 Mar 2020 17:22:07 GMT
CMD []
# Wed, 04 Mar 2020 17:22:12 GMT
RUN apk add --no-cache iproute2
# Wed, 04 Mar 2020 17:22:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 04 Mar 2020 17:22:14 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 04 Mar 2020 17:22:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Wed, 04 Mar 2020 17:22:16 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Wed, 04 Mar 2020 17:22:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Wed, 04 Mar 2020 17:22:28 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 04 Mar 2020 17:22:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 04 Mar 2020 17:22:28 GMT
USER rootless
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e7dd2f7ff9a88146afde90862ff21d3756e2ad8391b39f0b77b19a47087f6`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 5.6 MB (5598399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f469d3c2a9233205751c9765649477d7924d26e861cca0747a14e9b34d869`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5c0c310ba9cf022fbaf0c64aae31d8f300a76f480aaa90d064c236eaf7063`  
		Last Modified: Wed, 04 Mar 2020 17:23:09 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367cd13753e5e7c74e0ecb1d3ec19f3fa50126b80873249c8441df6dd4e8e502`  
		Last Modified: Wed, 04 Mar 2020 17:23:10 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6141bfb617c1af01bc7c06529965c74d87e42d2f1443c7dc1800432e7cae3bf4`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 796.0 KB (796001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e93580a4ad9de8706bd94bb723c6c88b0c9fefe97965c822a7afcc7c259fea`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a16432e12743b944b3536a0a26cc715e7ebf954b1d13168d2723ed2560e9fd`  
		Last Modified: Wed, 04 Mar 2020 17:23:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101f55e0075f21e2509937b9e1efb80a044ca9a085e09bf91a939c6bc474ae45`  
		Last Modified: Wed, 04 Mar 2020 17:23:20 GMT  
		Size: 9.1 MB (9109450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95b21c4fce4a8090f3cc6a3c39b8d9c1832f8e3c146e33fb8eb4ee2a18e3ca3`  
		Last Modified: Wed, 04 Mar 2020 17:23:19 GMT  
		Size: 12.6 MB (12622836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0682ee4c01c0d29e92f148d15eaec72f7aaad9552eb1063b3698498d12436fc7`  
		Last Modified: Wed, 04 Mar 2020 17:23:16 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-git`

```console
$ docker pull docker@sha256:1f5e9a7d1a98ad80877f94ad9608bb636519385471f5ab54cbeaa654bbed70c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test-git` - linux; amd64

```console
$ docker pull docker@sha256:27cdcf8663b0a5ea26b19878f60627deb2bc9fe0e071432f7d5dc1a132ae16ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.7 MB (77661883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b07c76f69789275285e37277861497724fec9ef91933183d21746098859a8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:42:06 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 04:42:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:21:51 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:21:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:21:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:21:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:21:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:21:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:21:58 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:22:33 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd54125436dc48e0d60096d61457bcfd886136eb67815a60210ec67d3793096f`  
		Last Modified: Sat, 18 Jan 2020 04:43:03 GMT  
		Size: 2.4 MB (2425150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1554c15cbb8c6b81fd21a057c8e97749fb24fd5befeb94ad960d3a350f91f`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4cf184ccf4b52d5c8d08df033371766d079793fe1867970b60474ac4fc507`  
		Last Modified: Wed, 04 Mar 2020 17:23:02 GMT  
		Size: 64.2 MB (64218024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aca4f9099240ff6a1a6e2e518fb4daf0eef7b50a9b967ad64286e48bebd3104`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60fe6b6c13841ddde5debfedcfc47b25f1676e7f2e3c567fe6e34766258c78e`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be01bc37983eab8da8605450958ba7b9f7fd092b3179923b32dfb45741c848f`  
		Last Modified: Wed, 04 Mar 2020 17:22:44 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d456abaf46087e2c5698ee23380c7c7b8a4ec6bd3fa4765a85c31c67deee0e7`  
		Last Modified: Wed, 04 Mar 2020 17:23:28 GMT  
		Size: 8.2 MB (8213916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:086ea37f53337b5c71cf2ffc855d60f2af967581ddf4024ad6572239218bd2e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72736501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3698bb9df531e442934d7ec0057f602695171096f72904f861166911858484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:52:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 05:52:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 05:52:35 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 16:52:36 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 16:52:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 16:52:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 16:52:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 16:52:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 16:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 16:52:54 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 16:53:26 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c86f804e7b5cc2f1f9d87340dfef1fcc13615f2cbd25bda470e513c1e4a627`  
		Last Modified: Sat, 18 Jan 2020 05:54:22 GMT  
		Size: 2.4 MB (2355405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d84775c03f92068112e3757afd6ddab1b2c0a3d1073e91b182620b6ec239f7`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09284621dc2c37675dbe65ac25d62bebafe4645c6257c3fa9da8ee5ff284f4df`  
		Last Modified: Wed, 04 Mar 2020 16:54:08 GMT  
		Size: 59.9 MB (59926461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b8ac029dab8d558f2cc15e7e7afb9ea44a6d55d6df2aa00d7b04b4bfa6db6d`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed60b41d38a7b405355c0e726c49f350f5f7342ce33f17ddc5dad17222345b0`  
		Last Modified: Wed, 04 Mar 2020 16:53:41 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f06186bba627a05b4a69ffacc3530a74356fff6bc3e99cbc3471d6220a3aabf`  
		Last Modified: Wed, 04 Mar 2020 16:53:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11810f158f4db8b344ddf5d1be7216ec75164370b3a0fa8fad13344e2476afa1`  
		Last Modified: Wed, 04 Mar 2020 16:54:38 GMT  
		Size: 7.8 MB (7835206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:e38fa9700b8fc5f13543eb1da67affd268615cdaa2eda921414d8bbc04580e33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71675090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f2c1f0cc0fcb80213f9306c6cc21bc45a4090d7e1a14e5d7d738b4752e3621c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:01:09 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 03:01:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 03:01:20 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:00:45 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:00:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:00:57 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:00:58 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:01:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:01:01 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:01:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5014010b799b2f3cc6305fd21cc4b096dd28ad093e165cea5976f92ccb8c462`  
		Last Modified: Sat, 18 Jan 2020 03:03:27 GMT  
		Size: 2.3 MB (2254397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f49247ef05003d569c198c4908b849fdadd330bf360c04360ae48fd0d68b6d`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b496238e7751aebcae85cfea232bf453d3fc3ce3b9704c95352486e417be9d9`  
		Last Modified: Wed, 04 Mar 2020 17:02:10 GMT  
		Size: 59.9 MB (59926470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f3e493cd3a9cbc75e4204038c33c21d6074dbe6ebe9ba87588f9a32881a2b4`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b754c53d46589e23f3649c78e490da17128aec8c9ac6c27a27dc06eede2e6a1e`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2659f8abc7c551d03eb0be08bdae79fc6bb30164c0576fe140ee949c85bfd72`  
		Last Modified: Wed, 04 Mar 2020 17:01:49 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a454bad18d5b57a19de767c777a68f66edf4aac14a7d388d9abe8ef3067e51`  
		Last Modified: Wed, 04 Mar 2020 17:02:41 GMT  
		Size: 7.1 MB (7072800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1a1e5818eacf93746d60ac517c71e5604e79e3f5d9868d3e15f3409485f02bdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70959381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0ae4bf2dfa420c176634742a8923bd5c00bc2ed399a80b3f971011a3ab68201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:23:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Sat, 18 Jan 2020 02:23:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 18 Jan 2020 02:23:12 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 04 Mar 2020 17:42:28 GMT
ENV DOCKER_VERSION=19.03.7
# Wed, 04 Mar 2020 17:42:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 04 Mar 2020 17:42:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 04 Mar 2020 17:42:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 04 Mar 2020 17:42:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 04 Mar 2020 17:42:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 04 Mar 2020 17:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Mar 2020 17:42:40 GMT
CMD ["sh"]
# Wed, 04 Mar 2020 17:43:05 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2917335fcb0a6856d5bf55430ba707c2c1378029a109e61959e62d2769230db`  
		Last Modified: Sat, 18 Jan 2020 02:25:35 GMT  
		Size: 2.4 MB (2445713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d3c84c2515134ddfa5ae5bac6e140953e9576fcd30a0bbc10fbc565d267895`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389b437d255495ac0a52d870784a869abfcadd2672060744043fbc26db408968`  
		Last Modified: Wed, 04 Mar 2020 17:43:39 GMT  
		Size: 57.4 MB (57382675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7a94e4d7cd4e2ec8094927df8b8aedfe40ab7f175fb381a68e04187773eaa3`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9cd851b371a1250c8c247ccb5cf69a2ada4c0c4b8c82ba2a48700835c95f96`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f7c33f26a071c090d6dbb68ced7dad33a6e4c8db63900af921b75c1651f562`  
		Last Modified: Wed, 04 Mar 2020 17:43:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dbf38487840206e7943626accb2820553c0696f2a00483ed01fff916be6aa4`  
		Last Modified: Wed, 04 Mar 2020 17:44:10 GMT  
		Size: 8.4 MB (8406051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
