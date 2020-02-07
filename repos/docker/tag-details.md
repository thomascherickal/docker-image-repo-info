<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:19`](#docker19)
-	[`docker:19.03`](#docker1903)
-	[`docker:19.03.5`](#docker19035)
-	[`docker:19.03.5-dind`](#docker19035-dind)
-	[`docker:19.03.5-dind-rootless`](#docker19035-dind-rootless)
-	[`docker:19.03.5-git`](#docker19035-git)
-	[`docker:19.03.6-rc2`](#docker19036-rc2)
-	[`docker:19.03.6-rc2-dind`](#docker19036-rc2-dind)
-	[`docker:19.03.6-rc2-dind-rootless`](#docker19036-rc2-dind-rootless)
-	[`docker:19.03.6-rc2-git`](#docker19036-rc2-git)
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

## `docker:19.03.6-rc2`

```console
$ docker pull docker@sha256:3cd7a8b6d68c88c3d643ce986c4ad7fd147ff3b413d0861a3727bc570b0e5bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03.6-rc2` - linux; amd64

```console
$ docker pull docker@sha256:6090f836b8f32a68e41cfa3018ab035902fc87923b9cde122b1281efa743075d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69404805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee9dc2165a30e8de57233295dbd9791110772704c22e99d5ce272fadd35a1d56`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.6-rc2` - linux; arm variant v6

```console
$ docker pull docker@sha256:b50cd9618f77ebb37c77bfbc7159787900f8449bff5ebd16ef4314439e1905d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64876994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996aeccdec0200978b3055ef8f213be775fcfb814206e90b5f451dbf28002f11`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.6-rc2` - linux; arm variant v7

```console
$ docker pull docker@sha256:eb32cec8343a12b521cc18b3f20bd834c93fd78d5ad364ae5f16375d396a2d9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64565553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d565c546476b27e22955e7eba0558a217cdec7677161d7d758e8e5a484873a9`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.6-rc2` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9fe4c7104a6080e0648677e29c6946c3bccc1d84bda797d69713244042679ff6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62519586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf3af9d08343c17d588e032ec82e2edb3a06d68414c999ea06da3a736510944`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.6-rc2-dind`

```console
$ docker pull docker@sha256:d0bef915133c450a0584f6a35af45f290e4e6125f1cd0b2fad57b692aeddeea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03.6-rc2-dind` - linux; amd64

```console
$ docker pull docker@sha256:e65cc5a657994afb60f8e36fb8d82100795c02891cf69bc8f85ee2a92b7090bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74996702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1858b6f9b12c2fd4043aa050021a447c595b1a2aef032dacd6bdf1eb59ceb646`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:45:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:45:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:21 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:45:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:45:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:24 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:45:24 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:45:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:25 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea91a5b97173d5dd2f344bc5d0e72f82699953ef1c5f959d4a9b7774afa8cf`  
		Last Modified: Fri, 07 Feb 2020 02:47:43 GMT  
		Size: 5.6 MB (5587326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb053638ea5610c62c318ca2e653ca9d0835c05411a1daaa83b82ec3c87b24`  
		Last Modified: Fri, 07 Feb 2020 02:47:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363b8a24b99d588e888eeec2ff5552375c3d2abfa228cd2380f06f6335ee4f8`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3d07de86fbe4cd8f0756a991706ead8e5663775b15af0d03643d133796463`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.6-rc2-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:a1e9f065ea4b31de9aeed07048cf820a64b8637262393b24a4216450da46b7d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68096981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da59f11687039721cafbe22807b6e85c9b11ca0111b044128dc645ce8d41395`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 01:50:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 01:50:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 01:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 01:50:24 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 01:50:25 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:50:26 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 01:50:27 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 01:50:27 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 01:50:28 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb980a31655ba58abb32f83560d0ef7f88661301b94ccaa175d2e313bc6aed7`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 3.2 MB (3215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce42f22e41480fa85926bef938310586295987a9f0722602ffd0b2d0eb4cd9c`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112fde20474ec85e4d421e2dd65099e4243260fa1e46d7b1e01f106ad335d3b6`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 754.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a0e541a9bb4780f1028d69eab8221e95d376c201eaee002c22de1367512015`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.6-rc2-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:2d945bded57825feb19e9c37871c849a56d1761c01274f9f1efecdc0b3be3e50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67448688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cd21cfa9c1ccacf612a7233e0e0627b92209be24b4b900f213c786105b3f05`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:40:18 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:40:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:40:24 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:40:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:40:27 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:27 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:40:28 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:40:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:30 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c49d89b3df9a5ae048f9b8a28125a3d03d349de05c21b3f612bf50b8cbff70`  
		Last Modified: Fri, 07 Feb 2020 02:41:50 GMT  
		Size: 2.9 MB (2878541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736423d9f5ee6704eb47d7eea5a10369e429a6bf29bb1a3753a24928f41b28e`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c6d201bed75e9b686968aac568ea8cce3ebe49784cb654e9498110d113174c`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 750.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e666991900d250a1b261fec470825cf883317a26a234d9336f995cb182db3e8c`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.6-rc2-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d46c1cee6f745e7118e2fa718ec72eb17263514baa2932b3dae4da6bde6314a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68113562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aded5db7219be06281aed695ef98acc490e783953e41beb622530928d7d71b4a`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:53:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:53:17 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:53:18 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:53:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:53:21 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:21 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:53:22 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:53:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:23 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872d7fdc8b0ffd0756d87eaf09b26dd15e9941a8d03cc08feb76d0471581de05`  
		Last Modified: Fri, 07 Feb 2020 02:54:38 GMT  
		Size: 5.6 MB (5589380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08019c6e91ad2246c3d0e1874ce38421287fa844bf497cc7e8484a60893163f`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8749586b7e21a06fc807c68e8a18c0b0b102e500cad4631d3ff91c44ef8963`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 751.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e67ba8b701e74bf676d86cf198127b8739aa2703773cc1d13263ca20e1784`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.6-rc2-dind-rootless`

```console
$ docker pull docker@sha256:4bab8ea9681dfa72ba4a2bb5aaba2e02d928436f3f5977cdb05ff394ac2539eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03.6-rc2-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:0efa3bcf56d0e9070be1a7327c90341e3c58ecedebf4c599c362a73c57e7c3ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97526559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76db5f76af7c366a1f24263eeab75c37609d227b73f75613c0291b93147f483f`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:45:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:45:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:21 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:45:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:45:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:24 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:45:24 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:45:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:25 GMT
CMD []
# Fri, 07 Feb 2020 02:45:32 GMT
RUN apk add --no-cache iproute2
# Fri, 07 Feb 2020 02:45:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 07 Feb 2020 02:45:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 07 Feb 2020 02:45:40 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 07 Feb 2020 02:46:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 07 Feb 2020 02:46:03 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 07 Feb 2020 02:46:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 07 Feb 2020 02:46:04 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea91a5b97173d5dd2f344bc5d0e72f82699953ef1c5f959d4a9b7774afa8cf`  
		Last Modified: Fri, 07 Feb 2020 02:47:43 GMT  
		Size: 5.6 MB (5587326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb053638ea5610c62c318ca2e653ca9d0835c05411a1daaa83b82ec3c87b24`  
		Last Modified: Fri, 07 Feb 2020 02:47:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363b8a24b99d588e888eeec2ff5552375c3d2abfa228cd2380f06f6335ee4f8`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3d07de86fbe4cd8f0756a991706ead8e5663775b15af0d03643d133796463`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342db616cce160fc08012aba5b09c05643f86f1a3619774e1f20d5284440ec73`  
		Last Modified: Fri, 07 Feb 2020 02:47:53 GMT  
		Size: 796.0 KB (795994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db756ea33c8791de85fefa909ce37b309704bd6a34f131ffb919d74f505ead3b`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9703c78438112237598d40096ede1222152aad967dacbac9fd4582373c8d0688`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d246c517d8c2448b88be1b032fb68bc6f86adcba1d8cf574a23c50fdadf6da`  
		Last Modified: Fri, 07 Feb 2020 02:48:00 GMT  
		Size: 9.1 MB (9109464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6270a09865bc1bbaa54e469241142ca426acd6eaea998dc82c435b066f527e7`  
		Last Modified: Fri, 07 Feb 2020 02:47:56 GMT  
		Size: 12.6 MB (12622787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fed64567b6f25fab4045c141d3665c9ea66a16c674a46ccca92ecea1bdaae6`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.6-rc2-git`

```console
$ docker pull docker@sha256:d2b6e6bcdbe71bbd9b283757e5f3c88ca7b416ac2b740eb1d29c411af943a433
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03.6-rc2-git` - linux; amd64

```console
$ docker pull docker@sha256:04b4d052d05be6937dbc121a28b27baaafd689db96cb162d278b2dcbe048cc6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77618705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c8b8d6e6197bebb5c0d1b94ada06238d3438050c4285acd9d3483198fec0ce`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:46:12 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6378fe9e3045e44d5320af2a106d17d5dd21255dea723490c04ae6c95c8361b`  
		Last Modified: Fri, 07 Feb 2020 02:48:18 GMT  
		Size: 8.2 MB (8213900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.6-rc2-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:caea4a7d7fe378ba510788faec30405dbde23cd5abb507bcb8e3966138d0b7a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72712203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0f7f7d70a46d9515d127312836386c98c3502b16759fafb0b11878763e19606`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 01:50:49 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2308e8328aef9a6de84f7410e943d859481a88aa7636d5297a2d35b9961566a8`  
		Last Modified: Fri, 07 Feb 2020 01:52:25 GMT  
		Size: 7.8 MB (7835209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.6-rc2-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:c310a56efb22f8697c34b441cf87b45e30e64369a5fca5967dc3938e57be5818
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71638357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12fb892d7c3e2cafe92f04437154f38313f159a6d959942d02a7dfd255090ce`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:40:38 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67e887d6c365daa130725d5bdcf3e4f4b4d8c2d3479c8677ebc0919dacd6432`  
		Last Modified: Fri, 07 Feb 2020 02:42:08 GMT  
		Size: 7.1 MB (7072804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.6-rc2-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c191bb5761937c957671c94862396a2b69c623eec2379306b3f91117fbdabde
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70925612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca5997b843d1cf224c6933ed3c2c12eb145f9a0657cf2de33cd2ac5c6a0c6ea`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:53:31 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5179ea1a503390358687888ca828868daf9b9459fec0da0a959e33bfc89fed`  
		Last Modified: Fri, 07 Feb 2020 02:54:55 GMT  
		Size: 8.4 MB (8406026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull docker@sha256:3cd7a8b6d68c88c3d643ce986c4ad7fd147ff3b413d0861a3727bc570b0e5bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-rc` - linux; amd64

```console
$ docker pull docker@sha256:6090f836b8f32a68e41cfa3018ab035902fc87923b9cde122b1281efa743075d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69404805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee9dc2165a30e8de57233295dbd9791110772704c22e99d5ce272fadd35a1d56`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc` - linux; arm variant v6

```console
$ docker pull docker@sha256:b50cd9618f77ebb37c77bfbc7159787900f8449bff5ebd16ef4314439e1905d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64876994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996aeccdec0200978b3055ef8f213be775fcfb814206e90b5f451dbf28002f11`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc` - linux; arm variant v7

```console
$ docker pull docker@sha256:eb32cec8343a12b521cc18b3f20bd834c93fd78d5ad364ae5f16375d396a2d9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64565553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d565c546476b27e22955e7eba0558a217cdec7677161d7d758e8e5a484873a9`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9fe4c7104a6080e0648677e29c6946c3bccc1d84bda797d69713244042679ff6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62519586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf3af9d08343c17d588e032ec82e2edb3a06d68414c999ea06da3a736510944`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-rc-dind`

```console
$ docker pull docker@sha256:d0bef915133c450a0584f6a35af45f290e4e6125f1cd0b2fad57b692aeddeea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:e65cc5a657994afb60f8e36fb8d82100795c02891cf69bc8f85ee2a92b7090bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74996702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1858b6f9b12c2fd4043aa050021a447c595b1a2aef032dacd6bdf1eb59ceb646`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:45:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:45:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:21 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:45:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:45:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:24 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:45:24 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:45:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:25 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea91a5b97173d5dd2f344bc5d0e72f82699953ef1c5f959d4a9b7774afa8cf`  
		Last Modified: Fri, 07 Feb 2020 02:47:43 GMT  
		Size: 5.6 MB (5587326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb053638ea5610c62c318ca2e653ca9d0835c05411a1daaa83b82ec3c87b24`  
		Last Modified: Fri, 07 Feb 2020 02:47:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363b8a24b99d588e888eeec2ff5552375c3d2abfa228cd2380f06f6335ee4f8`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3d07de86fbe4cd8f0756a991706ead8e5663775b15af0d03643d133796463`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:a1e9f065ea4b31de9aeed07048cf820a64b8637262393b24a4216450da46b7d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68096981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da59f11687039721cafbe22807b6e85c9b11ca0111b044128dc645ce8d41395`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 01:50:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 01:50:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 01:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 01:50:24 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 01:50:25 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:50:26 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 01:50:27 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 01:50:27 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 01:50:28 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb980a31655ba58abb32f83560d0ef7f88661301b94ccaa175d2e313bc6aed7`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 3.2 MB (3215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce42f22e41480fa85926bef938310586295987a9f0722602ffd0b2d0eb4cd9c`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112fde20474ec85e4d421e2dd65099e4243260fa1e46d7b1e01f106ad335d3b6`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 754.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a0e541a9bb4780f1028d69eab8221e95d376c201eaee002c22de1367512015`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:2d945bded57825feb19e9c37871c849a56d1761c01274f9f1efecdc0b3be3e50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67448688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cd21cfa9c1ccacf612a7233e0e0627b92209be24b4b900f213c786105b3f05`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:40:18 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:40:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:40:24 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:40:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:40:27 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:27 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:40:28 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:40:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:30 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c49d89b3df9a5ae048f9b8a28125a3d03d349de05c21b3f612bf50b8cbff70`  
		Last Modified: Fri, 07 Feb 2020 02:41:50 GMT  
		Size: 2.9 MB (2878541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736423d9f5ee6704eb47d7eea5a10369e429a6bf29bb1a3753a24928f41b28e`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c6d201bed75e9b686968aac568ea8cce3ebe49784cb654e9498110d113174c`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 750.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e666991900d250a1b261fec470825cf883317a26a234d9336f995cb182db3e8c`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d46c1cee6f745e7118e2fa718ec72eb17263514baa2932b3dae4da6bde6314a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68113562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aded5db7219be06281aed695ef98acc490e783953e41beb622530928d7d71b4a`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:53:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:53:17 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:53:18 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:53:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:53:21 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:21 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:53:22 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:53:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:23 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872d7fdc8b0ffd0756d87eaf09b26dd15e9941a8d03cc08feb76d0471581de05`  
		Last Modified: Fri, 07 Feb 2020 02:54:38 GMT  
		Size: 5.6 MB (5589380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08019c6e91ad2246c3d0e1874ce38421287fa844bf497cc7e8484a60893163f`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8749586b7e21a06fc807c68e8a18c0b0b102e500cad4631d3ff91c44ef8963`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 751.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e67ba8b701e74bf676d86cf198127b8739aa2703773cc1d13263ca20e1784`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-rc-dind-rootless`

```console
$ docker pull docker@sha256:4bab8ea9681dfa72ba4a2bb5aaba2e02d928436f3f5977cdb05ff394ac2539eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03-rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:0efa3bcf56d0e9070be1a7327c90341e3c58ecedebf4c599c362a73c57e7c3ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97526559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76db5f76af7c366a1f24263eeab75c37609d227b73f75613c0291b93147f483f`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:45:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:45:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:21 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:45:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:45:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:24 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:45:24 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:45:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:25 GMT
CMD []
# Fri, 07 Feb 2020 02:45:32 GMT
RUN apk add --no-cache iproute2
# Fri, 07 Feb 2020 02:45:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 07 Feb 2020 02:45:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 07 Feb 2020 02:45:40 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 07 Feb 2020 02:46:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 07 Feb 2020 02:46:03 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 07 Feb 2020 02:46:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 07 Feb 2020 02:46:04 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea91a5b97173d5dd2f344bc5d0e72f82699953ef1c5f959d4a9b7774afa8cf`  
		Last Modified: Fri, 07 Feb 2020 02:47:43 GMT  
		Size: 5.6 MB (5587326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb053638ea5610c62c318ca2e653ca9d0835c05411a1daaa83b82ec3c87b24`  
		Last Modified: Fri, 07 Feb 2020 02:47:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363b8a24b99d588e888eeec2ff5552375c3d2abfa228cd2380f06f6335ee4f8`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3d07de86fbe4cd8f0756a991706ead8e5663775b15af0d03643d133796463`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342db616cce160fc08012aba5b09c05643f86f1a3619774e1f20d5284440ec73`  
		Last Modified: Fri, 07 Feb 2020 02:47:53 GMT  
		Size: 796.0 KB (795994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db756ea33c8791de85fefa909ce37b309704bd6a34f131ffb919d74f505ead3b`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9703c78438112237598d40096ede1222152aad967dacbac9fd4582373c8d0688`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d246c517d8c2448b88be1b032fb68bc6f86adcba1d8cf574a23c50fdadf6da`  
		Last Modified: Fri, 07 Feb 2020 02:48:00 GMT  
		Size: 9.1 MB (9109464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6270a09865bc1bbaa54e469241142ca426acd6eaea998dc82c435b066f527e7`  
		Last Modified: Fri, 07 Feb 2020 02:47:56 GMT  
		Size: 12.6 MB (12622787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fed64567b6f25fab4045c141d3665c9ea66a16c674a46ccca92ecea1bdaae6`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-rc-git`

```console
$ docker pull docker@sha256:d2b6e6bcdbe71bbd9b283757e5f3c88ca7b416ac2b740eb1d29c411af943a433
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-rc-git` - linux; amd64

```console
$ docker pull docker@sha256:04b4d052d05be6937dbc121a28b27baaafd689db96cb162d278b2dcbe048cc6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77618705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c8b8d6e6197bebb5c0d1b94ada06238d3438050c4285acd9d3483198fec0ce`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:46:12 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6378fe9e3045e44d5320af2a106d17d5dd21255dea723490c04ae6c95c8361b`  
		Last Modified: Fri, 07 Feb 2020 02:48:18 GMT  
		Size: 8.2 MB (8213900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:caea4a7d7fe378ba510788faec30405dbde23cd5abb507bcb8e3966138d0b7a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72712203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0f7f7d70a46d9515d127312836386c98c3502b16759fafb0b11878763e19606`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 01:50:49 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2308e8328aef9a6de84f7410e943d859481a88aa7636d5297a2d35b9961566a8`  
		Last Modified: Fri, 07 Feb 2020 01:52:25 GMT  
		Size: 7.8 MB (7835209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:c310a56efb22f8697c34b441cf87b45e30e64369a5fca5967dc3938e57be5818
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71638357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12fb892d7c3e2cafe92f04437154f38313f159a6d959942d02a7dfd255090ce`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:40:38 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67e887d6c365daa130725d5bdcf3e4f4b4d8c2d3479c8677ebc0919dacd6432`  
		Last Modified: Fri, 07 Feb 2020 02:42:08 GMT  
		Size: 7.1 MB (7072804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c191bb5761937c957671c94862396a2b69c623eec2379306b3f91117fbdabde
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70925612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca5997b843d1cf224c6933ed3c2c12eb145f9a0657cf2de33cd2ac5c6a0c6ea`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:53:31 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5179ea1a503390358687888ca828868daf9b9459fec0da0a959e33bfc89fed`  
		Last Modified: Fri, 07 Feb 2020 02:54:55 GMT  
		Size: 8.4 MB (8406026 bytes)  
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
$ docker pull docker@sha256:3cd7a8b6d68c88c3d643ce986c4ad7fd147ff3b413d0861a3727bc570b0e5bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:rc` - linux; amd64

```console
$ docker pull docker@sha256:6090f836b8f32a68e41cfa3018ab035902fc87923b9cde122b1281efa743075d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69404805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee9dc2165a30e8de57233295dbd9791110772704c22e99d5ce272fadd35a1d56`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm variant v6

```console
$ docker pull docker@sha256:b50cd9618f77ebb37c77bfbc7159787900f8449bff5ebd16ef4314439e1905d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64876994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996aeccdec0200978b3055ef8f213be775fcfb814206e90b5f451dbf28002f11`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm variant v7

```console
$ docker pull docker@sha256:eb32cec8343a12b521cc18b3f20bd834c93fd78d5ad364ae5f16375d396a2d9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64565553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d565c546476b27e22955e7eba0558a217cdec7677161d7d758e8e5a484873a9`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9fe4c7104a6080e0648677e29c6946c3bccc1d84bda797d69713244042679ff6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62519586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf3af9d08343c17d588e032ec82e2edb3a06d68414c999ea06da3a736510944`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-dind`

```console
$ docker pull docker@sha256:d0bef915133c450a0584f6a35af45f290e4e6125f1cd0b2fad57b692aeddeea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:e65cc5a657994afb60f8e36fb8d82100795c02891cf69bc8f85ee2a92b7090bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74996702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1858b6f9b12c2fd4043aa050021a447c595b1a2aef032dacd6bdf1eb59ceb646`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:45:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:45:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:21 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:45:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:45:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:24 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:45:24 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:45:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:25 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea91a5b97173d5dd2f344bc5d0e72f82699953ef1c5f959d4a9b7774afa8cf`  
		Last Modified: Fri, 07 Feb 2020 02:47:43 GMT  
		Size: 5.6 MB (5587326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb053638ea5610c62c318ca2e653ca9d0835c05411a1daaa83b82ec3c87b24`  
		Last Modified: Fri, 07 Feb 2020 02:47:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363b8a24b99d588e888eeec2ff5552375c3d2abfa228cd2380f06f6335ee4f8`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3d07de86fbe4cd8f0756a991706ead8e5663775b15af0d03643d133796463`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:a1e9f065ea4b31de9aeed07048cf820a64b8637262393b24a4216450da46b7d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68096981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da59f11687039721cafbe22807b6e85c9b11ca0111b044128dc645ce8d41395`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 01:50:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 01:50:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 01:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 01:50:24 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 01:50:25 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:50:26 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 01:50:27 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 01:50:27 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 01:50:28 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb980a31655ba58abb32f83560d0ef7f88661301b94ccaa175d2e313bc6aed7`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 3.2 MB (3215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce42f22e41480fa85926bef938310586295987a9f0722602ffd0b2d0eb4cd9c`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112fde20474ec85e4d421e2dd65099e4243260fa1e46d7b1e01f106ad335d3b6`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 754.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a0e541a9bb4780f1028d69eab8221e95d376c201eaee002c22de1367512015`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:2d945bded57825feb19e9c37871c849a56d1761c01274f9f1efecdc0b3be3e50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67448688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cd21cfa9c1ccacf612a7233e0e0627b92209be24b4b900f213c786105b3f05`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:40:18 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:40:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:40:24 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:40:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:40:27 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:27 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:40:28 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:40:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:30 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c49d89b3df9a5ae048f9b8a28125a3d03d349de05c21b3f612bf50b8cbff70`  
		Last Modified: Fri, 07 Feb 2020 02:41:50 GMT  
		Size: 2.9 MB (2878541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736423d9f5ee6704eb47d7eea5a10369e429a6bf29bb1a3753a24928f41b28e`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c6d201bed75e9b686968aac568ea8cce3ebe49784cb654e9498110d113174c`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 750.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e666991900d250a1b261fec470825cf883317a26a234d9336f995cb182db3e8c`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d46c1cee6f745e7118e2fa718ec72eb17263514baa2932b3dae4da6bde6314a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68113562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aded5db7219be06281aed695ef98acc490e783953e41beb622530928d7d71b4a`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:53:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:53:17 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:53:18 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:53:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:53:21 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:21 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:53:22 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:53:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:23 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872d7fdc8b0ffd0756d87eaf09b26dd15e9941a8d03cc08feb76d0471581de05`  
		Last Modified: Fri, 07 Feb 2020 02:54:38 GMT  
		Size: 5.6 MB (5589380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08019c6e91ad2246c3d0e1874ce38421287fa844bf497cc7e8484a60893163f`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8749586b7e21a06fc807c68e8a18c0b0b102e500cad4631d3ff91c44ef8963`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 751.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e67ba8b701e74bf676d86cf198127b8739aa2703773cc1d13263ca20e1784`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-dind-rootless`

```console
$ docker pull docker@sha256:4bab8ea9681dfa72ba4a2bb5aaba2e02d928436f3f5977cdb05ff394ac2539eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:0efa3bcf56d0e9070be1a7327c90341e3c58ecedebf4c599c362a73c57e7c3ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97526559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76db5f76af7c366a1f24263eeab75c37609d227b73f75613c0291b93147f483f`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:45:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:45:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:21 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:45:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:45:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:24 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:45:24 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:45:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:25 GMT
CMD []
# Fri, 07 Feb 2020 02:45:32 GMT
RUN apk add --no-cache iproute2
# Fri, 07 Feb 2020 02:45:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 07 Feb 2020 02:45:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 07 Feb 2020 02:45:40 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 07 Feb 2020 02:46:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 07 Feb 2020 02:46:03 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 07 Feb 2020 02:46:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 07 Feb 2020 02:46:04 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea91a5b97173d5dd2f344bc5d0e72f82699953ef1c5f959d4a9b7774afa8cf`  
		Last Modified: Fri, 07 Feb 2020 02:47:43 GMT  
		Size: 5.6 MB (5587326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb053638ea5610c62c318ca2e653ca9d0835c05411a1daaa83b82ec3c87b24`  
		Last Modified: Fri, 07 Feb 2020 02:47:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363b8a24b99d588e888eeec2ff5552375c3d2abfa228cd2380f06f6335ee4f8`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3d07de86fbe4cd8f0756a991706ead8e5663775b15af0d03643d133796463`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342db616cce160fc08012aba5b09c05643f86f1a3619774e1f20d5284440ec73`  
		Last Modified: Fri, 07 Feb 2020 02:47:53 GMT  
		Size: 796.0 KB (795994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db756ea33c8791de85fefa909ce37b309704bd6a34f131ffb919d74f505ead3b`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9703c78438112237598d40096ede1222152aad967dacbac9fd4582373c8d0688`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d246c517d8c2448b88be1b032fb68bc6f86adcba1d8cf574a23c50fdadf6da`  
		Last Modified: Fri, 07 Feb 2020 02:48:00 GMT  
		Size: 9.1 MB (9109464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6270a09865bc1bbaa54e469241142ca426acd6eaea998dc82c435b066f527e7`  
		Last Modified: Fri, 07 Feb 2020 02:47:56 GMT  
		Size: 12.6 MB (12622787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fed64567b6f25fab4045c141d3665c9ea66a16c674a46ccca92ecea1bdaae6`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:rc-git`

```console
$ docker pull docker@sha256:d2b6e6bcdbe71bbd9b283757e5f3c88ca7b416ac2b740eb1d29c411af943a433
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:rc-git` - linux; amd64

```console
$ docker pull docker@sha256:04b4d052d05be6937dbc121a28b27baaafd689db96cb162d278b2dcbe048cc6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77618705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c8b8d6e6197bebb5c0d1b94ada06238d3438050c4285acd9d3483198fec0ce`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:46:12 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6378fe9e3045e44d5320af2a106d17d5dd21255dea723490c04ae6c95c8361b`  
		Last Modified: Fri, 07 Feb 2020 02:48:18 GMT  
		Size: 8.2 MB (8213900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:caea4a7d7fe378ba510788faec30405dbde23cd5abb507bcb8e3966138d0b7a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72712203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0f7f7d70a46d9515d127312836386c98c3502b16759fafb0b11878763e19606`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 01:50:49 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2308e8328aef9a6de84f7410e943d859481a88aa7636d5297a2d35b9961566a8`  
		Last Modified: Fri, 07 Feb 2020 01:52:25 GMT  
		Size: 7.8 MB (7835209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:c310a56efb22f8697c34b441cf87b45e30e64369a5fca5967dc3938e57be5818
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71638357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12fb892d7c3e2cafe92f04437154f38313f159a6d959942d02a7dfd255090ce`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:40:38 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67e887d6c365daa130725d5bdcf3e4f4b4d8c2d3479c8677ebc0919dacd6432`  
		Last Modified: Fri, 07 Feb 2020 02:42:08 GMT  
		Size: 7.1 MB (7072804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c191bb5761937c957671c94862396a2b69c623eec2379306b3f91117fbdabde
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70925612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca5997b843d1cf224c6933ed3c2c12eb145f9a0657cf2de33cd2ac5c6a0c6ea`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:53:31 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5179ea1a503390358687888ca828868daf9b9459fec0da0a959e33bfc89fed`  
		Last Modified: Fri, 07 Feb 2020 02:54:55 GMT  
		Size: 8.4 MB (8406026 bytes)  
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
$ docker pull docker@sha256:3cd7a8b6d68c88c3d643ce986c4ad7fd147ff3b413d0861a3727bc570b0e5bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test` - linux; amd64

```console
$ docker pull docker@sha256:6090f836b8f32a68e41cfa3018ab035902fc87923b9cde122b1281efa743075d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69404805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee9dc2165a30e8de57233295dbd9791110772704c22e99d5ce272fadd35a1d56`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm variant v6

```console
$ docker pull docker@sha256:b50cd9618f77ebb37c77bfbc7159787900f8449bff5ebd16ef4314439e1905d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64876994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996aeccdec0200978b3055ef8f213be775fcfb814206e90b5f451dbf28002f11`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm variant v7

```console
$ docker pull docker@sha256:eb32cec8343a12b521cc18b3f20bd834c93fd78d5ad364ae5f16375d396a2d9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.6 MB (64565553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d565c546476b27e22955e7eba0558a217cdec7677161d7d758e8e5a484873a9`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9fe4c7104a6080e0648677e29c6946c3bccc1d84bda797d69713244042679ff6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62519586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf3af9d08343c17d588e032ec82e2edb3a06d68414c999ea06da3a736510944`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-dind`

```console
$ docker pull docker@sha256:d0bef915133c450a0584f6a35af45f290e4e6125f1cd0b2fad57b692aeddeea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test-dind` - linux; amd64

```console
$ docker pull docker@sha256:e65cc5a657994afb60f8e36fb8d82100795c02891cf69bc8f85ee2a92b7090bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (74996702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1858b6f9b12c2fd4043aa050021a447c595b1a2aef032dacd6bdf1eb59ceb646`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:45:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:45:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:21 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:45:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:45:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:24 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:45:24 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:45:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:25 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea91a5b97173d5dd2f344bc5d0e72f82699953ef1c5f959d4a9b7774afa8cf`  
		Last Modified: Fri, 07 Feb 2020 02:47:43 GMT  
		Size: 5.6 MB (5587326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb053638ea5610c62c318ca2e653ca9d0835c05411a1daaa83b82ec3c87b24`  
		Last Modified: Fri, 07 Feb 2020 02:47:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363b8a24b99d588e888eeec2ff5552375c3d2abfa228cd2380f06f6335ee4f8`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3d07de86fbe4cd8f0756a991706ead8e5663775b15af0d03643d133796463`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:a1e9f065ea4b31de9aeed07048cf820a64b8637262393b24a4216450da46b7d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68096981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da59f11687039721cafbe22807b6e85c9b11ca0111b044128dc645ce8d41395`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 01:50:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 01:50:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 01:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 01:50:24 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 01:50:25 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:50:26 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 01:50:27 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 01:50:27 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 01:50:28 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb980a31655ba58abb32f83560d0ef7f88661301b94ccaa175d2e313bc6aed7`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 3.2 MB (3215389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce42f22e41480fa85926bef938310586295987a9f0722602ffd0b2d0eb4cd9c`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112fde20474ec85e4d421e2dd65099e4243260fa1e46d7b1e01f106ad335d3b6`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 754.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a0e541a9bb4780f1028d69eab8221e95d376c201eaee002c22de1367512015`  
		Last Modified: Fri, 07 Feb 2020 01:52:09 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:2d945bded57825feb19e9c37871c849a56d1761c01274f9f1efecdc0b3be3e50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67448688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cd21cfa9c1ccacf612a7233e0e0627b92209be24b4b900f213c786105b3f05`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:40:18 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:40:22 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:40:24 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:40:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:40:27 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:27 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:40:28 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:40:29 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:30 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c49d89b3df9a5ae048f9b8a28125a3d03d349de05c21b3f612bf50b8cbff70`  
		Last Modified: Fri, 07 Feb 2020 02:41:50 GMT  
		Size: 2.9 MB (2878541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736423d9f5ee6704eb47d7eea5a10369e429a6bf29bb1a3753a24928f41b28e`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c6d201bed75e9b686968aac568ea8cce3ebe49784cb654e9498110d113174c`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 750.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e666991900d250a1b261fec470825cf883317a26a234d9336f995cb182db3e8c`  
		Last Modified: Fri, 07 Feb 2020 02:41:49 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d46c1cee6f745e7118e2fa718ec72eb17263514baa2932b3dae4da6bde6314a4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68113562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aded5db7219be06281aed695ef98acc490e783953e41beb622530928d7d71b4a`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:53:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:53:17 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:53:18 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:53:20 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:53:21 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:21 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:53:22 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:53:22 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:23 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872d7fdc8b0ffd0756d87eaf09b26dd15e9941a8d03cc08feb76d0471581de05`  
		Last Modified: Fri, 07 Feb 2020 02:54:38 GMT  
		Size: 5.6 MB (5589380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08019c6e91ad2246c3d0e1874ce38421287fa844bf497cc7e8484a60893163f`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8749586b7e21a06fc807c68e8a18c0b0b102e500cad4631d3ff91c44ef8963`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 751.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e67ba8b701e74bf676d86cf198127b8739aa2703773cc1d13263ca20e1784`  
		Last Modified: Fri, 07 Feb 2020 02:54:35 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-dind-rootless`

```console
$ docker pull docker@sha256:4bab8ea9681dfa72ba4a2bb5aaba2e02d928436f3f5977cdb05ff394ac2539eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:test-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:0efa3bcf56d0e9070be1a7327c90341e3c58ecedebf4c599c362a73c57e7c3ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97526559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76db5f76af7c366a1f24263eeab75c37609d227b73f75613c0291b93147f483f`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:45:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 07 Feb 2020 02:45:21 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:21 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Fri, 07 Feb 2020 02:45:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 07 Feb 2020 02:45:23 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:24 GMT
VOLUME [/var/lib/docker]
# Fri, 07 Feb 2020 02:45:24 GMT
EXPOSE 2375 2376
# Fri, 07 Feb 2020 02:45:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:25 GMT
CMD []
# Fri, 07 Feb 2020 02:45:32 GMT
RUN apk add --no-cache iproute2
# Fri, 07 Feb 2020 02:45:34 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 07 Feb 2020 02:45:35 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 07 Feb 2020 02:45:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 07 Feb 2020 02:45:40 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 07 Feb 2020 02:46:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 07 Feb 2020 02:46:03 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 07 Feb 2020 02:46:04 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 07 Feb 2020 02:46:04 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eea91a5b97173d5dd2f344bc5d0e72f82699953ef1c5f959d4a9b7774afa8cf`  
		Last Modified: Fri, 07 Feb 2020 02:47:43 GMT  
		Size: 5.6 MB (5587326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbb053638ea5610c62c318ca2e653ca9d0835c05411a1daaa83b82ec3c87b24`  
		Last Modified: Fri, 07 Feb 2020 02:47:42 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363b8a24b99d588e888eeec2ff5552375c3d2abfa228cd2380f06f6335ee4f8`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3d07de86fbe4cd8f0756a991706ead8e5663775b15af0d03643d133796463`  
		Last Modified: Fri, 07 Feb 2020 02:47:41 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342db616cce160fc08012aba5b09c05643f86f1a3619774e1f20d5284440ec73`  
		Last Modified: Fri, 07 Feb 2020 02:47:53 GMT  
		Size: 796.0 KB (795994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db756ea33c8791de85fefa909ce37b309704bd6a34f131ffb919d74f505ead3b`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9703c78438112237598d40096ede1222152aad967dacbac9fd4582373c8d0688`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d246c517d8c2448b88be1b032fb68bc6f86adcba1d8cf574a23c50fdadf6da`  
		Last Modified: Fri, 07 Feb 2020 02:48:00 GMT  
		Size: 9.1 MB (9109464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6270a09865bc1bbaa54e469241142ca426acd6eaea998dc82c435b066f527e7`  
		Last Modified: Fri, 07 Feb 2020 02:47:56 GMT  
		Size: 12.6 MB (12622787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fed64567b6f25fab4045c141d3665c9ea66a16c674a46ccca92ecea1bdaae6`  
		Last Modified: Fri, 07 Feb 2020 02:47:51 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-git`

```console
$ docker pull docker@sha256:d2b6e6bcdbe71bbd9b283757e5f3c88ca7b416ac2b740eb1d29c411af943a433
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test-git` - linux; amd64

```console
$ docker pull docker@sha256:04b4d052d05be6937dbc121a28b27baaafd689db96cb162d278b2dcbe048cc6c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77618705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c8b8d6e6197bebb5c0d1b94ada06238d3438050c4285acd9d3483198fec0ce`
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
# Wed, 29 Jan 2020 19:20:00 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:44:57 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:45:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:45:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:45:08 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:45:08 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:45:10 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:45:10 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:46:12 GMT
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
	-	`sha256:caea7060abe9610714377bd4bba10bdc84753e6e62fa0e1ffdc5c4e12848b51e`  
		Last Modified: Fri, 07 Feb 2020 02:47:33 GMT  
		Size: 64.2 MB (64174865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b866925237283b42ccdf5500fced4225fc4ffa5aff8e5e797d8cee70997177`  
		Last Modified: Fri, 07 Feb 2020 02:47:12 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae0723913e410c295d4f5fedfe376630dd0a177f56989ef6b61b2e316e5884`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae024136251285a97bd4a3b789755dcbcc96f128f498429bfab5c8f4db8355e`  
		Last Modified: Fri, 07 Feb 2020 02:47:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6378fe9e3045e44d5320af2a106d17d5dd21255dea723490c04ae6c95c8361b`  
		Last Modified: Fri, 07 Feb 2020 02:48:18 GMT  
		Size: 8.2 MB (8213900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:caea4a7d7fe378ba510788faec30405dbde23cd5abb507bcb8e3966138d0b7a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72712203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0f7f7d70a46d9515d127312836386c98c3502b16759fafb0b11878763e19606`
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
# Wed, 29 Jan 2020 19:49:55 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 01:49:30 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 01:49:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 01:49:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 01:49:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 01:49:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 01:49:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 01:49:57 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 01:50:49 GMT
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
	-	`sha256:33c50d9f5ebbcdc846f18771ee330450b7fff603f6f3f0a162f827feefea9b2d`  
		Last Modified: Fri, 07 Feb 2020 01:51:56 GMT  
		Size: 59.9 MB (59902162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58ca6425cb3f176b096d64b01e6281be81bd13df81b50ffa27a95239e4511d5`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e48b798c3734357d6c87dfca18e0ae77f15e69e877cbc3c2370ac2ef004efe`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0fffc54c09bd0c9388338ccbf469ccc15bce13951638c2b07e9a64f7d7d761`  
		Last Modified: Fri, 07 Feb 2020 01:51:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2308e8328aef9a6de84f7410e943d859481a88aa7636d5297a2d35b9961566a8`  
		Last Modified: Fri, 07 Feb 2020 01:52:25 GMT  
		Size: 7.8 MB (7835209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:c310a56efb22f8697c34b441cf87b45e30e64369a5fca5967dc3938e57be5818
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.6 MB (71638357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12fb892d7c3e2cafe92f04437154f38313f159a6d959942d02a7dfd255090ce`
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
# Wed, 29 Jan 2020 19:57:32 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:39:45 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:40:03 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:40:05 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:40:38 GMT
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
	-	`sha256:d9015c180d6e38c780d7ffae8ed1360cba3fc384f560587a6092c42317740318`  
		Last Modified: Fri, 07 Feb 2020 02:41:38 GMT  
		Size: 59.9 MB (59889736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa23b1a26f3312c0b9b21381b8b9ed57002efaf12478275d8dfa252dcb55926`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9659cd7acc802bc16b7c635d6c4f4829612219506fb5a8c358c7e3ffe55ae0b1`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6e1d50e985217559261a740df789190ce04f211a9669c1e08ea0cf4d40ce4`  
		Last Modified: Fri, 07 Feb 2020 02:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67e887d6c365daa130725d5bdcf3e4f4b4d8c2d3479c8677ebc0919dacd6432`  
		Last Modified: Fri, 07 Feb 2020 02:42:08 GMT  
		Size: 7.1 MB (7072804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c191bb5761937c957671c94862396a2b69c623eec2379306b3f91117fbdabde
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70925612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca5997b843d1cf224c6933ed3c2c12eb145f9a0657cf2de33cd2ac5c6a0c6ea`
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
# Wed, 29 Jan 2020 19:39:53 GMT
ENV DOCKER_CHANNEL=test
# Fri, 07 Feb 2020 02:52:53 GMT
ENV DOCKER_VERSION=19.03.6-rc2
# Fri, 07 Feb 2020 02:53:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 07 Feb 2020 02:53:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 07 Feb 2020 02:53:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 07 Feb 2020 02:53:03 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Feb 2020 02:53:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 07 Feb 2020 02:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Feb 2020 02:53:06 GMT
CMD ["sh"]
# Fri, 07 Feb 2020 02:53:31 GMT
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
	-	`sha256:249007935e7995946e79e82a9ef14e3a3c4f028a3b7c73829321a7b1453896de`  
		Last Modified: Fri, 07 Feb 2020 02:54:25 GMT  
		Size: 57.3 MB (57348932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751604cc05a5cab2aeaf3ce464c37bcabb1be7bb5baeb1b3499ea205162b125d`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8810f9ed256bb873912d7282fedf94bc1d77ceb06d292224ad501e07aca584d`  
		Last Modified: Fri, 07 Feb 2020 02:54:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c929a236b4bd53fadd68dd1ac83e72a232c507a88eb904185b2bdfbb89d6936a`  
		Last Modified: Fri, 07 Feb 2020 02:54:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5179ea1a503390358687888ca828868daf9b9459fec0da0a959e33bfc89fed`  
		Last Modified: Fri, 07 Feb 2020 02:54:55 GMT  
		Size: 8.4 MB (8406026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
