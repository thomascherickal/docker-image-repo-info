## `docker:dind-rootless`

```console
$ docker pull docker@sha256:7a3fefa66c6c82f45e46c28ebeb1c8fc39a114ea6982ac236fdb2b6ba651e467
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:baab922c357ece896d896bfb211f27102de68e16ebe1d82e2a04516db6183631
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102535610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c017c761a04cf814673eae5c3e4dc6075a3e698d60aa9ea06867ddce83d9a4c0`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 07:56:00 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 26 Mar 2021 07:56:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 26 Mar 2021 07:56:01 GMT
ENV DOCKER_VERSION=20.10.5
# Fri, 26 Mar 2021 07:56:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.5.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 26 Mar 2021 07:56:07 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 26 Mar 2021 07:56:07 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:56:07 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 26 Mar 2021 07:56:08 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 26 Mar 2021 07:56:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 07:56:08 GMT
CMD ["sh"]
# Fri, 26 Mar 2021 07:56:14 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 26 Mar 2021 07:56:15 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 26 Mar 2021 07:56:15 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 26 Mar 2021 07:56:17 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 26 Mar 2021 07:56:17 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:56:17 GMT
VOLUME [/var/lib/docker]
# Fri, 26 Mar 2021 07:56:17 GMT
EXPOSE 2375 2376
# Fri, 26 Mar 2021 07:56:17 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 26 Mar 2021 07:56:18 GMT
CMD []
# Fri, 26 Mar 2021 07:56:22 GMT
RUN apk add --no-cache iproute2
# Fri, 26 Mar 2021 07:56:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 26 Mar 2021 07:56:24 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 26 Mar 2021 07:56:27 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.5.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 26 Mar 2021 07:56:28 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 26 Mar 2021 07:56:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 26 Mar 2021 07:56:28 GMT
USER rootless
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8aba36c48bdd8a8a32e7d5f4a2f99baaf3cfcb07d9252c9c24ce06689a7152`  
		Last Modified: Fri, 26 Mar 2021 07:57:44 GMT  
		Size: 2.1 MB (2050069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42621afb2e170dae0ffca17d04117dcc72ee595bd65f98cb2346740a7281213`  
		Last Modified: Fri, 26 Mar 2021 07:57:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb57477e3a83bb86296e7aa42ee5d54a7d39f2ebd178642885542a2336c796`  
		Last Modified: Fri, 26 Mar 2021 07:57:53 GMT  
		Size: 69.7 MB (69692157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5938d06b30e7b841fa1764eb1be6fd8d1f979c8f328f88b3d02a4e5b8cdcef47`  
		Last Modified: Fri, 26 Mar 2021 07:57:41 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a259f6e9d5125d07f1a1b59bf26e334dbc888d35dec4ac0b39ba1aa116caea23`  
		Last Modified: Fri, 26 Mar 2021 07:57:41 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ba9c27bd792c8d366365ecff9487c735f225b8cbf9aeb6ba4fab632e0d4cbd`  
		Last Modified: Fri, 26 Mar 2021 07:57:41 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe52de4eb78f716b8d54c442b82481271bcd0d3a151a08cbfc343fef597e8fa`  
		Last Modified: Fri, 26 Mar 2021 07:58:11 GMT  
		Size: 6.6 MB (6610543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1af7795c3a64e171f2e62db130414f86d0cc980d9be262c9a7d66e2e578fd1b`  
		Last Modified: Fri, 26 Mar 2021 07:58:10 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a720caae7ad13bec16874fe8f38ce1c843731fef9f44cb826c226159aa99764`  
		Last Modified: Fri, 26 Mar 2021 07:58:10 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c939cc4c164a0aca452362a88d72ededc61d36579e49a741b10297f14c2240`  
		Last Modified: Fri, 26 Mar 2021 07:58:10 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d28ba8963fac279c5a52a9eb475b79b6777edb7dfb0658733a55e5a6777dabc`  
		Last Modified: Fri, 26 Mar 2021 07:58:29 GMT  
		Size: 1.1 MB (1131823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd0f01dcfa54278db4f171d06096d9e01623f1895646b4622fd86c49d9b2e5`  
		Last Modified: Fri, 26 Mar 2021 07:58:28 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e81d53baa4c140dafd31786692e4fe894cb1391095a24d9c42693e9cb079fa`  
		Last Modified: Fri, 26 Mar 2021 07:58:28 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41e5d015ed6e5b7a18fb973782adb78fc93513f4b54886cea89eb64fb41da1b`  
		Last Modified: Fri, 26 Mar 2021 07:58:32 GMT  
		Size: 20.2 MB (20231016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bccdbc1efbfed45961a2c9503268ac309d500773cc050be42e956c9cb3634`  
		Last Modified: Fri, 26 Mar 2021 07:58:28 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
