## `docker:dind-rootless`

```console
$ docker pull docker@sha256:88bd12875df6cb64ffd3965a3977feb9c3a0fd1c971b9521534492d8cc818f3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:c574820d5eabf3bd03e11a911791178a30d5b90ba7daafbb52635aece6ec18ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95553909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18661e6d9122218fd4e0c88dc1e535ddbc477e8c2c64351efc251786a011e196`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 20:19:26 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 20:19:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 20:19:27 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 20:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 20:19:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:34 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 20:19:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:35 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 20:19:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 20:19:43 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:43 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 20:19:44 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 20:19:44 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 20:19:44 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 20:19:44 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 20:19:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 20:19:45 GMT
CMD []
# Wed, 15 Dec 2021 20:19:48 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 20:19:49 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 20:19:50 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 20:19:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 20:19:53 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 20:19:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 20:19:54 GMT
USER rootless
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea03e1895df432fba23ac2810a53a408fa25273ecf001276263d810107e1c81`  
		Last Modified: Wed, 15 Dec 2021 20:20:23 GMT  
		Size: 2.0 MB (1980404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff98835b05535c14c9bd8aa0449fd33d147a58c9a9fe7f21b76137065d0f4c5`  
		Last Modified: Wed, 15 Dec 2021 20:20:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f2dd7b7d653d57dbfc55dcef38007cf7ae05a4c1a226f4465b3723cb2232ed`  
		Last Modified: Wed, 15 Dec 2021 20:20:32 GMT  
		Size: 63.7 MB (63718464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182b62d4a3549bba88c6f8f32c2d7850ca927a7df0682d9a0de05d0c40095e2`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a57db2abd77c0b995c329d7812464e3734bc1af7b829bd1a42d461de77d3b7`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73490af52bd34939d0d8b02fe67c992943d062112c5a1cb41daf43146a25ae1b`  
		Last Modified: Wed, 15 Dec 2021 20:20:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d28806efd0ea428cf206cb382a31cb6fba2972e2e6e870051723dab28340158`  
		Last Modified: Wed, 15 Dec 2021 20:20:55 GMT  
		Size: 6.7 MB (6734098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97fd78563ff48a3ea4d64328aac35a97ef969306734b403631f8f8fb36d16e5`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaf1aff7f0b5974dc8e7b9ce5119cf168e186a2281887ebdb30b850059c51ec`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8eed8b923285e1979ee45a366bc2852d46843fc0ababa5c7de8d8009f25f757`  
		Last Modified: Wed, 15 Dec 2021 20:20:54 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4444124f7f8ff8ec85dd6ce1b2e709d524c897ac4115dee4d3fe112969a9e617`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.2 MB (1162106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03e82f9fb8f6b548ad22baa5fc4b53ed561d820d967f4da8cc9bd05f79c07ce`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dfe6db0ec7ad8e0fbf82c9af2fb052312f40985759a422df8c58d35e5a3635`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32afcbc4731321210e9b6e0741bcd6b694b0159fb3ae1ba6d5a327a0f0086bb7`  
		Last Modified: Wed, 15 Dec 2021 20:21:23 GMT  
		Size: 19.1 MB (19131953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902dceede3bc9a25497aeffa6125b18a89aea3e313b20a944f50f4f03d397c3`  
		Last Modified: Wed, 15 Dec 2021 20:21:20 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0b938ec7ea96b1f40863ecc7b01be4cf348c84800b9ccd38bf86126655426da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.3 MB (91316335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d4b842a15fcdb0104cacdbba294e63bcf3d1714af7ef34ddfbc5b8972f95bcd`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 15 Dec 2021 19:39:37 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 15 Dec 2021 19:39:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 15 Dec 2021 19:39:38 GMT
ENV DOCKER_VERSION=20.10.12
# Wed, 15 Dec 2021 19:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.12.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.12.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 15 Dec 2021 19:39:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 15 Dec 2021 19:39:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:39:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 15 Dec 2021 19:39:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 15 Dec 2021 19:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Dec 2021 19:39:48 GMT
CMD ["sh"]
# Wed, 15 Dec 2021 19:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 15 Dec 2021 19:39:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:00 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 15 Dec 2021 19:40:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 15 Dec 2021 19:40:03 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 15 Dec 2021 19:40:03 GMT
VOLUME [/var/lib/docker]
# Wed, 15 Dec 2021 19:40:04 GMT
EXPOSE 2375 2376
# Wed, 15 Dec 2021 19:40:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 15 Dec 2021 19:40:06 GMT
CMD []
# Wed, 15 Dec 2021 19:40:14 GMT
RUN apk add --no-cache iproute2
# Wed, 15 Dec 2021 19:40:14 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 15 Dec 2021 19:40:15 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 15 Dec 2021 19:40:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.12.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.12.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 15 Dec 2021 19:40:18 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 15 Dec 2021 19:40:19 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 15 Dec 2021 19:40:20 GMT
USER rootless
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1339a3be518a98fb1ef64708d14d86fd4039c4bb0a3d1db8c2d4a4c00fb8a2`  
		Last Modified: Wed, 15 Dec 2021 19:41:10 GMT  
		Size: 1.9 MB (1949540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353862b30dd70efe72e0bf55133d47f2a5b000e37f9cdb0e7e4a0178a5f076ec`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3190c06c4855888df747c4f505d0bc7aaecfbb0d9d4acaee685e28bddfb99b`  
		Last Modified: Wed, 15 Dec 2021 19:41:16 GMT  
		Size: 57.7 MB (57747213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55e216c2ebb46ec0635d982e57890ab4c9025c95a940e79a81a0ed8b50c49b6`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46f33417cc9574bd0139314cc88909fae8f672527fc69f493d406dad1991e1`  
		Last Modified: Wed, 15 Dec 2021 19:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c99da1af64cbeec415a8ce2302a76874846814f574e07e7d9072e70ad00192`  
		Last Modified: Wed, 15 Dec 2021 19:41:07 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12055a90557dd8852e5d26b75d39ee8c5bb53795e2df51b883cc60bf8d765aee`  
		Last Modified: Wed, 15 Dec 2021 19:41:39 GMT  
		Size: 6.6 MB (6612548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd11f99968f9c201fb0dcc9d59bcd8653f16ef5b376446a563ca41ec400751`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482d3fe6b24fb02fce911311cdbd9069d2a150c94dca0d5fcc85cf4b30b21b7`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7dc2dffdacf12cfe5762299899abbc48a89a3be50f8a7c62933935cdc3c9c2`  
		Last Modified: Wed, 15 Dec 2021 19:41:36 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d670443b55fd7ca190ef7e74937f339344c982fc891932721e85c0258f6a99`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.2 MB (1178051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32d2d69d1f3c01aa88625f185c33e9d81afc49cae7c69e60188ea8e33edfb44`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4374d2147deadc7d22f890fc9782880efb5b1f173e4c9532601ecc19dc672bc3`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17554114a98827967270ad33a848b60df2da91189aa8f7b5e96d201e26e97347`  
		Last Modified: Wed, 15 Dec 2021 19:42:03 GMT  
		Size: 21.1 MB (21105227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a74d2bf287bf033007cdbf327593f6b8e1a14edf5106b8a6bd75474eb22c435`  
		Last Modified: Wed, 15 Dec 2021 19:42:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
