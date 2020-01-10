## `docker:dind`

```console
$ docker pull docker@sha256:cc1a5397bee3e3afb94d79c01d874c5976a8c400118c7e388514544d88022caa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:60f3ae738c53cf6f10f662a24a3ef2b167ced132d3bff6aa88c82bb1edeb70d0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74622037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a90db1182c9918852511b20856a6526a32e704bbfa3e342b8022fc00f1e63e94`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 24 Dec 2019 19:20:12 GMT
ADD file:36fdc8cb08228a87093fb227736f4ce1d4d6c15366326dea541fbbd863976ee5 in / 
# Tue, 24 Dec 2019 19:20:12 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:22:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 26 Dec 2019 21:22:15 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 Dec 2019 21:22:15 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 26 Dec 2019 21:22:15 GMT
ENV DOCKER_VERSION=19.03.5
# Thu, 26 Dec 2019 21:22:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 26 Dec 2019 21:22:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 26 Dec 2019 21:22:22 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 26 Dec 2019 21:22:22 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Dec 2019 21:22:23 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 26 Dec 2019 21:22:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Dec 2019 21:22:24 GMT
CMD ["sh"]
# Thu, 26 Dec 2019 21:22:30 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 26 Dec 2019 21:22:31 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 26 Dec 2019 21:22:31 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Thu, 26 Dec 2019 21:22:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 26 Dec 2019 21:22:32 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Thu, 26 Dec 2019 21:22:32 GMT
VOLUME [/var/lib/docker]
# Thu, 26 Dec 2019 21:22:33 GMT
EXPOSE 2375 2376
# Thu, 26 Dec 2019 21:22:33 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 26 Dec 2019 21:22:33 GMT
CMD []
```

-	Layers:
	-	`sha256:e6b0cf9c0882fb079c9d35361d12ff4691f916b6d825061247d1bd0b26d7cf3f`  
		Last Modified: Tue, 24 Dec 2019 19:20:40 GMT  
		Size: 2.8 MB (2801778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb3b77ad49c7f3dc1e1240949ada3332fc07949a5fd88bf85ceb284c069509d`  
		Last Modified: Thu, 26 Dec 2019 21:23:12 GMT  
		Size: 2.4 MB (2425153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49ead4c98e3d4d53ca8b2a765a8043f9fb5a3527c1b5d9190b483cb5efbdace`  
		Last Modified: Thu, 26 Dec 2019 21:23:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63462afa1330adf1e85f53d5f34449210b4810e791e2c79ec8d2218e550cc06e`  
		Last Modified: Thu, 26 Dec 2019 21:23:24 GMT  
		Size: 63.8 MB (63803055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0637d9fbe54c3be5da0310206745b1fb212029acf8c780e33cf37c11c5d80026`  
		Last Modified: Thu, 26 Dec 2019 21:23:11 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901dbaeb8b4aa6ef7d8d474e91c43ec83a7393dccf619116c142a4ddd7c4b849`  
		Last Modified: Thu, 26 Dec 2019 21:23:11 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3652bd79826fd0fb2159012fdfd5aac6290f7be722db70ba4e5aaa331fec88`  
		Last Modified: Thu, 26 Dec 2019 21:23:11 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ec5d62350d3cda807f7e704c87d57b10fb1ba85fe1f699e21f84ad5c27c3f2`  
		Last Modified: Thu, 26 Dec 2019 21:23:30 GMT  
		Size: 5.6 MB (5585653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33bd47420cfb04992ddff758284e17deb3e37d458561f6406509ceffbf8f961`  
		Last Modified: Thu, 26 Dec 2019 21:23:29 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa446682b03f5fef5287800942831e4df43e14496e0cbb951b557e9f6768267f`  
		Last Modified: Thu, 26 Dec 2019 21:23:29 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0558cf2aea5c752da89127f633b2a7bd9f21b7fbc37a193e1bc94d518b07f551`  
		Last Modified: Thu, 26 Dec 2019 21:23:29 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:b9c43fe631267f357df2985d3c3f7e70138c48b64cff93784c2eae59788d9990
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67723193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faead06f30f7cbd84302c7d35db261fc005a4c3afa745dca913999d73253e9f7`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:50:48 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 26 Dec 2019 21:50:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 Dec 2019 21:50:52 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 26 Dec 2019 21:50:53 GMT
ENV DOCKER_VERSION=19.03.5
# Thu, 26 Dec 2019 21:51:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 26 Dec 2019 21:51:08 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 26 Dec 2019 21:51:09 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 26 Dec 2019 21:51:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Dec 2019 21:51:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 26 Dec 2019 21:51:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Dec 2019 21:51:16 GMT
CMD ["sh"]
# Thu, 26 Dec 2019 21:51:30 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 26 Dec 2019 21:51:35 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 26 Dec 2019 21:51:37 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Thu, 26 Dec 2019 21:51:42 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 09 Jan 2020 23:49:49 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Thu, 09 Jan 2020 23:49:53 GMT
VOLUME [/var/lib/docker]
# Thu, 09 Jan 2020 23:49:55 GMT
EXPOSE 2375 2376
# Thu, 09 Jan 2020 23:49:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 09 Jan 2020 23:49:57 GMT
CMD []
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478492ea0683b34ae904eef577598b09ce1dbe4230af7a3920720bb816e95191`  
		Last Modified: Thu, 26 Dec 2019 21:52:34 GMT  
		Size: 2.4 MB (2355396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3af0915702a94dc803895239d700514ff4b25b946a55c5feaa45887c6dd649`  
		Last Modified: Thu, 26 Dec 2019 21:52:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c9411ea300b6cb0357017a7622e46a795c7a7acd744893d1157858f9be65f7`  
		Last Modified: Thu, 26 Dec 2019 21:52:48 GMT  
		Size: 59.5 MB (59537091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193f1ebb3f7fc87e3bd0fb06d4453594906d54e705a7a7e438259429633cca29`  
		Last Modified: Thu, 26 Dec 2019 21:52:30 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21ae19a6988bc39dbec026bcd5c3533ea6c1f878e700d24b87fac38624d4cb4`  
		Last Modified: Thu, 26 Dec 2019 21:52:30 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84874978fd32476c30a94a54a06631d103a9144642b463482f821b4176dc03ff`  
		Last Modified: Thu, 26 Dec 2019 21:52:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19801c3696a606cdfa10376aad90fb833530e5c00b7390044bb59716f5344d69`  
		Last Modified: Thu, 26 Dec 2019 21:53:04 GMT  
		Size: 3.2 MB (3212221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fae31fe824fbbe7c619386711de4a2ac0bb416850127be04b103f664bbd7cf`  
		Last Modified: Thu, 26 Dec 2019 21:53:03 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b7d8d1ff5bbc65d1c330321373584880a3859b009a9e695d3399626867b558`  
		Last Modified: Thu, 26 Dec 2019 21:53:03 GMT  
		Size: 753.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbba0a5ba1e4a6d0dbf73d1e7efc438ff713c8324e30b4b56338769a562321f`  
		Last Modified: Thu, 09 Jan 2020 23:50:24 GMT  
		Size: 2.5 KB (2533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:9649ddd527935f66833e5f956446fa004f2fc4d3b04ddcb04b16ffc9546446bf
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67086665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e769ce7668390c87a7ce7d7adce81ce1d0019c9815cbb51f2ab96d88c2503bb`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 24 Dec 2019 18:59:09 GMT
ADD file:caf7ca25875eddd2bfa2d1e56663bb52d278a85f6ee1314f9ccf01dc4da8070a in / 
# Tue, 24 Dec 2019 18:59:10 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:01:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 26 Dec 2019 21:01:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 Dec 2019 21:01:51 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 26 Dec 2019 21:01:51 GMT
ENV DOCKER_VERSION=19.03.5
# Thu, 26 Dec 2019 21:02:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 26 Dec 2019 21:02:02 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 26 Dec 2019 21:02:03 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 26 Dec 2019 21:02:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Dec 2019 21:02:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 26 Dec 2019 21:02:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Dec 2019 21:02:07 GMT
CMD ["sh"]
# Thu, 26 Dec 2019 21:02:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 26 Dec 2019 21:02:18 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 26 Dec 2019 21:02:19 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Thu, 26 Dec 2019 21:02:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 09 Jan 2020 23:57:39 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Thu, 09 Jan 2020 23:57:42 GMT
VOLUME [/var/lib/docker]
# Thu, 09 Jan 2020 23:57:43 GMT
EXPOSE 2375 2376
# Thu, 09 Jan 2020 23:57:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 09 Jan 2020 23:57:45 GMT
CMD []
```

-	Layers:
	-	`sha256:3922e475e500b2739b5e74787fc80622853325822f71f8bd3de7e5b09654d60f`  
		Last Modified: Tue, 24 Dec 2019 18:59:33 GMT  
		Size: 2.4 MB (2416691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cee0efcbfb35406895e68c92bc2bbfb3447d96a7abb40d288629b4b60dbb7`  
		Last Modified: Thu, 26 Dec 2019 21:02:53 GMT  
		Size: 2.3 MB (2254389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616c380c09fcd10304ae95afaf65a56079f310bcd7660b163370efdf0b33a965`  
		Last Modified: Thu, 26 Dec 2019 21:02:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac8eb6de7546b474ea400c5f6d22a866ae4d7f2f6464cf86db2adb1213fb57e`  
		Last Modified: Thu, 26 Dec 2019 21:03:10 GMT  
		Size: 59.5 MB (59532264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95eb49dcdc6cb96b28a162723f7d13520268128fb0dee031e3205e7bb0bb5a26`  
		Last Modified: Thu, 26 Dec 2019 21:02:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b4531e095724b34fddfb3866f12630bc9e4c059191411ee8d896b8cc994e91`  
		Last Modified: Thu, 26 Dec 2019 21:02:51 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcae309c142f252026c7392e3ed4340e1de544c8175e791bc420106117a57fc6`  
		Last Modified: Thu, 26 Dec 2019 21:02:51 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1958f1bd036df3edf8860a0cdbf99ef8a1d34c053f4812b9d32f99acaf33c6bc`  
		Last Modified: Thu, 26 Dec 2019 21:03:27 GMT  
		Size: 2.9 MB (2876858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0091e1ec4c073c221cb6c4f2085c7e859299056cc8df8cba557acb067a84600`  
		Last Modified: Thu, 26 Dec 2019 21:03:27 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685a123dd0c5cb45703dc6a8b0cb7a72b005a6c4fb805828ba00dfbe4152cf89`  
		Last Modified: Thu, 26 Dec 2019 21:03:27 GMT  
		Size: 754.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d05165e79af063c32c1306a948c2d8f30d342babbdabead5ca075cfd81824e`  
		Last Modified: Thu, 09 Jan 2020 23:58:09 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c1087304065e5e870616897276df9bd622828cbe1550c8652af8c1a7cc25ed64
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67762772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9370a6266b0e5fea0d998c22dd4fbd9d2210ce15a8ab4b05331ffa7f9f3226c6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 24 Dec 2019 20:26:15 GMT
ADD file:d6c3db0313ab0c6201770c7248d1bac964011a1c08f1a9b434442b7c21efef87 in / 
# Tue, 24 Dec 2019 20:26:24 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:41:21 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 26 Dec 2019 21:41:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 Dec 2019 21:41:24 GMT
ENV DOCKER_CHANNEL=stable
# Thu, 26 Dec 2019 21:41:25 GMT
ENV DOCKER_VERSION=19.03.5
# Thu, 26 Dec 2019 21:41:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 26 Dec 2019 21:41:35 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 26 Dec 2019 21:41:36 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 26 Dec 2019 21:41:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Dec 2019 21:41:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 26 Dec 2019 21:41:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Dec 2019 21:41:40 GMT
CMD ["sh"]
# Thu, 26 Dec 2019 21:41:53 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 26 Dec 2019 21:41:56 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 26 Dec 2019 21:41:57 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Thu, 26 Dec 2019 21:42:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 09 Jan 2020 23:48:52 GMT
COPY file:e088145e3deff2cef88e32686489e5e86fdf5669c275cd1a877d11d740ab1a80 in /usr/local/bin/ 
# Thu, 09 Jan 2020 23:48:53 GMT
VOLUME [/var/lib/docker]
# Thu, 09 Jan 2020 23:48:53 GMT
EXPOSE 2375 2376
# Thu, 09 Jan 2020 23:48:54 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 09 Jan 2020 23:48:55 GMT
CMD []
```

-	Layers:
	-	`sha256:cde5963f3b93eec667cad527c99d80402a5a91a7a1381f7ffe562f215aec0c50`  
		Last Modified: Tue, 24 Dec 2019 20:26:52 GMT  
		Size: 2.7 MB (2719182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a539ce405eae7a9d400a4d8c2521b9a81fae3ba37efe207ed90c69a067870f`  
		Last Modified: Thu, 26 Dec 2019 21:42:42 GMT  
		Size: 2.4 MB (2445769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca65af24bce1d26d447c2c0aa91e1f4ccb6cd5d96c0280fdd8d40d48d9400fd3`  
		Last Modified: Thu, 26 Dec 2019 21:42:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a8beb42a78bdd1f883dbaef4f42326476f57bc5619e9e6fa76afb3dc7b1d46`  
		Last Modified: Thu, 26 Dec 2019 21:42:59 GMT  
		Size: 57.0 MB (57006195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62812bce294473719c18be945b890895fa606e5b9af98754472a8763179b19d8`  
		Last Modified: Thu, 26 Dec 2019 21:42:39 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5704281cbb022f2bd56d30c18b2343b29911d02bd76aac0afdef1676c0ff2c4b`  
		Last Modified: Thu, 26 Dec 2019 21:42:39 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e45b27f9399515bd037cab2b1a6b6e16bb333620ad8b8a01b465517eb083fda`  
		Last Modified: Thu, 26 Dec 2019 21:42:39 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c74405a7be2aec1082c15e263feed8780614581e8c9c696a829e2cd8ccfc423`  
		Last Modified: Thu, 26 Dec 2019 21:43:14 GMT  
		Size: 5.6 MB (5585152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3d101a79be03f2dc57dc67d9d5a7443616cf7da6cae0e72b363f34827f44fd`  
		Last Modified: Thu, 26 Dec 2019 21:43:13 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e1496e6873f629ea5b961d3dc789080c6012d79261228aeec0efd58f528d57`  
		Last Modified: Thu, 26 Dec 2019 21:43:13 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba22b18ae1908166eb8031343c535050210992d6e3006b701ae6884f5660c81`  
		Last Modified: Thu, 09 Jan 2020 23:49:17 GMT  
		Size: 2.5 KB (2542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
