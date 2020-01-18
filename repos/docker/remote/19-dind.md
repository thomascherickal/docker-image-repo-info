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
