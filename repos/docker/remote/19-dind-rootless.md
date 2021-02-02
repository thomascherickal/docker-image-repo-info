## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:259dbf2fe0cc6d23c2a42caf0da1f0778fc850c26301657800fcc7d70086cd7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:711ea28bf1f83af6b95c7122285a72af394304666c1b0bb74cc204cf0dd945ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94877543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32b072e6af370115fea331dd17919372cce51fa1e8c342b1a4c5d1eb4fc06e90`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Tue, 02 Feb 2021 02:12:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 02 Feb 2021 02:12:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Feb 2021 02:13:09 GMT
ENV DOCKER_VERSION=19.03.15
# Tue, 02 Feb 2021 02:13:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 02 Feb 2021 02:13:17 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 02 Feb 2021 02:13:19 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 02 Feb 2021 02:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:19 GMT
CMD ["sh"]
# Tue, 02 Feb 2021 02:13:25 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 02 Feb 2021 02:13:26 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:26 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Tue, 02 Feb 2021 02:13:28 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 02 Feb 2021 02:13:28 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Tue, 02 Feb 2021 02:13:28 GMT
VOLUME [/var/lib/docker]
# Tue, 02 Feb 2021 02:13:28 GMT
EXPOSE 2375 2376
# Tue, 02 Feb 2021 02:13:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 02 Feb 2021 02:13:29 GMT
CMD []
# Tue, 02 Feb 2021 02:13:34 GMT
RUN apk add --no-cache iproute2
# Tue, 02 Feb 2021 02:13:35 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 02 Feb 2021 02:13:36 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 02 Feb 2021 02:13:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 02 Feb 2021 02:13:40 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 02 Feb 2021 02:13:40 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 02 Feb 2021 02:13:40 GMT
USER rootless
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f804d31884ef9e5356531d66ea8414eb307bdcb41a9b6a54e641848db51129`  
		Last Modified: Tue, 02 Feb 2021 02:14:15 GMT  
		Size: 2.1 MB (2051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a73bd8bacd2fc1e4269672c9cc3c1df45395893fca6720305fe06deca599913`  
		Last Modified: Tue, 02 Feb 2021 02:14:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4db05ddd5899af30ee0c5795aec2b49ac9d71df0cc4cb94f6e0dd1a9d444b02`  
		Last Modified: Tue, 02 Feb 2021 02:15:09 GMT  
		Size: 62.9 MB (62882884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b5eba8b232ce16e5ee1c005b5474ce8c4ace39ebb54702cc2bd6494566636b`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bece180336fa27595ce33fedc51ec456725fa8da0fc5501ad698ab630352f15`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ed15b4f9e6397f01e3e062ac8fd3c0963368a642364660b3ce1de4fa7da789`  
		Last Modified: Tue, 02 Feb 2021 02:14:56 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a63ba1d9089b3bebe2f96e7531317a35bc1b9ee116a34230036cfb0c9dfce17`  
		Last Modified: Tue, 02 Feb 2021 02:15:16 GMT  
		Size: 6.6 MB (6569583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbbb8fe7a5d45862302213cc2177f69dd10b125332de13a02d16dbfca7eddbf`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b267352ad78ddb70e7fdf7d8904ee6ccdfddce228541c8fbbff0d1fde2785be6`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8000174dfbac9b913dd3a6f82102a020e542eb48afe878dccf5a75f237dba345`  
		Last Modified: Tue, 02 Feb 2021 02:15:15 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4e48614a44dbccd302d9c92fc5a86a79e863407c4430ee408de62defc66e3`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 1.1 MB (1131433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff619e5e99aaf0556af66c31f305e3b054d8919f548d75b6abc09569bad530fe`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17a0e7edbf7c145009ebf83b802edaae0acd03cbf04c6364ea3dfa4b85b22c9`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a87220e4b94b4e720025144dae539d9e7a18dea719110830f32e76eeab0ea`  
		Last Modified: Tue, 02 Feb 2021 02:15:25 GMT  
		Size: 19.4 MB (19422701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e608ad6fa13da7ec47bdb2d866d9b83da78fb3de0e3f38dc4d099523608c63`  
		Last Modified: Tue, 02 Feb 2021 02:15:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
