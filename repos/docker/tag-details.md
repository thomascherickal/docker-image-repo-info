<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:19`](#docker19)
-	[`docker:19.03`](#docker1903)
-	[`docker:19.03.5`](#docker19035)
-	[`docker:19.03.5-dind`](#docker19035-dind)
-	[`docker:19.03.5-dind-rootless`](#docker19035-dind-rootless)
-	[`docker:19.03.5-git`](#docker19035-git)
-	[`docker:19.03.6-rc1`](#docker19036-rc1)
-	[`docker:19.03.6-rc1-dind`](#docker19036-rc1-dind)
-	[`docker:19.03.6-rc1-dind-rootless`](#docker19036-rc1-dind-rootless)
-	[`docker:19.03.6-rc1-git`](#docker19036-rc1-git)
-	[`docker:19.03-dind`](#docker1903-dind)
-	[`docker:19.03-dind-rootless`](#docker1903-dind-rootless)
-	[`docker:19.03-git`](#docker1903-git)
-	[`docker:19.03-rc`](#docker1903-rc)
-	[`docker:19.03-rc-dind`](#docker1903-rc-dind)
-	[`docker:19.03-rc-dind-rootless`](#docker1903-rc-dind-rootless)
-	[`docker:19.03-rc-git`](#docker1903-rc-git)
-	[`docker:19-dind`](#docker19-dind)
-	[`docker:19-dind-rootless`](#docker19-dind-rootless)
-	[`docker:19-git`](#docker19-git)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:rc`](#dockerrc)
-	[`docker:rc-dind`](#dockerrc-dind)
-	[`docker:rc-dind-rootless`](#dockerrc-dind-rootless)
-	[`docker:rc-git`](#dockerrc-git)
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
$ docker pull docker@sha256:0b90b0aefd15794e4d5bea2debc3b761c1d3481a92ec7166f8453652d0deba95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19` - linux; amd64

```console
$ docker pull docker@sha256:48db0e29e2214d564b66daffc707ad290c8788dc655cea59c605f021790d38a0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69033024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c774f62a9b520060d72c3c1901facdfdfd0fc4ae7c5e817cdaf6acd456432c`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm variant v6

```console
$ docker pull docker@sha256:aa908727daa7433a0d156f6c6703fe5d945c4019e8b7f5d0c4fc8213e6d67fed
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64511941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e68c26581b5f619c73bdd54951308df6920447f7be745bea2bfbb6b3624b26`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm variant v7

```console
$ docker pull docker@sha256:ec6f3f2f65803962bd623ab2de639bd87d41d856c6ef477ae58383b379a1376a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64208081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fc3364d97bc6d5e8c8de60fa7c776bbc4eb6ca32c38029201f27c506086b11`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e09d98b19bbee9f15b9f66604d48401833716faef061e9e509b48fb8db8bd1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62176875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:466581031774ac8ddb27699e61f2fbf858fce357adad7352cc410ef9ad6344bf`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03`

```console
$ docker pull docker@sha256:0b90b0aefd15794e4d5bea2debc3b761c1d3481a92ec7166f8453652d0deba95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03` - linux; amd64

```console
$ docker pull docker@sha256:48db0e29e2214d564b66daffc707ad290c8788dc655cea59c605f021790d38a0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69033024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c774f62a9b520060d72c3c1901facdfdfd0fc4ae7c5e817cdaf6acd456432c`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm variant v6

```console
$ docker pull docker@sha256:aa908727daa7433a0d156f6c6703fe5d945c4019e8b7f5d0c4fc8213e6d67fed
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64511941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e68c26581b5f619c73bdd54951308df6920447f7be745bea2bfbb6b3624b26`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm variant v7

```console
$ docker pull docker@sha256:ec6f3f2f65803962bd623ab2de639bd87d41d856c6ef477ae58383b379a1376a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64208081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fc3364d97bc6d5e8c8de60fa7c776bbc4eb6ca32c38029201f27c506086b11`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e09d98b19bbee9f15b9f66604d48401833716faef061e9e509b48fb8db8bd1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62176875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:466581031774ac8ddb27699e61f2fbf858fce357adad7352cc410ef9ad6344bf`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.5`

```console
$ docker pull docker@sha256:0b90b0aefd15794e4d5bea2debc3b761c1d3481a92ec7166f8453652d0deba95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03.5` - linux; amd64

```console
$ docker pull docker@sha256:48db0e29e2214d564b66daffc707ad290c8788dc655cea59c605f021790d38a0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69033024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c774f62a9b520060d72c3c1901facdfdfd0fc4ae7c5e817cdaf6acd456432c`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5` - linux; arm variant v6

```console
$ docker pull docker@sha256:aa908727daa7433a0d156f6c6703fe5d945c4019e8b7f5d0c4fc8213e6d67fed
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64511941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e68c26581b5f619c73bdd54951308df6920447f7be745bea2bfbb6b3624b26`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5` - linux; arm variant v7

```console
$ docker pull docker@sha256:ec6f3f2f65803962bd623ab2de639bd87d41d856c6ef477ae58383b379a1376a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64208081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fc3364d97bc6d5e8c8de60fa7c776bbc4eb6ca32c38029201f27c506086b11`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e09d98b19bbee9f15b9f66604d48401833716faef061e9e509b48fb8db8bd1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62176875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:466581031774ac8ddb27699e61f2fbf858fce357adad7352cc410ef9ad6344bf`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.5-dind`

```console
$ docker pull docker@sha256:033ba84f8ea98910d8fc51b8263fbeb24c48d6daf55ef7c654e2981784dac2f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03.5-dind` - linux; amd64

```console
$ docker pull docker@sha256:efd3d1db027f0c8d2cc7019b5381fc9c3cdbbda3642c3ef4feefe5a36cbf0769
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74624904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8489eeb24a264b6bcdb17f3da00140cebe92ee36bd22365f37d07d59390df4ee`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:1e319d9500b33aea20e9c76900595c113e652ebf38ed7021f5daf0e5d78f48af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67731913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6bc19942666d644c636de3a0210745329f07a4c2d3f32c3e9cbd7454e1228c`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 05:53:41 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 05:53:41 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 05:53:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 05:53:44 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:45 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 05:53:46 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 05:53:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:47 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6186deaef3161317f61f202acfab3875747c2a724fad1a65f29f18b068a9ca6c`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 3.2 MB (3215383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6fa6e67b938d446f54f8d3a432d35377ff3431821d39ea805fb2de790ef343`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00bcda5d341dc29b37b45898451e3133f9d420af32d36b21c94d30ac2429ed6`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 749.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daeb323203a88ce4e9152363b7ea9dc8c97580d9723309e442b2c170beb2815`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:7e8985ea07f8786be5b7c551d9547aac01e43a74e8a5831685b39d40fda6d3c6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67091202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef820b49fd591346a99dec34fab401da3022b7cbd60eb8d06f9baef8872d9f3`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:02:23 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 03:02:28 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 03:02:31 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 03:02:36 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 03:02:38 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:02:41 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 03:02:43 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 03:02:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:49 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cb30959a65f691f18075812bbdb8d5f87f944b6d8012dbce90e70e61de7c17`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 2.9 MB (2878527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4bdbf92a47a6e710c3aa65a5fbe9136e986509ab9dacdb67a196fa99441578`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ee73f368ab0a867e3f6b7294736b2ea3263dbf8cc5e6881a1b68ff5856a5c7`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 752.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0bf5e1afaa1f42f73b39a23c9e2203e65c65f6246e63d17ae6def1232a6c5b`  
		Last Modified: Sat, 18 Jan 2020 03:04:00 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31f0251cf185d41e1b6f25bf8acf3d816a73d1d8e583b4c72321a7ccc05801e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67770716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53793fffe26de8f80d9cdfa58c38018e90af8d08eb3f44ebedc03079b7d04d`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 02:24:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 02:24:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 02:24:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 02:24:22 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:24:25 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 02:24:26 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 02:24:30 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 02:24:33 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4704739272105dd3fdfc8614ba689cffe338a0faddc99dace44e191c4567ce`  
		Last Modified: Sat, 18 Jan 2020 02:26:12 GMT  
		Size: 5.6 MB (5589240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8637fb5dd84f5ab45114fc090fda27e2eee33b46a01802c9853a3d0c1b623`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab01413155fcbeedeee71c38d84c48825794515972fd5480a22210379d739d0a`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9514c7ce5d1ffef3aa0a3d41faed1d3ac1e700f99f71157dd4e7d6c418b01de`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.5-dind-rootless`

```console
$ docker pull docker@sha256:51f925a59f79f9f85b4869649f6bec7bed065f381186f4102c942ddd4a861cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03.5-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:966cb6bf3b3955ebda64d4e156870e68e3ce20ac9c84a01dee28803aebc334af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97154857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384deac7f3c53083e5d29d8e56a0fa57afa7d88db3c4c34a80c774852f789d26`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
CMD []
# Sat, 18 Jan 2020 04:42:28 GMT
RUN apk add --no-cache iproute2
# Sat, 18 Jan 2020 04:42:29 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Sat, 18 Jan 2020 04:42:30 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Sat, 18 Jan 2020 04:42:32 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Sat, 18 Jan 2020 04:42:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Sat, 18 Jan 2020 04:42:44 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Sat, 18 Jan 2020 04:42:44 GMT
VOLUME [/home/rootless/.local/share/docker]
# Sat, 18 Jan 2020 04:42:44 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cdf1bd44b48b8727fa4bb0545240435dcf820156f0408b1bc13c094f8c01ea`  
		Last Modified: Sat, 18 Jan 2020 04:43:31 GMT  
		Size: 796.0 KB (795977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2313da576c87883442d37ff3743eacdb90d03a6928e9296f65a1083828ffc33`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b530e16b9b04d347cb7c9c99bfa6e4929f67f58f26d1d74d41ab5d80ac8f2`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf525cafee47f341c3c95e742264c04417841f805670bbf8696bdcc8668082d`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 9.1 MB (9109448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2f405bb85fe91994888d7507dd0641b3db43930cf575311ec56af1eead91bd`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 12.6 MB (12622917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373e62ddc7e7489f78a881fa66963be9043dc35ca8e4f345f1d7623af4444fcc`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.5-git`

```console
$ docker pull docker@sha256:8b7d15b6cf2118ec104cae6af089d5a9e25f26c687244a2ff93434d10203aa67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03.5-git` - linux; amd64

```console
$ docker pull docker@sha256:64c5cef8dc95f84402635d52a1970f958cec67091c18faf4ccd67eeeb53cbf08
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77246911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eab302e671fdaea238f1049815cb3a36f892ca5499535b6ac80cb6dddb25016`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:50 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f18ea2cbac4c4171b630fa800f91a1cb433728e55ebf865c4e560df098f16d`  
		Last Modified: Sat, 18 Jan 2020 04:43:42 GMT  
		Size: 8.2 MB (8213887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d7464319797cdc81c2a14d9a7c7cbf33afc28d80f08ad9c17ddf543d0d14d6d4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72347135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c3149aca6d91cef011b6ae505719d9294f0cfc56f9c3ec27e89d06e5248ff9`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:56 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25f25e40a87dd2b1e9da8caeaa383822f1194959380646fd4b91816d0fdfb9b`  
		Last Modified: Sat, 18 Jan 2020 05:55:11 GMT  
		Size: 7.8 MB (7835194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:b13771936ea2943baad627ff2354ef3a37b33729054081807f03f756379891de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71280905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10013a543102f31972358bdebe7ab2982abd88ca34247df0d6795f042eca2a0e`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:03:02 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febf3eb0506dfc4914c9b895325fecdb22a9f7545f259026158f6ed3e951bd0b`  
		Last Modified: Sat, 18 Jan 2020 03:04:19 GMT  
		Size: 7.1 MB (7072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d833dbf8e852bcebee568d846c92b5dfdac913bfe5c798b9cddba14b0b0c5cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70582903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa0741e9eec3e5cff51d73a17e11ae2068efc7c31fdb5eb995e7420e100c1af`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:50 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb377abbe251ebb2800e09dd698c95aaabf1a718ab29100760305b15b5a69c`  
		Last Modified: Sat, 18 Jan 2020 02:26:34 GMT  
		Size: 8.4 MB (8406028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.6-rc1`

**does not exist** (yet?)

## `docker:19.03.6-rc1-dind`

**does not exist** (yet?)

## `docker:19.03.6-rc1-dind-rootless`

**does not exist** (yet?)

## `docker:19.03.6-rc1-git`

**does not exist** (yet?)

## `docker:19.03-dind`

```console
$ docker pull docker@sha256:033ba84f8ea98910d8fc51b8263fbeb24c48d6daf55ef7c654e2981784dac2f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-dind` - linux; amd64

```console
$ docker pull docker@sha256:efd3d1db027f0c8d2cc7019b5381fc9c3cdbbda3642c3ef4feefe5a36cbf0769
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74624904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8489eeb24a264b6bcdb17f3da00140cebe92ee36bd22365f37d07d59390df4ee`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:1e319d9500b33aea20e9c76900595c113e652ebf38ed7021f5daf0e5d78f48af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67731913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6bc19942666d644c636de3a0210745329f07a4c2d3f32c3e9cbd7454e1228c`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 05:53:41 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 05:53:41 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 05:53:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 05:53:44 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:45 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 05:53:46 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 05:53:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:47 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6186deaef3161317f61f202acfab3875747c2a724fad1a65f29f18b068a9ca6c`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 3.2 MB (3215383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6fa6e67b938d446f54f8d3a432d35377ff3431821d39ea805fb2de790ef343`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00bcda5d341dc29b37b45898451e3133f9d420af32d36b21c94d30ac2429ed6`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 749.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daeb323203a88ce4e9152363b7ea9dc8c97580d9723309e442b2c170beb2815`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:7e8985ea07f8786be5b7c551d9547aac01e43a74e8a5831685b39d40fda6d3c6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67091202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef820b49fd591346a99dec34fab401da3022b7cbd60eb8d06f9baef8872d9f3`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:02:23 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 03:02:28 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 03:02:31 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 03:02:36 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 03:02:38 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:02:41 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 03:02:43 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 03:02:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:49 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cb30959a65f691f18075812bbdb8d5f87f944b6d8012dbce90e70e61de7c17`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 2.9 MB (2878527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4bdbf92a47a6e710c3aa65a5fbe9136e986509ab9dacdb67a196fa99441578`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ee73f368ab0a867e3f6b7294736b2ea3263dbf8cc5e6881a1b68ff5856a5c7`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 752.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0bf5e1afaa1f42f73b39a23c9e2203e65c65f6246e63d17ae6def1232a6c5b`  
		Last Modified: Sat, 18 Jan 2020 03:04:00 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31f0251cf185d41e1b6f25bf8acf3d816a73d1d8e583b4c72321a7ccc05801e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67770716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53793fffe26de8f80d9cdfa58c38018e90af8d08eb3f44ebedc03079b7d04d`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 02:24:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 02:24:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 02:24:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 02:24:22 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:24:25 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 02:24:26 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 02:24:30 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 02:24:33 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4704739272105dd3fdfc8614ba689cffe338a0faddc99dace44e191c4567ce`  
		Last Modified: Sat, 18 Jan 2020 02:26:12 GMT  
		Size: 5.6 MB (5589240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8637fb5dd84f5ab45114fc090fda27e2eee33b46a01802c9853a3d0c1b623`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab01413155fcbeedeee71c38d84c48825794515972fd5480a22210379d739d0a`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9514c7ce5d1ffef3aa0a3d41faed1d3ac1e700f99f71157dd4e7d6c418b01de`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind-rootless`

```console
$ docker pull docker@sha256:51f925a59f79f9f85b4869649f6bec7bed065f381186f4102c942ddd4a861cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:966cb6bf3b3955ebda64d4e156870e68e3ce20ac9c84a01dee28803aebc334af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97154857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384deac7f3c53083e5d29d8e56a0fa57afa7d88db3c4c34a80c774852f789d26`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
CMD []
# Sat, 18 Jan 2020 04:42:28 GMT
RUN apk add --no-cache iproute2
# Sat, 18 Jan 2020 04:42:29 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Sat, 18 Jan 2020 04:42:30 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Sat, 18 Jan 2020 04:42:32 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Sat, 18 Jan 2020 04:42:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Sat, 18 Jan 2020 04:42:44 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Sat, 18 Jan 2020 04:42:44 GMT
VOLUME [/home/rootless/.local/share/docker]
# Sat, 18 Jan 2020 04:42:44 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cdf1bd44b48b8727fa4bb0545240435dcf820156f0408b1bc13c094f8c01ea`  
		Last Modified: Sat, 18 Jan 2020 04:43:31 GMT  
		Size: 796.0 KB (795977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2313da576c87883442d37ff3743eacdb90d03a6928e9296f65a1083828ffc33`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b530e16b9b04d347cb7c9c99bfa6e4929f67f58f26d1d74d41ab5d80ac8f2`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf525cafee47f341c3c95e742264c04417841f805670bbf8696bdcc8668082d`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 9.1 MB (9109448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2f405bb85fe91994888d7507dd0641b3db43930cf575311ec56af1eead91bd`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 12.6 MB (12622917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373e62ddc7e7489f78a881fa66963be9043dc35ca8e4f345f1d7623af4444fcc`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-git`

```console
$ docker pull docker@sha256:8b7d15b6cf2118ec104cae6af089d5a9e25f26c687244a2ff93434d10203aa67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-git` - linux; amd64

```console
$ docker pull docker@sha256:64c5cef8dc95f84402635d52a1970f958cec67091c18faf4ccd67eeeb53cbf08
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77246911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eab302e671fdaea238f1049815cb3a36f892ca5499535b6ac80cb6dddb25016`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:50 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f18ea2cbac4c4171b630fa800f91a1cb433728e55ebf865c4e560df098f16d`  
		Last Modified: Sat, 18 Jan 2020 04:43:42 GMT  
		Size: 8.2 MB (8213887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d7464319797cdc81c2a14d9a7c7cbf33afc28d80f08ad9c17ddf543d0d14d6d4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72347135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c3149aca6d91cef011b6ae505719d9294f0cfc56f9c3ec27e89d06e5248ff9`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:56 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25f25e40a87dd2b1e9da8caeaa383822f1194959380646fd4b91816d0fdfb9b`  
		Last Modified: Sat, 18 Jan 2020 05:55:11 GMT  
		Size: 7.8 MB (7835194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:b13771936ea2943baad627ff2354ef3a37b33729054081807f03f756379891de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71280905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10013a543102f31972358bdebe7ab2982abd88ca34247df0d6795f042eca2a0e`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:03:02 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febf3eb0506dfc4914c9b895325fecdb22a9f7545f259026158f6ed3e951bd0b`  
		Last Modified: Sat, 18 Jan 2020 03:04:19 GMT  
		Size: 7.1 MB (7072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d833dbf8e852bcebee568d846c92b5dfdac913bfe5c798b9cddba14b0b0c5cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70582903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa0741e9eec3e5cff51d73a17e11ae2068efc7c31fdb5eb995e7420e100c1af`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:50 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb377abbe251ebb2800e09dd698c95aaabf1a718ab29100760305b15b5a69c`  
		Last Modified: Sat, 18 Jan 2020 02:26:34 GMT  
		Size: 8.4 MB (8406028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-rc`

```console
$ docker pull docker@sha256:0937e7454b5c442713bdf91760e129d75cd1b84b1574819255a63e296f776f4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-rc` - linux; amd64

```console
$ docker pull docker@sha256:429ae05e87d1b4fc006c33dc64a9d78b3439971c85e23a5594eed899f81c18cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66895480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df10864a388d6f2b4a7996b89033d694bf7bc4a6406bb2d6481b0fae5015437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:25:35 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:25:25 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:25:30 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:25:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:31 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d00f109003f5dd9e123c11faa3270ff5790e2e94cc062ac33acd54317e15e5`  
		Last Modified: Tue, 12 Nov 2019 00:26:53 GMT  
		Size: 63.8 MB (63804789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c3bf8eedaf11dca42c6bdd3160a31267b056f30138e9a83ae6291d7a50d712`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea408e741e559862add2ec71bc27aa6e6a9d6cc900bb7ff5399a3f221c850f4`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d3ea9ec8d1db322186cdbecdc3bffb283e8b87e2f59adfa5ed06c40e9f5f40`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc` - linux; arm variant v6

```console
$ docker pull docker@sha256:4eb44a6c9dbaf95151e7abf1ddc5e5742c4113528548dbe30d0e9ff1e9cc086b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62410589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91b16b4d3a3c41a4695ac30ca628198e887fe93d7171140b902766f39002332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 16:57:30 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 16:57:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:52:42 GMT
ENV DOCKER_CHANNEL=test
# Mon, 11 Nov 2019 23:49:32 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Mon, 11 Nov 2019 23:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 11 Nov 2019 23:49:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 11 Nov 2019 23:49:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 11 Nov 2019 23:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Nov 2019 23:49:47 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4d69e9c49d276dea623c6b05666752b107b3ae7e7fb31faa84c28a89270f7a`  
		Last Modified: Mon, 21 Oct 2019 17:01:55 GMT  
		Size: 302.0 KB (302014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665e2d25121195adad669aa3560768041a5fd3998c859fd6b324c11aac41e3f`  
		Last Modified: Mon, 21 Oct 2019 17:01:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5345f78e94b47be6a4174eaaaa15c5fb58d9d1bee49039f44bd5428cbfd8a10`  
		Last Modified: Mon, 11 Nov 2019 23:51:06 GMT  
		Size: 59.5 MB (59535399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104cd1a725a545c203fc7d69c58ada07ac323e87fad7846f6f7aaffe65899e26`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada593112b1c758ccc55294ec50129d346bc6af329c4f6d9c0855b8d8dad4b40`  
		Last Modified: Mon, 11 Nov 2019 23:50:45 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d393f5a61ff5c52d44b3b7aba3590517be98d59eb54d6039ef1066dc9155642`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc` - linux; arm variant v7

```console
$ docker pull docker@sha256:bae935201bf2ce20863bda3b0af2bd1130f3184ab475dbb38877e2652bc16468
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62213367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4b39e687f75980c5af6356d66962c30a63014c1f3f4f882547332fe8827bb3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:52:36 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:52:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:14:58 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:03:39 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:03:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:03:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:03:50 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:03:50 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:03:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:03:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:03:53 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417fcb3850a7455af93e93458e59d7f95bdbb16f1857e99d901142c8d2095eb`  
		Last Modified: Mon, 21 Oct 2019 18:54:57 GMT  
		Size: 300.9 KB (300946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a6ddf38e7cc67bd2f493ebb023839b57b404cc2299f2326c1771c3d559deda`  
		Last Modified: Mon, 21 Oct 2019 18:54:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3849a5e202f85a65a5ad9c6fe517da4209b9c38fa833e3192611a39ef0f94c3`  
		Last Modified: Tue, 12 Nov 2019 00:05:20 GMT  
		Size: 59.5 MB (59532118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea1770de5c377d031e6c7acb30e97987f723c4dad685fe266ac393bf7569a48`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a467e1c8e0b94cc0393bf55890dfc44d81df25c5be86ee01126e96878c0aa655`  
		Last Modified: Tue, 12 Nov 2019 00:04:59 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c668020528b34e7e638923d6cc2b9f90d00fdd2bf18c2973d2375dfa1439e02`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:82e9b3a5a3ab224844184d2450160aaaedca60676a457f8b9ed8c91f6873e150
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60026907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b581f22d584db1363f4ea1fadc653263ef374a4b32aa81875a2c59a3cae1eeba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:13 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:59:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:47:08 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:41:27 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:41:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:41:35 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:41:36 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:41:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:41:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:41:47 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d523c651118b8110a7055546123bb301485868b779462028d410ad31ce758844`  
		Last Modified: Mon, 21 Oct 2019 19:00:39 GMT  
		Size: 302.3 KB (302343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c404896130ad49e5b0a29fef854c53e121f275ffdd3c624399291cdb710c7`  
		Last Modified: Mon, 21 Oct 2019 19:00:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0ba3badd15b680ea219b55b068bd29a785f18b5d643ddb3bd654bc8d33b46d`  
		Last Modified: Tue, 12 Nov 2019 00:43:18 GMT  
		Size: 57.0 MB (57004922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bad5a8e310ac5b16ebbdbdfa2f613f240e09a5e0c14bc1d543034ea5d420da`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d91f3b8cbf514007493a365e75eb6fc43387856d3158724c425c3958914c11`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa64a18183f137480ac54f7b70a4caa1b3c9d69b76e6210ba3c5160dc06dd9f2`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-rc-dind`

```console
$ docker pull docker@sha256:cdc341d9ad19860700f550ed5bd8d913eacb65738735c0e0b57f1818da51aeac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:784eb8916b691a333effec393964ec085d7523c7a8a257d55a3685c7a6928b98
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72393382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447d74b8707445b802067e1c4ad4d8060333eddad1eb8e059c63e55573c0c721`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:25:35 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:25:25 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:25:30 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:25:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:31 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:25:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 12 Nov 2019 00:25:37 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:25:37 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 12 Nov 2019 00:25:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 12 Nov 2019 00:25:38 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:38 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Nov 2019 00:25:39 GMT
EXPOSE 2375 2376
# Tue, 12 Nov 2019 00:25:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:39 GMT
CMD []
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d00f109003f5dd9e123c11faa3270ff5790e2e94cc062ac33acd54317e15e5`  
		Last Modified: Tue, 12 Nov 2019 00:26:53 GMT  
		Size: 63.8 MB (63804789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c3bf8eedaf11dca42c6bdd3160a31267b056f30138e9a83ae6291d7a50d712`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea408e741e559862add2ec71bc27aa6e6a9d6cc900bb7ff5399a3f221c850f4`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d3ea9ec8d1db322186cdbecdc3bffb283e8b87e2f59adfa5ed06c40e9f5f40`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8c4e1a890d6df2310dec90af1a5d6cb0889567e89206389d1873470591a8eb`  
		Last Modified: Tue, 12 Nov 2019 00:27:01 GMT  
		Size: 5.5 MB (5493300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b345be14caeab88468bbf27dc41c5b8751fdfce83312288386288d471f9ec8d0`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e22df429876fd6d189c1fa3bc8f82b66195923ec8881a14f78df16682a59df2`  
		Last Modified: Tue, 12 Nov 2019 00:27:00 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915977ae9ff10b427ff17d4c9152d37ee3575c87d72b5da2b7c68cd0b9556f84`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:8ff42a3c45326fc4dd29b660c134d32aee284db1bddce6d523fde211cd02525e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65490814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68b182842a630efa2a6978365ca604ee7764789c4d6c5c8d0d5a5c1326d32f88`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 16:57:30 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 16:57:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:52:42 GMT
ENV DOCKER_CHANNEL=test
# Mon, 11 Nov 2019 23:49:32 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Mon, 11 Nov 2019 23:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 11 Nov 2019 23:49:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 11 Nov 2019 23:49:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 11 Nov 2019 23:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Nov 2019 23:49:47 GMT
CMD ["sh"]
# Mon, 11 Nov 2019 23:49:56 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 11 Nov 2019 23:49:57 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 11 Nov 2019 23:49:58 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Mon, 11 Nov 2019 23:50:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 11 Nov 2019 23:50:00 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Mon, 11 Nov 2019 23:50:01 GMT
VOLUME [/var/lib/docker]
# Mon, 11 Nov 2019 23:50:01 GMT
EXPOSE 2375 2376
# Mon, 11 Nov 2019 23:50:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 11 Nov 2019 23:50:03 GMT
CMD []
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4d69e9c49d276dea623c6b05666752b107b3ae7e7fb31faa84c28a89270f7a`  
		Last Modified: Mon, 21 Oct 2019 17:01:55 GMT  
		Size: 302.0 KB (302014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665e2d25121195adad669aa3560768041a5fd3998c859fd6b324c11aac41e3f`  
		Last Modified: Mon, 21 Oct 2019 17:01:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5345f78e94b47be6a4174eaaaa15c5fb58d9d1bee49039f44bd5428cbfd8a10`  
		Last Modified: Mon, 11 Nov 2019 23:51:06 GMT  
		Size: 59.5 MB (59535399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104cd1a725a545c203fc7d69c58ada07ac323e87fad7846f6f7aaffe65899e26`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada593112b1c758ccc55294ec50129d346bc6af329c4f6d9c0855b8d8dad4b40`  
		Last Modified: Mon, 11 Nov 2019 23:50:45 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d393f5a61ff5c52d44b3b7aba3590517be98d59eb54d6039ef1066dc9155642`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0c68e9126ceb889937e4ea4bc5f7073c7134e4feaa4a8ce3bd770b8ee12ae3`  
		Last Modified: Mon, 11 Nov 2019 23:51:19 GMT  
		Size: 3.1 MB (3075592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4646adc61add069716773e72c89f35a80ce16b9392c875cc78c9f18a3691ac`  
		Last Modified: Mon, 11 Nov 2019 23:51:19 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a02871256dc25be5c8def5d731ac9c1bb0296584d14acf545dc8e746828dd`  
		Last Modified: Mon, 11 Nov 2019 23:51:19 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75185c1e06a9732ec086ddcaa667bf3af3e0ff1e870ffee397894572c0eb1a6e`  
		Last Modified: Mon, 11 Nov 2019 23:51:19 GMT  
		Size: 2.5 KB (2538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:d6e44edcbb81b7ef0cd084eea51510a7e8125a41cd71e1d5706b2a5c67c07100
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64963156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:961a08e3b30bee562c2e7754c058fc84faac7a521bbeaf666b3a2192064fda84`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:52:36 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:52:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:14:58 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:03:39 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:03:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:03:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:03:50 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:03:50 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:03:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:03:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:03:53 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:04:03 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 12 Nov 2019 00:04:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:04:06 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 12 Nov 2019 00:04:08 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 12 Nov 2019 00:04:09 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:04:09 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Nov 2019 00:04:10 GMT
EXPOSE 2375 2376
# Tue, 12 Nov 2019 00:04:11 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Nov 2019 00:04:11 GMT
CMD []
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417fcb3850a7455af93e93458e59d7f95bdbb16f1857e99d901142c8d2095eb`  
		Last Modified: Mon, 21 Oct 2019 18:54:57 GMT  
		Size: 300.9 KB (300946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a6ddf38e7cc67bd2f493ebb023839b57b404cc2299f2326c1771c3d559deda`  
		Last Modified: Mon, 21 Oct 2019 18:54:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3849a5e202f85a65a5ad9c6fe517da4209b9c38fa833e3192611a39ef0f94c3`  
		Last Modified: Tue, 12 Nov 2019 00:05:20 GMT  
		Size: 59.5 MB (59532118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea1770de5c377d031e6c7acb30e97987f723c4dad685fe266ac393bf7569a48`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a467e1c8e0b94cc0393bf55890dfc44d81df25c5be86ee01126e96878c0aa655`  
		Last Modified: Tue, 12 Nov 2019 00:04:59 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c668020528b34e7e638923d6cc2b9f90d00fdd2bf18c2973d2375dfa1439e02`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14053bfa3cac76e398dfbe6ccd2ca36eb6765a62c5e61a37bed8243383f5cba7`  
		Last Modified: Tue, 12 Nov 2019 00:05:30 GMT  
		Size: 2.7 MB (2745159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cf65faffbd73e9d6805706b582f930971da640840df9ea0086abf07606f03b`  
		Last Modified: Tue, 12 Nov 2019 00:05:29 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe602a0da610d6505478af90b66a8605fd6fdfc762600e0ac97632182c37def7`  
		Last Modified: Tue, 12 Nov 2019 00:05:29 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d27f6ac9848db30122bcaba288d55026f2a85f8dabc5180d12c6d50de078b25`  
		Last Modified: Tue, 12 Nov 2019 00:05:29 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:ca575c4e6936224e14390fa32d0689cbbabb76da8276593fd3a26219e9038c18
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65554058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:069183d331a4c7faaaf80de3d973255647b6e1df0f16168d6d4eef469d0d1b4d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:13 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:59:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:47:08 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:41:27 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:41:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:41:35 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:41:36 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:41:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:41:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:41:47 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:42:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 12 Nov 2019 00:42:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:42:06 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 12 Nov 2019 00:42:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 12 Nov 2019 00:42:09 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:42:11 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Nov 2019 00:42:11 GMT
EXPOSE 2375 2376
# Tue, 12 Nov 2019 00:42:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Nov 2019 00:42:13 GMT
CMD []
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d523c651118b8110a7055546123bb301485868b779462028d410ad31ce758844`  
		Last Modified: Mon, 21 Oct 2019 19:00:39 GMT  
		Size: 302.3 KB (302343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c404896130ad49e5b0a29fef854c53e121f275ffdd3c624399291cdb710c7`  
		Last Modified: Mon, 21 Oct 2019 19:00:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0ba3badd15b680ea219b55b068bd29a785f18b5d643ddb3bd654bc8d33b46d`  
		Last Modified: Tue, 12 Nov 2019 00:43:18 GMT  
		Size: 57.0 MB (57004922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bad5a8e310ac5b16ebbdbdfa2f613f240e09a5e0c14bc1d543034ea5d420da`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d91f3b8cbf514007493a365e75eb6fc43387856d3158724c425c3958914c11`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa64a18183f137480ac54f7b70a4caa1b3c9d69b76e6210ba3c5160dc06dd9f2`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b067cebdc3e51c1be42460d99d0471c64f4d5d7adb24af16e92c917d13d4c2dc`  
		Last Modified: Tue, 12 Nov 2019 00:43:30 GMT  
		Size: 5.5 MB (5522518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bc0d47be907d032606231e020caff4bd1c2306601748c3a944381deb943974`  
		Last Modified: Tue, 12 Nov 2019 00:43:28 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a98c342e8c81b034629e96469522ce3bf70e6af9a0a79bbdfcd52e0352106ee`  
		Last Modified: Tue, 12 Nov 2019 00:43:28 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f9a38e3d6220a6aea668779fa7c6c4cf8f1b7820b7815f6d0f7191f825556e`  
		Last Modified: Tue, 12 Nov 2019 00:43:28 GMT  
		Size: 2.5 KB (2538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-rc-dind-rootless`

```console
$ docker pull docker@sha256:f066ad6c74a4c14595f66f14589a70da93d5f76c02c15752f6c9ae195b5b0c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03-rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:3528a31cd28a813dc89e8180903f82b10170239a14bf14a08b9c03ce43b700a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94645373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7910b59ec98e75afa6b8c9f24f47fb741ac9383f43ee11e7ccdf790a0e2c01d9`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:25:35 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:25:25 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:25:30 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:25:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:31 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:25:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 12 Nov 2019 00:25:37 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:25:37 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 12 Nov 2019 00:25:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 12 Nov 2019 00:25:38 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:38 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Nov 2019 00:25:39 GMT
EXPOSE 2375 2376
# Tue, 12 Nov 2019 00:25:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:39 GMT
CMD []
# Tue, 12 Nov 2019 00:25:44 GMT
RUN apk add --no-cache iproute2
# Tue, 12 Nov 2019 00:25:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 12 Nov 2019 00:25:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:25:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Tue, 12 Nov 2019 00:25:47 GMT
ENV ROOTLESSKIT_VERSION=0.6.0
# Tue, 12 Nov 2019 00:25:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Tue, 12 Nov 2019 00:25:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 12 Nov 2019 00:25:59 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 12 Nov 2019 00:25:59 GMT
USER rootless
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d00f109003f5dd9e123c11faa3270ff5790e2e94cc062ac33acd54317e15e5`  
		Last Modified: Tue, 12 Nov 2019 00:26:53 GMT  
		Size: 63.8 MB (63804789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c3bf8eedaf11dca42c6bdd3160a31267b056f30138e9a83ae6291d7a50d712`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea408e741e559862add2ec71bc27aa6e6a9d6cc900bb7ff5399a3f221c850f4`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d3ea9ec8d1db322186cdbecdc3bffb283e8b87e2f59adfa5ed06c40e9f5f40`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8c4e1a890d6df2310dec90af1a5d6cb0889567e89206389d1873470591a8eb`  
		Last Modified: Tue, 12 Nov 2019 00:27:01 GMT  
		Size: 5.5 MB (5493300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b345be14caeab88468bbf27dc41c5b8751fdfce83312288386288d471f9ec8d0`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e22df429876fd6d189c1fa3bc8f82b66195923ec8881a14f78df16682a59df2`  
		Last Modified: Tue, 12 Nov 2019 00:27:00 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915977ae9ff10b427ff17d4c9152d37ee3575c87d72b5da2b7c68cd0b9556f84`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32795880a521eae7582c0270f900fcac318a148e278f3c5f2056dbecb566c6ae`  
		Last Modified: Tue, 12 Nov 2019 00:27:08 GMT  
		Size: 722.6 KB (722572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c19ee2832c7580babdc0b08bef1837a9639bf2b7efb302d9f800fd400a53c5`  
		Last Modified: Tue, 12 Nov 2019 00:27:06 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5d7916f8600113e56597d04afd6d8d01dfa266fbc832988789b17a50764f97`  
		Last Modified: Tue, 12 Nov 2019 00:27:06 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a06f686027b0f516409ec930965e0510b34ea75f88542df6762cbc226bead62`  
		Last Modified: Tue, 12 Nov 2019 00:27:09 GMT  
		Size: 9.1 MB (9109464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60c15bf7903b46f98edc01a329c0de68aedd24774de6fcb278c1897cd6aa1bb`  
		Last Modified: Tue, 12 Nov 2019 00:27:08 GMT  
		Size: 12.4 MB (12418316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542afa5f61c8214b17bf510810c9d3147ea3de49c53bfb4adc049a62bfc9e7ae`  
		Last Modified: Tue, 12 Nov 2019 00:27:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-rc-git`

```console
$ docker pull docker@sha256:53dcde16046479558fc598170a2a31d4177175b6b7f38cd94dd4881bcbfd7c40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-rc-git` - linux; amd64

```console
$ docker pull docker@sha256:d599afcdd9c35ac777f5cc0ceac1a9bb5f84be9988ff2a86bd30cb1a36cc122b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76799809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55a0e0e0041238f292ea566db38d2571383c905fa20414dc2d12574e8ab327b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:25:35 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:25:25 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:25:30 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:25:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:31 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:26:06 GMT
RUN apk add --no-cache 		git 		openssh-client
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d00f109003f5dd9e123c11faa3270ff5790e2e94cc062ac33acd54317e15e5`  
		Last Modified: Tue, 12 Nov 2019 00:26:53 GMT  
		Size: 63.8 MB (63804789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c3bf8eedaf11dca42c6bdd3160a31267b056f30138e9a83ae6291d7a50d712`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea408e741e559862add2ec71bc27aa6e6a9d6cc900bb7ff5399a3f221c850f4`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d3ea9ec8d1db322186cdbecdc3bffb283e8b87e2f59adfa5ed06c40e9f5f40`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1acd9de865848d52af16bf1e2c115fe0f53c16e547d44c7173b4741003bd9`  
		Last Modified: Tue, 12 Nov 2019 00:27:17 GMT  
		Size: 9.9 MB (9904329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:8c7f68f26d9236b945df3d7a0c4eda32eab25f583607c51f49548458cca4627b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71797181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a839ea0e09d70a66d2b3ead5a5ff13d627accbe2e4e5845bc7e0dd5c29040e31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 16:57:30 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 16:57:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:52:42 GMT
ENV DOCKER_CHANNEL=test
# Mon, 11 Nov 2019 23:49:32 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Mon, 11 Nov 2019 23:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 11 Nov 2019 23:49:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 11 Nov 2019 23:49:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 11 Nov 2019 23:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Nov 2019 23:49:47 GMT
CMD ["sh"]
# Mon, 11 Nov 2019 23:50:12 GMT
RUN apk add --no-cache 		git 		openssh-client
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4d69e9c49d276dea623c6b05666752b107b3ae7e7fb31faa84c28a89270f7a`  
		Last Modified: Mon, 21 Oct 2019 17:01:55 GMT  
		Size: 302.0 KB (302014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665e2d25121195adad669aa3560768041a5fd3998c859fd6b324c11aac41e3f`  
		Last Modified: Mon, 21 Oct 2019 17:01:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5345f78e94b47be6a4174eaaaa15c5fb58d9d1bee49039f44bd5428cbfd8a10`  
		Last Modified: Mon, 11 Nov 2019 23:51:06 GMT  
		Size: 59.5 MB (59535399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104cd1a725a545c203fc7d69c58ada07ac323e87fad7846f6f7aaffe65899e26`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada593112b1c758ccc55294ec50129d346bc6af329c4f6d9c0855b8d8dad4b40`  
		Last Modified: Mon, 11 Nov 2019 23:50:45 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d393f5a61ff5c52d44b3b7aba3590517be98d59eb54d6039ef1066dc9155642`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226cf46f7d3e794e14a6b1e83cf1f9ea93a3e08026b725f05f03cb2a2dec44b4`  
		Last Modified: Mon, 11 Nov 2019 23:51:31 GMT  
		Size: 9.4 MB (9386592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:c7fcc64622440705eab3d9907b58e7aa69eb77578666cbf04c41b132b5be9f7b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70669783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0afd2582713dc5c58c7177cd04f57d8a5f2f394d7a38b4d32e81f1d4a235c0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:52:36 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:52:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:14:58 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:03:39 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:03:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:03:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:03:50 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:03:50 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:03:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:03:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:03:53 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:04:23 GMT
RUN apk add --no-cache 		git 		openssh-client
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417fcb3850a7455af93e93458e59d7f95bdbb16f1857e99d901142c8d2095eb`  
		Last Modified: Mon, 21 Oct 2019 18:54:57 GMT  
		Size: 300.9 KB (300946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a6ddf38e7cc67bd2f493ebb023839b57b404cc2299f2326c1771c3d559deda`  
		Last Modified: Mon, 21 Oct 2019 18:54:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3849a5e202f85a65a5ad9c6fe517da4209b9c38fa833e3192611a39ef0f94c3`  
		Last Modified: Tue, 12 Nov 2019 00:05:20 GMT  
		Size: 59.5 MB (59532118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea1770de5c377d031e6c7acb30e97987f723c4dad685fe266ac393bf7569a48`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a467e1c8e0b94cc0393bf55890dfc44d81df25c5be86ee01126e96878c0aa655`  
		Last Modified: Tue, 12 Nov 2019 00:04:59 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c668020528b34e7e638923d6cc2b9f90d00fdd2bf18c2973d2375dfa1439e02`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79407638a2835a9aecac1a9df3716130d77061023173d124a092b56cb4500b39`  
		Last Modified: Tue, 12 Nov 2019 00:05:45 GMT  
		Size: 8.5 MB (8456416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:049c58b05337d3882755a6bab40de2fffeb1f2b24f975ac0ab74172588cdb632
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70192134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e589cc3d723bfd13bd500b5e2389e3de9d52d002ce8449b94eb52f14ab525b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:13 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:59:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:47:08 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:41:27 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:41:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:41:35 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:41:36 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:41:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:41:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:41:47 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:42:22 GMT
RUN apk add --no-cache 		git 		openssh-client
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d523c651118b8110a7055546123bb301485868b779462028d410ad31ce758844`  
		Last Modified: Mon, 21 Oct 2019 19:00:39 GMT  
		Size: 302.3 KB (302343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c404896130ad49e5b0a29fef854c53e121f275ffdd3c624399291cdb710c7`  
		Last Modified: Mon, 21 Oct 2019 19:00:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0ba3badd15b680ea219b55b068bd29a785f18b5d643ddb3bd654bc8d33b46d`  
		Last Modified: Tue, 12 Nov 2019 00:43:18 GMT  
		Size: 57.0 MB (57004922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bad5a8e310ac5b16ebbdbdfa2f613f240e09a5e0c14bc1d543034ea5d420da`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d91f3b8cbf514007493a365e75eb6fc43387856d3158724c425c3958914c11`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa64a18183f137480ac54f7b70a4caa1b3c9d69b76e6210ba3c5160dc06dd9f2`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9bfc23da2e6d49d0d1137456552f257b9eab32db0509a8bbb53458528f58df`  
		Last Modified: Tue, 12 Nov 2019 00:43:43 GMT  
		Size: 10.2 MB (10165227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind`

```console
$ docker pull docker@sha256:033ba84f8ea98910d8fc51b8263fbeb24c48d6daf55ef7c654e2981784dac2f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-dind` - linux; amd64

```console
$ docker pull docker@sha256:efd3d1db027f0c8d2cc7019b5381fc9c3cdbbda3642c3ef4feefe5a36cbf0769
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74624904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8489eeb24a264b6bcdb17f3da00140cebe92ee36bd22365f37d07d59390df4ee`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:1e319d9500b33aea20e9c76900595c113e652ebf38ed7021f5daf0e5d78f48af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67731913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6bc19942666d644c636de3a0210745329f07a4c2d3f32c3e9cbd7454e1228c`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 05:53:41 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 05:53:41 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 05:53:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 05:53:44 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:45 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 05:53:46 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 05:53:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:47 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6186deaef3161317f61f202acfab3875747c2a724fad1a65f29f18b068a9ca6c`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 3.2 MB (3215383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6fa6e67b938d446f54f8d3a432d35377ff3431821d39ea805fb2de790ef343`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00bcda5d341dc29b37b45898451e3133f9d420af32d36b21c94d30ac2429ed6`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 749.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daeb323203a88ce4e9152363b7ea9dc8c97580d9723309e442b2c170beb2815`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:7e8985ea07f8786be5b7c551d9547aac01e43a74e8a5831685b39d40fda6d3c6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67091202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef820b49fd591346a99dec34fab401da3022b7cbd60eb8d06f9baef8872d9f3`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:02:23 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 03:02:28 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 03:02:31 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 03:02:36 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 03:02:38 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:02:41 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 03:02:43 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 03:02:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:49 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cb30959a65f691f18075812bbdb8d5f87f944b6d8012dbce90e70e61de7c17`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 2.9 MB (2878527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4bdbf92a47a6e710c3aa65a5fbe9136e986509ab9dacdb67a196fa99441578`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ee73f368ab0a867e3f6b7294736b2ea3263dbf8cc5e6881a1b68ff5856a5c7`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 752.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0bf5e1afaa1f42f73b39a23c9e2203e65c65f6246e63d17ae6def1232a6c5b`  
		Last Modified: Sat, 18 Jan 2020 03:04:00 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31f0251cf185d41e1b6f25bf8acf3d816a73d1d8e583b4c72321a7ccc05801e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67770716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53793fffe26de8f80d9cdfa58c38018e90af8d08eb3f44ebedc03079b7d04d`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 02:24:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 02:24:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 02:24:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 02:24:22 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:24:25 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 02:24:26 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 02:24:30 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 02:24:33 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4704739272105dd3fdfc8614ba689cffe338a0faddc99dace44e191c4567ce`  
		Last Modified: Sat, 18 Jan 2020 02:26:12 GMT  
		Size: 5.6 MB (5589240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8637fb5dd84f5ab45114fc090fda27e2eee33b46a01802c9853a3d0c1b623`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab01413155fcbeedeee71c38d84c48825794515972fd5480a22210379d739d0a`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9514c7ce5d1ffef3aa0a3d41faed1d3ac1e700f99f71157dd4e7d6c418b01de`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:51f925a59f79f9f85b4869649f6bec7bed065f381186f4102c942ddd4a861cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:966cb6bf3b3955ebda64d4e156870e68e3ce20ac9c84a01dee28803aebc334af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97154857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384deac7f3c53083e5d29d8e56a0fa57afa7d88db3c4c34a80c774852f789d26`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
CMD []
# Sat, 18 Jan 2020 04:42:28 GMT
RUN apk add --no-cache iproute2
# Sat, 18 Jan 2020 04:42:29 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Sat, 18 Jan 2020 04:42:30 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Sat, 18 Jan 2020 04:42:32 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Sat, 18 Jan 2020 04:42:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Sat, 18 Jan 2020 04:42:44 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Sat, 18 Jan 2020 04:42:44 GMT
VOLUME [/home/rootless/.local/share/docker]
# Sat, 18 Jan 2020 04:42:44 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cdf1bd44b48b8727fa4bb0545240435dcf820156f0408b1bc13c094f8c01ea`  
		Last Modified: Sat, 18 Jan 2020 04:43:31 GMT  
		Size: 796.0 KB (795977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2313da576c87883442d37ff3743eacdb90d03a6928e9296f65a1083828ffc33`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b530e16b9b04d347cb7c9c99bfa6e4929f67f58f26d1d74d41ab5d80ac8f2`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf525cafee47f341c3c95e742264c04417841f805670bbf8696bdcc8668082d`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 9.1 MB (9109448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2f405bb85fe91994888d7507dd0641b3db43930cf575311ec56af1eead91bd`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 12.6 MB (12622917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373e62ddc7e7489f78a881fa66963be9043dc35ca8e4f345f1d7623af4444fcc`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-git`

```console
$ docker pull docker@sha256:8b7d15b6cf2118ec104cae6af089d5a9e25f26c687244a2ff93434d10203aa67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-git` - linux; amd64

```console
$ docker pull docker@sha256:64c5cef8dc95f84402635d52a1970f958cec67091c18faf4ccd67eeeb53cbf08
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77246911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eab302e671fdaea238f1049815cb3a36f892ca5499535b6ac80cb6dddb25016`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:50 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f18ea2cbac4c4171b630fa800f91a1cb433728e55ebf865c4e560df098f16d`  
		Last Modified: Sat, 18 Jan 2020 04:43:42 GMT  
		Size: 8.2 MB (8213887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d7464319797cdc81c2a14d9a7c7cbf33afc28d80f08ad9c17ddf543d0d14d6d4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72347135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c3149aca6d91cef011b6ae505719d9294f0cfc56f9c3ec27e89d06e5248ff9`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:56 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25f25e40a87dd2b1e9da8caeaa383822f1194959380646fd4b91816d0fdfb9b`  
		Last Modified: Sat, 18 Jan 2020 05:55:11 GMT  
		Size: 7.8 MB (7835194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:b13771936ea2943baad627ff2354ef3a37b33729054081807f03f756379891de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71280905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10013a543102f31972358bdebe7ab2982abd88ca34247df0d6795f042eca2a0e`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:03:02 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febf3eb0506dfc4914c9b895325fecdb22a9f7545f259026158f6ed3e951bd0b`  
		Last Modified: Sat, 18 Jan 2020 03:04:19 GMT  
		Size: 7.1 MB (7072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d833dbf8e852bcebee568d846c92b5dfdac913bfe5c798b9cddba14b0b0c5cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70582903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa0741e9eec3e5cff51d73a17e11ae2068efc7c31fdb5eb995e7420e100c1af`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:50 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb377abbe251ebb2800e09dd698c95aaabf1a718ab29100760305b15b5a69c`  
		Last Modified: Sat, 18 Jan 2020 02:26:34 GMT  
		Size: 8.4 MB (8406028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:033ba84f8ea98910d8fc51b8263fbeb24c48d6daf55ef7c654e2981784dac2f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:efd3d1db027f0c8d2cc7019b5381fc9c3cdbbda3642c3ef4feefe5a36cbf0769
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74624904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8489eeb24a264b6bcdb17f3da00140cebe92ee36bd22365f37d07d59390df4ee`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:1e319d9500b33aea20e9c76900595c113e652ebf38ed7021f5daf0e5d78f48af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67731913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6bc19942666d644c636de3a0210745329f07a4c2d3f32c3e9cbd7454e1228c`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 05:53:41 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 05:53:41 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 05:53:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 05:53:44 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:45 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 05:53:46 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 05:53:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:47 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6186deaef3161317f61f202acfab3875747c2a724fad1a65f29f18b068a9ca6c`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 3.2 MB (3215383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6fa6e67b938d446f54f8d3a432d35377ff3431821d39ea805fb2de790ef343`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00bcda5d341dc29b37b45898451e3133f9d420af32d36b21c94d30ac2429ed6`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 749.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daeb323203a88ce4e9152363b7ea9dc8c97580d9723309e442b2c170beb2815`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:7e8985ea07f8786be5b7c551d9547aac01e43a74e8a5831685b39d40fda6d3c6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67091202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef820b49fd591346a99dec34fab401da3022b7cbd60eb8d06f9baef8872d9f3`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:02:23 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 03:02:28 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 03:02:31 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 03:02:36 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 03:02:38 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:02:41 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 03:02:43 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 03:02:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:49 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cb30959a65f691f18075812bbdb8d5f87f944b6d8012dbce90e70e61de7c17`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 2.9 MB (2878527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4bdbf92a47a6e710c3aa65a5fbe9136e986509ab9dacdb67a196fa99441578`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ee73f368ab0a867e3f6b7294736b2ea3263dbf8cc5e6881a1b68ff5856a5c7`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 752.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0bf5e1afaa1f42f73b39a23c9e2203e65c65f6246e63d17ae6def1232a6c5b`  
		Last Modified: Sat, 18 Jan 2020 03:04:00 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31f0251cf185d41e1b6f25bf8acf3d816a73d1d8e583b4c72321a7ccc05801e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67770716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53793fffe26de8f80d9cdfa58c38018e90af8d08eb3f44ebedc03079b7d04d`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 02:24:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 02:24:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 02:24:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 02:24:22 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:24:25 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 02:24:26 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 02:24:30 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 02:24:33 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4704739272105dd3fdfc8614ba689cffe338a0faddc99dace44e191c4567ce`  
		Last Modified: Sat, 18 Jan 2020 02:26:12 GMT  
		Size: 5.6 MB (5589240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8637fb5dd84f5ab45114fc090fda27e2eee33b46a01802c9853a3d0c1b623`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab01413155fcbeedeee71c38d84c48825794515972fd5480a22210379d739d0a`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9514c7ce5d1ffef3aa0a3d41faed1d3ac1e700f99f71157dd4e7d6c418b01de`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:51f925a59f79f9f85b4869649f6bec7bed065f381186f4102c942ddd4a861cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:966cb6bf3b3955ebda64d4e156870e68e3ce20ac9c84a01dee28803aebc334af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97154857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384deac7f3c53083e5d29d8e56a0fa57afa7d88db3c4c34a80c774852f789d26`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
CMD []
# Sat, 18 Jan 2020 04:42:28 GMT
RUN apk add --no-cache iproute2
# Sat, 18 Jan 2020 04:42:29 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Sat, 18 Jan 2020 04:42:30 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Sat, 18 Jan 2020 04:42:32 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Sat, 18 Jan 2020 04:42:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Sat, 18 Jan 2020 04:42:44 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Sat, 18 Jan 2020 04:42:44 GMT
VOLUME [/home/rootless/.local/share/docker]
# Sat, 18 Jan 2020 04:42:44 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cdf1bd44b48b8727fa4bb0545240435dcf820156f0408b1bc13c094f8c01ea`  
		Last Modified: Sat, 18 Jan 2020 04:43:31 GMT  
		Size: 796.0 KB (795977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2313da576c87883442d37ff3743eacdb90d03a6928e9296f65a1083828ffc33`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b530e16b9b04d347cb7c9c99bfa6e4929f67f58f26d1d74d41ab5d80ac8f2`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf525cafee47f341c3c95e742264c04417841f805670bbf8696bdcc8668082d`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 9.1 MB (9109448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2f405bb85fe91994888d7507dd0641b3db43930cf575311ec56af1eead91bd`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 12.6 MB (12622917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373e62ddc7e7489f78a881fa66963be9043dc35ca8e4f345f1d7623af4444fcc`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:8b7d15b6cf2118ec104cae6af089d5a9e25f26c687244a2ff93434d10203aa67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:64c5cef8dc95f84402635d52a1970f958cec67091c18faf4ccd67eeeb53cbf08
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77246911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eab302e671fdaea238f1049815cb3a36f892ca5499535b6ac80cb6dddb25016`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:50 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f18ea2cbac4c4171b630fa800f91a1cb433728e55ebf865c4e560df098f16d`  
		Last Modified: Sat, 18 Jan 2020 04:43:42 GMT  
		Size: 8.2 MB (8213887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d7464319797cdc81c2a14d9a7c7cbf33afc28d80f08ad9c17ddf543d0d14d6d4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72347135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c3149aca6d91cef011b6ae505719d9294f0cfc56f9c3ec27e89d06e5248ff9`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:56 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25f25e40a87dd2b1e9da8caeaa383822f1194959380646fd4b91816d0fdfb9b`  
		Last Modified: Sat, 18 Jan 2020 05:55:11 GMT  
		Size: 7.8 MB (7835194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm variant v7

```console
$ docker pull docker@sha256:b13771936ea2943baad627ff2354ef3a37b33729054081807f03f756379891de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71280905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10013a543102f31972358bdebe7ab2982abd88ca34247df0d6795f042eca2a0e`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:03:02 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febf3eb0506dfc4914c9b895325fecdb22a9f7545f259026158f6ed3e951bd0b`  
		Last Modified: Sat, 18 Jan 2020 03:04:19 GMT  
		Size: 7.1 MB (7072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d833dbf8e852bcebee568d846c92b5dfdac913bfe5c798b9cddba14b0b0c5cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70582903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa0741e9eec3e5cff51d73a17e11ae2068efc7c31fdb5eb995e7420e100c1af`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:50 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb377abbe251ebb2800e09dd698c95aaabf1a718ab29100760305b15b5a69c`  
		Last Modified: Sat, 18 Jan 2020 02:26:34 GMT  
		Size: 8.4 MB (8406028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:0b90b0aefd15794e4d5bea2debc3b761c1d3481a92ec7166f8453652d0deba95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:48db0e29e2214d564b66daffc707ad290c8788dc655cea59c605f021790d38a0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69033024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c774f62a9b520060d72c3c1901facdfdfd0fc4ae7c5e817cdaf6acd456432c`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm variant v6

```console
$ docker pull docker@sha256:aa908727daa7433a0d156f6c6703fe5d945c4019e8b7f5d0c4fc8213e6d67fed
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64511941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e68c26581b5f619c73bdd54951308df6920447f7be745bea2bfbb6b3624b26`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm variant v7

```console
$ docker pull docker@sha256:ec6f3f2f65803962bd623ab2de639bd87d41d856c6ef477ae58383b379a1376a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64208081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fc3364d97bc6d5e8c8de60fa7c776bbc4eb6ca32c38029201f27c506086b11`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e09d98b19bbee9f15b9f66604d48401833716faef061e9e509b48fb8db8bd1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62176875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:466581031774ac8ddb27699e61f2fbf858fce357adad7352cc410ef9ad6344bf`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc`

```console
$ docker pull docker@sha256:0937e7454b5c442713bdf91760e129d75cd1b84b1574819255a63e296f776f4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:rc` - linux; amd64

```console
$ docker pull docker@sha256:429ae05e87d1b4fc006c33dc64a9d78b3439971c85e23a5594eed899f81c18cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66895480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df10864a388d6f2b4a7996b89033d694bf7bc4a6406bb2d6481b0fae5015437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:25:35 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:25:25 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:25:30 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:25:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:31 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d00f109003f5dd9e123c11faa3270ff5790e2e94cc062ac33acd54317e15e5`  
		Last Modified: Tue, 12 Nov 2019 00:26:53 GMT  
		Size: 63.8 MB (63804789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c3bf8eedaf11dca42c6bdd3160a31267b056f30138e9a83ae6291d7a50d712`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea408e741e559862add2ec71bc27aa6e6a9d6cc900bb7ff5399a3f221c850f4`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d3ea9ec8d1db322186cdbecdc3bffb283e8b87e2f59adfa5ed06c40e9f5f40`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm variant v6

```console
$ docker pull docker@sha256:4eb44a6c9dbaf95151e7abf1ddc5e5742c4113528548dbe30d0e9ff1e9cc086b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62410589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91b16b4d3a3c41a4695ac30ca628198e887fe93d7171140b902766f39002332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 16:57:30 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 16:57:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:52:42 GMT
ENV DOCKER_CHANNEL=test
# Mon, 11 Nov 2019 23:49:32 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Mon, 11 Nov 2019 23:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 11 Nov 2019 23:49:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 11 Nov 2019 23:49:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 11 Nov 2019 23:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Nov 2019 23:49:47 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4d69e9c49d276dea623c6b05666752b107b3ae7e7fb31faa84c28a89270f7a`  
		Last Modified: Mon, 21 Oct 2019 17:01:55 GMT  
		Size: 302.0 KB (302014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665e2d25121195adad669aa3560768041a5fd3998c859fd6b324c11aac41e3f`  
		Last Modified: Mon, 21 Oct 2019 17:01:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5345f78e94b47be6a4174eaaaa15c5fb58d9d1bee49039f44bd5428cbfd8a10`  
		Last Modified: Mon, 11 Nov 2019 23:51:06 GMT  
		Size: 59.5 MB (59535399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104cd1a725a545c203fc7d69c58ada07ac323e87fad7846f6f7aaffe65899e26`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada593112b1c758ccc55294ec50129d346bc6af329c4f6d9c0855b8d8dad4b40`  
		Last Modified: Mon, 11 Nov 2019 23:50:45 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d393f5a61ff5c52d44b3b7aba3590517be98d59eb54d6039ef1066dc9155642`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm variant v7

```console
$ docker pull docker@sha256:bae935201bf2ce20863bda3b0af2bd1130f3184ab475dbb38877e2652bc16468
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62213367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4b39e687f75980c5af6356d66962c30a63014c1f3f4f882547332fe8827bb3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:52:36 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:52:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:14:58 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:03:39 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:03:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:03:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:03:50 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:03:50 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:03:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:03:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:03:53 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417fcb3850a7455af93e93458e59d7f95bdbb16f1857e99d901142c8d2095eb`  
		Last Modified: Mon, 21 Oct 2019 18:54:57 GMT  
		Size: 300.9 KB (300946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a6ddf38e7cc67bd2f493ebb023839b57b404cc2299f2326c1771c3d559deda`  
		Last Modified: Mon, 21 Oct 2019 18:54:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3849a5e202f85a65a5ad9c6fe517da4209b9c38fa833e3192611a39ef0f94c3`  
		Last Modified: Tue, 12 Nov 2019 00:05:20 GMT  
		Size: 59.5 MB (59532118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea1770de5c377d031e6c7acb30e97987f723c4dad685fe266ac393bf7569a48`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a467e1c8e0b94cc0393bf55890dfc44d81df25c5be86ee01126e96878c0aa655`  
		Last Modified: Tue, 12 Nov 2019 00:04:59 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c668020528b34e7e638923d6cc2b9f90d00fdd2bf18c2973d2375dfa1439e02`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:82e9b3a5a3ab224844184d2450160aaaedca60676a457f8b9ed8c91f6873e150
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60026907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b581f22d584db1363f4ea1fadc653263ef374a4b32aa81875a2c59a3cae1eeba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:13 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:59:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:47:08 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:41:27 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:41:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:41:35 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:41:36 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:41:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:41:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:41:47 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d523c651118b8110a7055546123bb301485868b779462028d410ad31ce758844`  
		Last Modified: Mon, 21 Oct 2019 19:00:39 GMT  
		Size: 302.3 KB (302343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c404896130ad49e5b0a29fef854c53e121f275ffdd3c624399291cdb710c7`  
		Last Modified: Mon, 21 Oct 2019 19:00:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0ba3badd15b680ea219b55b068bd29a785f18b5d643ddb3bd654bc8d33b46d`  
		Last Modified: Tue, 12 Nov 2019 00:43:18 GMT  
		Size: 57.0 MB (57004922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bad5a8e310ac5b16ebbdbdfa2f613f240e09a5e0c14bc1d543034ea5d420da`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d91f3b8cbf514007493a365e75eb6fc43387856d3158724c425c3958914c11`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa64a18183f137480ac54f7b70a4caa1b3c9d69b76e6210ba3c5160dc06dd9f2`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-dind`

```console
$ docker pull docker@sha256:cdc341d9ad19860700f550ed5bd8d913eacb65738735c0e0b57f1818da51aeac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:784eb8916b691a333effec393964ec085d7523c7a8a257d55a3685c7a6928b98
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72393382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447d74b8707445b802067e1c4ad4d8060333eddad1eb8e059c63e55573c0c721`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:25:35 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:25:25 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:25:30 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:25:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:31 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:25:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 12 Nov 2019 00:25:37 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:25:37 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 12 Nov 2019 00:25:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 12 Nov 2019 00:25:38 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:38 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Nov 2019 00:25:39 GMT
EXPOSE 2375 2376
# Tue, 12 Nov 2019 00:25:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:39 GMT
CMD []
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d00f109003f5dd9e123c11faa3270ff5790e2e94cc062ac33acd54317e15e5`  
		Last Modified: Tue, 12 Nov 2019 00:26:53 GMT  
		Size: 63.8 MB (63804789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c3bf8eedaf11dca42c6bdd3160a31267b056f30138e9a83ae6291d7a50d712`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea408e741e559862add2ec71bc27aa6e6a9d6cc900bb7ff5399a3f221c850f4`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d3ea9ec8d1db322186cdbecdc3bffb283e8b87e2f59adfa5ed06c40e9f5f40`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8c4e1a890d6df2310dec90af1a5d6cb0889567e89206389d1873470591a8eb`  
		Last Modified: Tue, 12 Nov 2019 00:27:01 GMT  
		Size: 5.5 MB (5493300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b345be14caeab88468bbf27dc41c5b8751fdfce83312288386288d471f9ec8d0`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e22df429876fd6d189c1fa3bc8f82b66195923ec8881a14f78df16682a59df2`  
		Last Modified: Tue, 12 Nov 2019 00:27:00 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915977ae9ff10b427ff17d4c9152d37ee3575c87d72b5da2b7c68cd0b9556f84`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:8ff42a3c45326fc4dd29b660c134d32aee284db1bddce6d523fde211cd02525e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65490814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68b182842a630efa2a6978365ca604ee7764789c4d6c5c8d0d5a5c1326d32f88`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 16:57:30 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 16:57:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:52:42 GMT
ENV DOCKER_CHANNEL=test
# Mon, 11 Nov 2019 23:49:32 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Mon, 11 Nov 2019 23:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 11 Nov 2019 23:49:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 11 Nov 2019 23:49:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 11 Nov 2019 23:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Nov 2019 23:49:47 GMT
CMD ["sh"]
# Mon, 11 Nov 2019 23:49:56 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 11 Nov 2019 23:49:57 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 11 Nov 2019 23:49:58 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Mon, 11 Nov 2019 23:50:00 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 11 Nov 2019 23:50:00 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Mon, 11 Nov 2019 23:50:01 GMT
VOLUME [/var/lib/docker]
# Mon, 11 Nov 2019 23:50:01 GMT
EXPOSE 2375 2376
# Mon, 11 Nov 2019 23:50:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 11 Nov 2019 23:50:03 GMT
CMD []
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4d69e9c49d276dea623c6b05666752b107b3ae7e7fb31faa84c28a89270f7a`  
		Last Modified: Mon, 21 Oct 2019 17:01:55 GMT  
		Size: 302.0 KB (302014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665e2d25121195adad669aa3560768041a5fd3998c859fd6b324c11aac41e3f`  
		Last Modified: Mon, 21 Oct 2019 17:01:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5345f78e94b47be6a4174eaaaa15c5fb58d9d1bee49039f44bd5428cbfd8a10`  
		Last Modified: Mon, 11 Nov 2019 23:51:06 GMT  
		Size: 59.5 MB (59535399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104cd1a725a545c203fc7d69c58ada07ac323e87fad7846f6f7aaffe65899e26`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada593112b1c758ccc55294ec50129d346bc6af329c4f6d9c0855b8d8dad4b40`  
		Last Modified: Mon, 11 Nov 2019 23:50:45 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d393f5a61ff5c52d44b3b7aba3590517be98d59eb54d6039ef1066dc9155642`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0c68e9126ceb889937e4ea4bc5f7073c7134e4feaa4a8ce3bd770b8ee12ae3`  
		Last Modified: Mon, 11 Nov 2019 23:51:19 GMT  
		Size: 3.1 MB (3075592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4646adc61add069716773e72c89f35a80ce16b9392c875cc78c9f18a3691ac`  
		Last Modified: Mon, 11 Nov 2019 23:51:19 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a02871256dc25be5c8def5d731ac9c1bb0296584d14acf545dc8e746828dd`  
		Last Modified: Mon, 11 Nov 2019 23:51:19 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75185c1e06a9732ec086ddcaa667bf3af3e0ff1e870ffee397894572c0eb1a6e`  
		Last Modified: Mon, 11 Nov 2019 23:51:19 GMT  
		Size: 2.5 KB (2538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:d6e44edcbb81b7ef0cd084eea51510a7e8125a41cd71e1d5706b2a5c67c07100
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64963156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:961a08e3b30bee562c2e7754c058fc84faac7a521bbeaf666b3a2192064fda84`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:52:36 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:52:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:14:58 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:03:39 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:03:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:03:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:03:50 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:03:50 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:03:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:03:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:03:53 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:04:03 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 12 Nov 2019 00:04:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:04:06 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 12 Nov 2019 00:04:08 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 12 Nov 2019 00:04:09 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:04:09 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Nov 2019 00:04:10 GMT
EXPOSE 2375 2376
# Tue, 12 Nov 2019 00:04:11 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Nov 2019 00:04:11 GMT
CMD []
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417fcb3850a7455af93e93458e59d7f95bdbb16f1857e99d901142c8d2095eb`  
		Last Modified: Mon, 21 Oct 2019 18:54:57 GMT  
		Size: 300.9 KB (300946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a6ddf38e7cc67bd2f493ebb023839b57b404cc2299f2326c1771c3d559deda`  
		Last Modified: Mon, 21 Oct 2019 18:54:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3849a5e202f85a65a5ad9c6fe517da4209b9c38fa833e3192611a39ef0f94c3`  
		Last Modified: Tue, 12 Nov 2019 00:05:20 GMT  
		Size: 59.5 MB (59532118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea1770de5c377d031e6c7acb30e97987f723c4dad685fe266ac393bf7569a48`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a467e1c8e0b94cc0393bf55890dfc44d81df25c5be86ee01126e96878c0aa655`  
		Last Modified: Tue, 12 Nov 2019 00:04:59 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c668020528b34e7e638923d6cc2b9f90d00fdd2bf18c2973d2375dfa1439e02`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14053bfa3cac76e398dfbe6ccd2ca36eb6765a62c5e61a37bed8243383f5cba7`  
		Last Modified: Tue, 12 Nov 2019 00:05:30 GMT  
		Size: 2.7 MB (2745159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cf65faffbd73e9d6805706b582f930971da640840df9ea0086abf07606f03b`  
		Last Modified: Tue, 12 Nov 2019 00:05:29 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe602a0da610d6505478af90b66a8605fd6fdfc762600e0ac97632182c37def7`  
		Last Modified: Tue, 12 Nov 2019 00:05:29 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d27f6ac9848db30122bcaba288d55026f2a85f8dabc5180d12c6d50de078b25`  
		Last Modified: Tue, 12 Nov 2019 00:05:29 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:ca575c4e6936224e14390fa32d0689cbbabb76da8276593fd3a26219e9038c18
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65554058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:069183d331a4c7faaaf80de3d973255647b6e1df0f16168d6d4eef469d0d1b4d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:13 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:59:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:47:08 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:41:27 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:41:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:41:35 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:41:36 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:41:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:41:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:41:47 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:42:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 12 Nov 2019 00:42:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:42:06 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 12 Nov 2019 00:42:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 12 Nov 2019 00:42:09 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:42:11 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Nov 2019 00:42:11 GMT
EXPOSE 2375 2376
# Tue, 12 Nov 2019 00:42:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Nov 2019 00:42:13 GMT
CMD []
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d523c651118b8110a7055546123bb301485868b779462028d410ad31ce758844`  
		Last Modified: Mon, 21 Oct 2019 19:00:39 GMT  
		Size: 302.3 KB (302343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c404896130ad49e5b0a29fef854c53e121f275ffdd3c624399291cdb710c7`  
		Last Modified: Mon, 21 Oct 2019 19:00:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0ba3badd15b680ea219b55b068bd29a785f18b5d643ddb3bd654bc8d33b46d`  
		Last Modified: Tue, 12 Nov 2019 00:43:18 GMT  
		Size: 57.0 MB (57004922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bad5a8e310ac5b16ebbdbdfa2f613f240e09a5e0c14bc1d543034ea5d420da`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d91f3b8cbf514007493a365e75eb6fc43387856d3158724c425c3958914c11`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa64a18183f137480ac54f7b70a4caa1b3c9d69b76e6210ba3c5160dc06dd9f2`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b067cebdc3e51c1be42460d99d0471c64f4d5d7adb24af16e92c917d13d4c2dc`  
		Last Modified: Tue, 12 Nov 2019 00:43:30 GMT  
		Size: 5.5 MB (5522518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bc0d47be907d032606231e020caff4bd1c2306601748c3a944381deb943974`  
		Last Modified: Tue, 12 Nov 2019 00:43:28 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a98c342e8c81b034629e96469522ce3bf70e6af9a0a79bbdfcd52e0352106ee`  
		Last Modified: Tue, 12 Nov 2019 00:43:28 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f9a38e3d6220a6aea668779fa7c6c4cf8f1b7820b7815f6d0f7191f825556e`  
		Last Modified: Tue, 12 Nov 2019 00:43:28 GMT  
		Size: 2.5 KB (2538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-dind-rootless`

```console
$ docker pull docker@sha256:f066ad6c74a4c14595f66f14589a70da93d5f76c02c15752f6c9ae195b5b0c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:3528a31cd28a813dc89e8180903f82b10170239a14bf14a08b9c03ce43b700a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94645373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7910b59ec98e75afa6b8c9f24f47fb741ac9383f43ee11e7ccdf790a0e2c01d9`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:25:35 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:25:25 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:25:30 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:25:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:31 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:25:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 12 Nov 2019 00:25:37 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:25:37 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 12 Nov 2019 00:25:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 12 Nov 2019 00:25:38 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:38 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Nov 2019 00:25:39 GMT
EXPOSE 2375 2376
# Tue, 12 Nov 2019 00:25:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:39 GMT
CMD []
# Tue, 12 Nov 2019 00:25:44 GMT
RUN apk add --no-cache iproute2
# Tue, 12 Nov 2019 00:25:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 12 Nov 2019 00:25:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:25:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Tue, 12 Nov 2019 00:25:47 GMT
ENV ROOTLESSKIT_VERSION=0.6.0
# Tue, 12 Nov 2019 00:25:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Tue, 12 Nov 2019 00:25:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 12 Nov 2019 00:25:59 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 12 Nov 2019 00:25:59 GMT
USER rootless
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d00f109003f5dd9e123c11faa3270ff5790e2e94cc062ac33acd54317e15e5`  
		Last Modified: Tue, 12 Nov 2019 00:26:53 GMT  
		Size: 63.8 MB (63804789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c3bf8eedaf11dca42c6bdd3160a31267b056f30138e9a83ae6291d7a50d712`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea408e741e559862add2ec71bc27aa6e6a9d6cc900bb7ff5399a3f221c850f4`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d3ea9ec8d1db322186cdbecdc3bffb283e8b87e2f59adfa5ed06c40e9f5f40`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8c4e1a890d6df2310dec90af1a5d6cb0889567e89206389d1873470591a8eb`  
		Last Modified: Tue, 12 Nov 2019 00:27:01 GMT  
		Size: 5.5 MB (5493300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b345be14caeab88468bbf27dc41c5b8751fdfce83312288386288d471f9ec8d0`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e22df429876fd6d189c1fa3bc8f82b66195923ec8881a14f78df16682a59df2`  
		Last Modified: Tue, 12 Nov 2019 00:27:00 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915977ae9ff10b427ff17d4c9152d37ee3575c87d72b5da2b7c68cd0b9556f84`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32795880a521eae7582c0270f900fcac318a148e278f3c5f2056dbecb566c6ae`  
		Last Modified: Tue, 12 Nov 2019 00:27:08 GMT  
		Size: 722.6 KB (722572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c19ee2832c7580babdc0b08bef1837a9639bf2b7efb302d9f800fd400a53c5`  
		Last Modified: Tue, 12 Nov 2019 00:27:06 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5d7916f8600113e56597d04afd6d8d01dfa266fbc832988789b17a50764f97`  
		Last Modified: Tue, 12 Nov 2019 00:27:06 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a06f686027b0f516409ec930965e0510b34ea75f88542df6762cbc226bead62`  
		Last Modified: Tue, 12 Nov 2019 00:27:09 GMT  
		Size: 9.1 MB (9109464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60c15bf7903b46f98edc01a329c0de68aedd24774de6fcb278c1897cd6aa1bb`  
		Last Modified: Tue, 12 Nov 2019 00:27:08 GMT  
		Size: 12.4 MB (12418316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542afa5f61c8214b17bf510810c9d3147ea3de49c53bfb4adc049a62bfc9e7ae`  
		Last Modified: Tue, 12 Nov 2019 00:27:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-git`

```console
$ docker pull docker@sha256:53dcde16046479558fc598170a2a31d4177175b6b7f38cd94dd4881bcbfd7c40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:rc-git` - linux; amd64

```console
$ docker pull docker@sha256:d599afcdd9c35ac777f5cc0ceac1a9bb5f84be9988ff2a86bd30cb1a36cc122b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76799809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55a0e0e0041238f292ea566db38d2571383c905fa20414dc2d12574e8ab327b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:25:35 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:25:25 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:25:30 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:25:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:31 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:26:06 GMT
RUN apk add --no-cache 		git 		openssh-client
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d00f109003f5dd9e123c11faa3270ff5790e2e94cc062ac33acd54317e15e5`  
		Last Modified: Tue, 12 Nov 2019 00:26:53 GMT  
		Size: 63.8 MB (63804789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c3bf8eedaf11dca42c6bdd3160a31267b056f30138e9a83ae6291d7a50d712`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea408e741e559862add2ec71bc27aa6e6a9d6cc900bb7ff5399a3f221c850f4`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d3ea9ec8d1db322186cdbecdc3bffb283e8b87e2f59adfa5ed06c40e9f5f40`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d1acd9de865848d52af16bf1e2c115fe0f53c16e547d44c7173b4741003bd9`  
		Last Modified: Tue, 12 Nov 2019 00:27:17 GMT  
		Size: 9.9 MB (9904329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:8c7f68f26d9236b945df3d7a0c4eda32eab25f583607c51f49548458cca4627b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71797181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a839ea0e09d70a66d2b3ead5a5ff13d627accbe2e4e5845bc7e0dd5c29040e31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 16:57:30 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 16:57:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:52:42 GMT
ENV DOCKER_CHANNEL=test
# Mon, 11 Nov 2019 23:49:32 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Mon, 11 Nov 2019 23:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 11 Nov 2019 23:49:43 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 11 Nov 2019 23:49:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 11 Nov 2019 23:49:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 11 Nov 2019 23:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Nov 2019 23:49:47 GMT
CMD ["sh"]
# Mon, 11 Nov 2019 23:50:12 GMT
RUN apk add --no-cache 		git 		openssh-client
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4d69e9c49d276dea623c6b05666752b107b3ae7e7fb31faa84c28a89270f7a`  
		Last Modified: Mon, 21 Oct 2019 17:01:55 GMT  
		Size: 302.0 KB (302014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2665e2d25121195adad669aa3560768041a5fd3998c859fd6b324c11aac41e3f`  
		Last Modified: Mon, 21 Oct 2019 17:01:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5345f78e94b47be6a4174eaaaa15c5fb58d9d1bee49039f44bd5428cbfd8a10`  
		Last Modified: Mon, 11 Nov 2019 23:51:06 GMT  
		Size: 59.5 MB (59535399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104cd1a725a545c203fc7d69c58ada07ac323e87fad7846f6f7aaffe65899e26`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada593112b1c758ccc55294ec50129d346bc6af329c4f6d9c0855b8d8dad4b40`  
		Last Modified: Mon, 11 Nov 2019 23:50:45 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d393f5a61ff5c52d44b3b7aba3590517be98d59eb54d6039ef1066dc9155642`  
		Last Modified: Mon, 11 Nov 2019 23:50:44 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226cf46f7d3e794e14a6b1e83cf1f9ea93a3e08026b725f05f03cb2a2dec44b4`  
		Last Modified: Mon, 11 Nov 2019 23:51:31 GMT  
		Size: 9.4 MB (9386592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:c7fcc64622440705eab3d9907b58e7aa69eb77578666cbf04c41b132b5be9f7b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70669783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0afd2582713dc5c58c7177cd04f57d8a5f2f394d7a38b4d32e81f1d4a235c0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:52:36 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:52:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:14:58 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:03:39 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:03:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:03:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:03:50 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:03:50 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:03:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:03:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:03:53 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:04:23 GMT
RUN apk add --no-cache 		git 		openssh-client
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a417fcb3850a7455af93e93458e59d7f95bdbb16f1857e99d901142c8d2095eb`  
		Last Modified: Mon, 21 Oct 2019 18:54:57 GMT  
		Size: 300.9 KB (300946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a6ddf38e7cc67bd2f493ebb023839b57b404cc2299f2326c1771c3d559deda`  
		Last Modified: Mon, 21 Oct 2019 18:54:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3849a5e202f85a65a5ad9c6fe517da4209b9c38fa833e3192611a39ef0f94c3`  
		Last Modified: Tue, 12 Nov 2019 00:05:20 GMT  
		Size: 59.5 MB (59532118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea1770de5c377d031e6c7acb30e97987f723c4dad685fe266ac393bf7569a48`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a467e1c8e0b94cc0393bf55890dfc44d81df25c5be86ee01126e96878c0aa655`  
		Last Modified: Tue, 12 Nov 2019 00:04:59 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c668020528b34e7e638923d6cc2b9f90d00fdd2bf18c2973d2375dfa1439e02`  
		Last Modified: Tue, 12 Nov 2019 00:05:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79407638a2835a9aecac1a9df3716130d77061023173d124a092b56cb4500b39`  
		Last Modified: Tue, 12 Nov 2019 00:05:45 GMT  
		Size: 8.5 MB (8456416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:049c58b05337d3882755a6bab40de2fffeb1f2b24f975ac0ab74172588cdb632
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70192134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e589cc3d723bfd13bd500b5e2389e3de9d52d002ce8449b94eb52f14ab525b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:59:13 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:59:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 22:47:08 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:41:27 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:41:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:41:35 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:41:36 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:41:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:41:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:41:47 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:42:22 GMT
RUN apk add --no-cache 		git 		openssh-client
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d523c651118b8110a7055546123bb301485868b779462028d410ad31ce758844`  
		Last Modified: Mon, 21 Oct 2019 19:00:39 GMT  
		Size: 302.3 KB (302343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c404896130ad49e5b0a29fef854c53e121f275ffdd3c624399291cdb710c7`  
		Last Modified: Mon, 21 Oct 2019 19:00:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0ba3badd15b680ea219b55b068bd29a785f18b5d643ddb3bd654bc8d33b46d`  
		Last Modified: Tue, 12 Nov 2019 00:43:18 GMT  
		Size: 57.0 MB (57004922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bad5a8e310ac5b16ebbdbdfa2f613f240e09a5e0c14bc1d543034ea5d420da`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d91f3b8cbf514007493a365e75eb6fc43387856d3158724c425c3958914c11`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa64a18183f137480ac54f7b70a4caa1b3c9d69b76e6210ba3c5160dc06dd9f2`  
		Last Modified: Tue, 12 Nov 2019 00:42:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9bfc23da2e6d49d0d1137456552f257b9eab32db0509a8bbb53458528f58df`  
		Last Modified: Tue, 12 Nov 2019 00:43:43 GMT  
		Size: 10.2 MB (10165227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable`

```console
$ docker pull docker@sha256:0b90b0aefd15794e4d5bea2debc3b761c1d3481a92ec7166f8453652d0deba95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:stable` - linux; amd64

```console
$ docker pull docker@sha256:48db0e29e2214d564b66daffc707ad290c8788dc655cea59c605f021790d38a0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69033024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c774f62a9b520060d72c3c1901facdfdfd0fc4ae7c5e817cdaf6acd456432c`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable` - linux; arm variant v6

```console
$ docker pull docker@sha256:aa908727daa7433a0d156f6c6703fe5d945c4019e8b7f5d0c4fc8213e6d67fed
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64511941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e68c26581b5f619c73bdd54951308df6920447f7be745bea2bfbb6b3624b26`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable` - linux; arm variant v7

```console
$ docker pull docker@sha256:ec6f3f2f65803962bd623ab2de639bd87d41d856c6ef477ae58383b379a1376a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64208081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fc3364d97bc6d5e8c8de60fa7c776bbc4eb6ca32c38029201f27c506086b11`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e09d98b19bbee9f15b9f66604d48401833716faef061e9e509b48fb8db8bd1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62176875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:466581031774ac8ddb27699e61f2fbf858fce357adad7352cc410ef9ad6344bf`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable-dind`

```console
$ docker pull docker@sha256:033ba84f8ea98910d8fc51b8263fbeb24c48d6daf55ef7c654e2981784dac2f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:stable-dind` - linux; amd64

```console
$ docker pull docker@sha256:efd3d1db027f0c8d2cc7019b5381fc9c3cdbbda3642c3ef4feefe5a36cbf0769
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74624904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8489eeb24a264b6bcdb17f3da00140cebe92ee36bd22365f37d07d59390df4ee`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:1e319d9500b33aea20e9c76900595c113e652ebf38ed7021f5daf0e5d78f48af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67731913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6bc19942666d644c636de3a0210745329f07a4c2d3f32c3e9cbd7454e1228c`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 05:53:41 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 05:53:41 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 05:53:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 05:53:44 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:45 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 05:53:46 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 05:53:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:47 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6186deaef3161317f61f202acfab3875747c2a724fad1a65f29f18b068a9ca6c`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 3.2 MB (3215383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6fa6e67b938d446f54f8d3a432d35377ff3431821d39ea805fb2de790ef343`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00bcda5d341dc29b37b45898451e3133f9d420af32d36b21c94d30ac2429ed6`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 749.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daeb323203a88ce4e9152363b7ea9dc8c97580d9723309e442b2c170beb2815`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:7e8985ea07f8786be5b7c551d9547aac01e43a74e8a5831685b39d40fda6d3c6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67091202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef820b49fd591346a99dec34fab401da3022b7cbd60eb8d06f9baef8872d9f3`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:02:23 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 03:02:28 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 03:02:31 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 03:02:36 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 03:02:38 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:02:41 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 03:02:43 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 03:02:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:49 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cb30959a65f691f18075812bbdb8d5f87f944b6d8012dbce90e70e61de7c17`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 2.9 MB (2878527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4bdbf92a47a6e710c3aa65a5fbe9136e986509ab9dacdb67a196fa99441578`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ee73f368ab0a867e3f6b7294736b2ea3263dbf8cc5e6881a1b68ff5856a5c7`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 752.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0bf5e1afaa1f42f73b39a23c9e2203e65c65f6246e63d17ae6def1232a6c5b`  
		Last Modified: Sat, 18 Jan 2020 03:04:00 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31f0251cf185d41e1b6f25bf8acf3d816a73d1d8e583b4c72321a7ccc05801e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67770716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53793fffe26de8f80d9cdfa58c38018e90af8d08eb3f44ebedc03079b7d04d`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 02:24:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 02:24:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 02:24:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 02:24:22 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:24:25 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 02:24:26 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 02:24:30 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 02:24:33 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4704739272105dd3fdfc8614ba689cffe338a0faddc99dace44e191c4567ce`  
		Last Modified: Sat, 18 Jan 2020 02:26:12 GMT  
		Size: 5.6 MB (5589240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8637fb5dd84f5ab45114fc090fda27e2eee33b46a01802c9853a3d0c1b623`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab01413155fcbeedeee71c38d84c48825794515972fd5480a22210379d739d0a`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9514c7ce5d1ffef3aa0a3d41faed1d3ac1e700f99f71157dd4e7d6c418b01de`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable-dind-rootless`

```console
$ docker pull docker@sha256:51f925a59f79f9f85b4869649f6bec7bed065f381186f4102c942ddd4a861cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:stable-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:966cb6bf3b3955ebda64d4e156870e68e3ce20ac9c84a01dee28803aebc334af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97154857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384deac7f3c53083e5d29d8e56a0fa57afa7d88db3c4c34a80c774852f789d26`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
CMD []
# Sat, 18 Jan 2020 04:42:28 GMT
RUN apk add --no-cache iproute2
# Sat, 18 Jan 2020 04:42:29 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Sat, 18 Jan 2020 04:42:30 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Sat, 18 Jan 2020 04:42:32 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Sat, 18 Jan 2020 04:42:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Sat, 18 Jan 2020 04:42:44 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Sat, 18 Jan 2020 04:42:44 GMT
VOLUME [/home/rootless/.local/share/docker]
# Sat, 18 Jan 2020 04:42:44 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cdf1bd44b48b8727fa4bb0545240435dcf820156f0408b1bc13c094f8c01ea`  
		Last Modified: Sat, 18 Jan 2020 04:43:31 GMT  
		Size: 796.0 KB (795977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2313da576c87883442d37ff3743eacdb90d03a6928e9296f65a1083828ffc33`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b530e16b9b04d347cb7c9c99bfa6e4929f67f58f26d1d74d41ab5d80ac8f2`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf525cafee47f341c3c95e742264c04417841f805670bbf8696bdcc8668082d`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 9.1 MB (9109448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2f405bb85fe91994888d7507dd0641b3db43930cf575311ec56af1eead91bd`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 12.6 MB (12622917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373e62ddc7e7489f78a881fa66963be9043dc35ca8e4f345f1d7623af4444fcc`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable-git`

```console
$ docker pull docker@sha256:8b7d15b6cf2118ec104cae6af089d5a9e25f26c687244a2ff93434d10203aa67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:stable-git` - linux; amd64

```console
$ docker pull docker@sha256:64c5cef8dc95f84402635d52a1970f958cec67091c18faf4ccd67eeeb53cbf08
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77246911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eab302e671fdaea238f1049815cb3a36f892ca5499535b6ac80cb6dddb25016`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:50 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f18ea2cbac4c4171b630fa800f91a1cb433728e55ebf865c4e560df098f16d`  
		Last Modified: Sat, 18 Jan 2020 04:43:42 GMT  
		Size: 8.2 MB (8213887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d7464319797cdc81c2a14d9a7c7cbf33afc28d80f08ad9c17ddf543d0d14d6d4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72347135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c3149aca6d91cef011b6ae505719d9294f0cfc56f9c3ec27e89d06e5248ff9`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:56 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25f25e40a87dd2b1e9da8caeaa383822f1194959380646fd4b91816d0fdfb9b`  
		Last Modified: Sat, 18 Jan 2020 05:55:11 GMT  
		Size: 7.8 MB (7835194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:b13771936ea2943baad627ff2354ef3a37b33729054081807f03f756379891de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71280905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10013a543102f31972358bdebe7ab2982abd88ca34247df0d6795f042eca2a0e`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:03:02 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febf3eb0506dfc4914c9b895325fecdb22a9f7545f259026158f6ed3e951bd0b`  
		Last Modified: Sat, 18 Jan 2020 03:04:19 GMT  
		Size: 7.1 MB (7072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d833dbf8e852bcebee568d846c92b5dfdac913bfe5c798b9cddba14b0b0c5cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70582903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa0741e9eec3e5cff51d73a17e11ae2068efc7c31fdb5eb995e7420e100c1af`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:50 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb377abbe251ebb2800e09dd698c95aaabf1a718ab29100760305b15b5a69c`  
		Last Modified: Sat, 18 Jan 2020 02:26:34 GMT  
		Size: 8.4 MB (8406028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test`

```console
$ docker pull docker@sha256:0b90b0aefd15794e4d5bea2debc3b761c1d3481a92ec7166f8453652d0deba95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test` - linux; amd64

```console
$ docker pull docker@sha256:48db0e29e2214d564b66daffc707ad290c8788dc655cea59c605f021790d38a0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69033024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c774f62a9b520060d72c3c1901facdfdfd0fc4ae7c5e817cdaf6acd456432c`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm variant v6

```console
$ docker pull docker@sha256:aa908727daa7433a0d156f6c6703fe5d945c4019e8b7f5d0c4fc8213e6d67fed
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64511941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e68c26581b5f619c73bdd54951308df6920447f7be745bea2bfbb6b3624b26`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm variant v7

```console
$ docker pull docker@sha256:ec6f3f2f65803962bd623ab2de639bd87d41d856c6ef477ae58383b379a1376a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.2 MB (64208081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fc3364d97bc6d5e8c8de60fa7c776bbc4eb6ca32c38029201f27c506086b11`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e09d98b19bbee9f15b9f66604d48401833716faef061e9e509b48fb8db8bd1c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62176875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:466581031774ac8ddb27699e61f2fbf858fce357adad7352cc410ef9ad6344bf`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-dind`

```console
$ docker pull docker@sha256:033ba84f8ea98910d8fc51b8263fbeb24c48d6daf55ef7c654e2981784dac2f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test-dind` - linux; amd64

```console
$ docker pull docker@sha256:efd3d1db027f0c8d2cc7019b5381fc9c3cdbbda3642c3ef4feefe5a36cbf0769
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74624904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8489eeb24a264b6bcdb17f3da00140cebe92ee36bd22365f37d07d59390df4ee`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:1e319d9500b33aea20e9c76900595c113e652ebf38ed7021f5daf0e5d78f48af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67731913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6bc19942666d644c636de3a0210745329f07a4c2d3f32c3e9cbd7454e1228c`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 05:53:41 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 05:53:41 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 05:53:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 05:53:44 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:45 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 05:53:46 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 05:53:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:47 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6186deaef3161317f61f202acfab3875747c2a724fad1a65f29f18b068a9ca6c`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 3.2 MB (3215383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6fa6e67b938d446f54f8d3a432d35377ff3431821d39ea805fb2de790ef343`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00bcda5d341dc29b37b45898451e3133f9d420af32d36b21c94d30ac2429ed6`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 749.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daeb323203a88ce4e9152363b7ea9dc8c97580d9723309e442b2c170beb2815`  
		Last Modified: Sat, 18 Jan 2020 05:54:54 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:7e8985ea07f8786be5b7c551d9547aac01e43a74e8a5831685b39d40fda6d3c6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67091202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef820b49fd591346a99dec34fab401da3022b7cbd60eb8d06f9baef8872d9f3`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:02:23 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 03:02:28 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 03:02:31 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 03:02:36 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 03:02:38 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:02:41 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 03:02:43 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 03:02:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:49 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cb30959a65f691f18075812bbdb8d5f87f944b6d8012dbce90e70e61de7c17`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 2.9 MB (2878527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4bdbf92a47a6e710c3aa65a5fbe9136e986509ab9dacdb67a196fa99441578`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ee73f368ab0a867e3f6b7294736b2ea3263dbf8cc5e6881a1b68ff5856a5c7`  
		Last Modified: Sat, 18 Jan 2020 03:03:59 GMT  
		Size: 752.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0bf5e1afaa1f42f73b39a23c9e2203e65c65f6246e63d17ae6def1232a6c5b`  
		Last Modified: Sat, 18 Jan 2020 03:04:00 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:31f0251cf185d41e1b6f25bf8acf3d816a73d1d8e583b4c72321a7ccc05801e7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67770716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a53793fffe26de8f80d9cdfa58c38018e90af8d08eb3f44ebedc03079b7d04d`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 02:24:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 02:24:13 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 02:24:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 02:24:22 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:24:25 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 02:24:26 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 02:24:30 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 02:24:33 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4704739272105dd3fdfc8614ba689cffe338a0faddc99dace44e191c4567ce`  
		Last Modified: Sat, 18 Jan 2020 02:26:12 GMT  
		Size: 5.6 MB (5589240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee8637fb5dd84f5ab45114fc090fda27e2eee33b46a01802c9853a3d0c1b623`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab01413155fcbeedeee71c38d84c48825794515972fd5480a22210379d739d0a`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9514c7ce5d1ffef3aa0a3d41faed1d3ac1e700f99f71157dd4e7d6c418b01de`  
		Last Modified: Sat, 18 Jan 2020 02:26:10 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-dind-rootless`

```console
$ docker pull docker@sha256:51f925a59f79f9f85b4869649f6bec7bed065f381186f4102c942ddd4a861cd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:test-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:966cb6bf3b3955ebda64d4e156870e68e3ce20ac9c84a01dee28803aebc334af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97154857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384deac7f3c53083e5d29d8e56a0fa57afa7d88db3c4c34a80c774852f789d26`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:21 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Sat, 18 Jan 2020 04:42:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Sat, 18 Jan 2020 04:42:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Sat, 18 Jan 2020 04:42:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:23 GMT
VOLUME [/var/lib/docker]
# Sat, 18 Jan 2020 04:42:23 GMT
EXPOSE 2375 2376
# Sat, 18 Jan 2020 04:42:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:24 GMT
CMD []
# Sat, 18 Jan 2020 04:42:28 GMT
RUN apk add --no-cache iproute2
# Sat, 18 Jan 2020 04:42:29 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Sat, 18 Jan 2020 04:42:30 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Sat, 18 Jan 2020 04:42:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Sat, 18 Jan 2020 04:42:32 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Sat, 18 Jan 2020 04:42:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Sat, 18 Jan 2020 04:42:44 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Sat, 18 Jan 2020 04:42:44 GMT
VOLUME [/home/rootless/.local/share/docker]
# Sat, 18 Jan 2020 04:42:44 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a997a372dbd0d87870fa25eae7215255eb2b01d9e29628131bc069ec6881d51`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 5.6 MB (5587312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab6c938e0f206309b6694d77374fe49f8885b0ecd70255ff85f20b0ba5958c`  
		Last Modified: Sat, 18 Jan 2020 04:43:22 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fcc3f54ae1a83af62f345563b1dfa6b0ae7b0a7b41a29cae54b519c920fc39`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8202733384404f005b36e4dd532c29869dc6d52131d69cb7c3970906f62a81`  
		Last Modified: Sat, 18 Jan 2020 04:43:21 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cdf1bd44b48b8727fa4bb0545240435dcf820156f0408b1bc13c094f8c01ea`  
		Last Modified: Sat, 18 Jan 2020 04:43:31 GMT  
		Size: 796.0 KB (795977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2313da576c87883442d37ff3743eacdb90d03a6928e9296f65a1083828ffc33`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b530e16b9b04d347cb7c9c99bfa6e4929f67f58f26d1d74d41ab5d80ac8f2`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf525cafee47f341c3c95e742264c04417841f805670bbf8696bdcc8668082d`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 9.1 MB (9109448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2f405bb85fe91994888d7507dd0641b3db43930cf575311ec56af1eead91bd`  
		Last Modified: Sat, 18 Jan 2020 04:43:32 GMT  
		Size: 12.6 MB (12622917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373e62ddc7e7489f78a881fa66963be9043dc35ca8e4f345f1d7623af4444fcc`  
		Last Modified: Sat, 18 Jan 2020 04:43:30 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-git`

```console
$ docker pull docker@sha256:8b7d15b6cf2118ec104cae6af089d5a9e25f26c687244a2ff93434d10203aa67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test-git` - linux; amd64

```console
$ docker pull docker@sha256:64c5cef8dc95f84402635d52a1970f958cec67091c18faf4ccd67eeeb53cbf08
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77246911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eab302e671fdaea238f1049815cb3a36f892ca5499535b6ac80cb6dddb25016`
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
# Sat, 18 Jan 2020 04:42:07 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 04:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 04:42:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 04:42:14 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 04:42:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 04:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:42:15 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 04:42:50 GMT
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
	-	`sha256:79e322b40fa78bcb793fcabe57869cfb5e210bb5cfc275064f0cfbe427a36e4e`  
		Last Modified: Sat, 18 Jan 2020 04:43:14 GMT  
		Size: 63.8 MB (63803085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa396aa1c77a2fdb0f6c0ac033a521f8de6ead46ba5d705165277cc5941eda4d`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8b1978c51ebb57ab388b7b3c5a9f6590b49dc4d66b2975074b47a92a56c67c`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc93a7c6112de21c1587c24848731a1ebe1fb72cd8c70179311490b881d6cb`  
		Last Modified: Sat, 18 Jan 2020 04:43:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f18ea2cbac4c4171b630fa800f91a1cb433728e55ebf865c4e560df098f16d`  
		Last Modified: Sat, 18 Jan 2020 04:43:42 GMT  
		Size: 8.2 MB (8213887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d7464319797cdc81c2a14d9a7c7cbf33afc28d80f08ad9c17ddf543d0d14d6d4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72347135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c3149aca6d91cef011b6ae505719d9294f0cfc56f9c3ec27e89d06e5248ff9`
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
# Sat, 18 Jan 2020 05:52:39 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 05:53:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 05:53:01 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 05:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:53:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 05:53:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 05:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 05:53:22 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 05:53:56 GMT
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
	-	`sha256:b2b67a1db9eac111453ec819e686eb891049a6f159178b5e9b3d09c31fd30f26`  
		Last Modified: Sat, 18 Jan 2020 05:54:40 GMT  
		Size: 59.5 MB (59537111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec15d907cba1cc3d6cce4ab1bdd3a7dc51f47536ee2cee27045d33874c14a46`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d3737ec4c19552130a00ec7865542544cfa894f2a8db7d0af66f5d7f689f60`  
		Last Modified: Sat, 18 Jan 2020 05:54:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ce6c271f4e453a31d10d27ae7e3293e9cd064155a53dca693672a455cd4654`  
		Last Modified: Sat, 18 Jan 2020 05:54:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25f25e40a87dd2b1e9da8caeaa383822f1194959380646fd4b91816d0fdfb9b`  
		Last Modified: Sat, 18 Jan 2020 05:55:11 GMT  
		Size: 7.8 MB (7835194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:b13771936ea2943baad627ff2354ef3a37b33729054081807f03f756379891de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71280905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10013a543102f31972358bdebe7ab2982abd88ca34247df0d6795f042eca2a0e`
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
# Sat, 18 Jan 2020 03:01:23 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 03:01:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 03:01:50 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 03:01:51 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:01:54 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 03:02:00 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 03:02:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:02:04 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 03:03:02 GMT
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
	-	`sha256:326615998585f23d6e965ad3a7c5ae78ad6751b00d515729fbe5b6812253c7ef`  
		Last Modified: Sat, 18 Jan 2020 03:03:44 GMT  
		Size: 59.5 MB (59532265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2babc205ada15798696c663e276d3e030c340387254b459937fd034f901ae6`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca461e06d78610e28ccb1e7164387cdd443dbe0c28876aa1ff1af27083240a`  
		Last Modified: Sat, 18 Jan 2020 03:03:24 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3c6de963ff509e6c53b701cfe9c9410e7d346c8433079189a2cb394f6ae247`  
		Last Modified: Sat, 18 Jan 2020 03:03:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febf3eb0506dfc4914c9b895325fecdb22a9f7545f259026158f6ed3e951bd0b`  
		Last Modified: Sat, 18 Jan 2020 03:04:19 GMT  
		Size: 7.1 MB (7072824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d833dbf8e852bcebee568d846c92b5dfdac913bfe5c798b9cddba14b0b0c5cb2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70582903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa0741e9eec3e5cff51d73a17e11ae2068efc7c31fdb5eb995e7420e100c1af`
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
# Sat, 18 Jan 2020 02:23:13 GMT
ENV DOCKER_VERSION=19.03.5
# Sat, 18 Jan 2020 02:23:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Sat, 18 Jan 2020 02:23:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Sat, 18 Jan 2020 02:23:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:23:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Sat, 18 Jan 2020 02:23:41 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Sat, 18 Jan 2020 02:23:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:23:44 GMT
CMD ["sh"]
# Sat, 18 Jan 2020 02:24:50 GMT
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
	-	`sha256:32738a03c1ca50289bdc7d81b64edd2af2a130c1d1d742a8cd81e63c9306aff7`  
		Last Modified: Sat, 18 Jan 2020 02:25:52 GMT  
		Size: 57.0 MB (57006218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36258bdcaf02f467a616cd09eafc78bef2d8343cfd373ade6678cc2669b376e`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149292bf8308cae48ff11692e17ff1e42f4627983b20838d43c9ff7daf0fc23a`  
		Last Modified: Sat, 18 Jan 2020 02:25:31 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91f03656c5246a841a4caf06f518776b95c9fc77409342bc082fa7eaacfe3bb`  
		Last Modified: Sat, 18 Jan 2020 02:25:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb377abbe251ebb2800e09dd698c95aaabf1a718ab29100760305b15b5a69c`  
		Last Modified: Sat, 18 Jan 2020 02:26:34 GMT  
		Size: 8.4 MB (8406028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
