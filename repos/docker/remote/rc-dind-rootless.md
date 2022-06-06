## `docker:rc-dind-rootless`

```console
$ docker pull docker@sha256:ab0c2c8440ac1dc57509c31a2ec3a78c22371ca27e0031a6218a98b8256d3a8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5f35a22a6237a9d6156de30ff19eb4b4ec21d3efa821475842741240b5eae9df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95244762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11315f1e3d51a31f7e66cc17b2135b89aa716b335c6881d409022365201e821f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 22:19:34 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 01 Sep 2021 22:19:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 22:19:21 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 22:19:27 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 22:19:27 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 22:19:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 22:19:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 22:19:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 22:19:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 22:19:29 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 22:19:34 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 22:19:35 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 22:19:35 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 22:19:36 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 22:19:36 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 22:19:37 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 22:19:37 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 22:19:37 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 22:19:37 GMT
CMD []
# Mon, 18 Oct 2021 22:19:41 GMT
RUN apk add --no-cache iproute2
# Mon, 18 Oct 2021 22:19:42 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 18 Oct 2021 22:19:43 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 18 Oct 2021 22:19:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 18 Oct 2021 22:19:46 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 18 Oct 2021 22:19:46 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 18 Oct 2021 22:19:46 GMT
USER rootless
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14df950e5a796f46eb6615169002a1c428bd908141de49fb35ec026c206e77aa`  
		Last Modified: Wed, 01 Sep 2021 22:20:33 GMT  
		Size: 1.9 MB (1935099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a31cc9e913427e8959328b7d290bdcc639a9f84c11956c33c0ce112788cf19`  
		Last Modified: Wed, 01 Sep 2021 22:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccfef21a1ba86a2a49122b42c2b6894a1fb8b832279017d10fcf3799e95d5f0`  
		Last Modified: Mon, 18 Oct 2021 22:20:47 GMT  
		Size: 63.7 MB (63691665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443ed9bdac873af3eff9398dbc77b000df4a4c25ef3a78ced87e178ff1c92645`  
		Last Modified: Mon, 18 Oct 2021 22:20:35 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51846a1759acabeb7964b68eb7c183c0668a5ff1175ac9b1952fc4949b649cf`  
		Last Modified: Mon, 18 Oct 2021 22:20:36 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ab21c0404cdc3f3a67b807ff478d3a3d705a4a37c4bc9e3b922ca8e984a2fd`  
		Last Modified: Mon, 18 Oct 2021 22:20:35 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425931fed24edf6259d6a6ddd00725a7195a42dd7bc0b70b0cc18d0d1aaa4396`  
		Last Modified: Mon, 18 Oct 2021 22:21:04 GMT  
		Size: 6.5 MB (6521438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a87d63582576ec7a470e771f6c5d16ff7cb7338024ea93995f04bfb4fe1199f`  
		Last Modified: Mon, 18 Oct 2021 22:21:02 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9e7e65b6f97a6d64f396fdfbbfdf24802e58a822b16eea7a8992dd36b39f88`  
		Last Modified: Mon, 18 Oct 2021 22:21:03 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f06cc2cbb18da705b3065ac5c595df3809a82b8ea5e3763fd8fe50d96590e03`  
		Last Modified: Mon, 18 Oct 2021 22:21:02 GMT  
		Size: 2.6 KB (2619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48282e6bb68b3cd85c6888c382ce44c03aac4a0c3ddc81d442dfc72efe84aae`  
		Last Modified: Mon, 18 Oct 2021 22:21:20 GMT  
		Size: 1.1 MB (1148742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b3f4f2b7dacb4399397b7cac7bbfd3328746289da0eacacdde2b936a389390`  
		Last Modified: Mon, 18 Oct 2021 22:21:20 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abe8559ece6fc51061309e75b0be253306e8b9d26e64c2ecf486041a51b52f4`  
		Last Modified: Mon, 18 Oct 2021 22:21:20 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f177d2e28217b973c3b8bc08c5d5a743e443de5daa815086e05848b46b7db`  
		Last Modified: Mon, 18 Oct 2021 22:21:24 GMT  
		Size: 19.1 MB (19124895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280a62307b878257d2128209fd92a1005e52eddf1a1409ef3770d74fc4122e92`  
		Last Modified: Mon, 18 Oct 2021 22:21:20 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:036139df2869c66580cf19c3f5e10fbfcdc51e44e4c253dd52461dbaf8756d1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.0 MB (91048708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592281427bbc8f0ac33cd2c8cc861023d89fe8804da4082b826bb8976bf55339`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 21:39:51 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 18 Oct 2021 21:39:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Oct 2021 21:39:53 GMT
ENV DOCKER_VERSION=20.10.10-rc1
# Mon, 18 Oct 2021 21:39:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-20.10.10-rc1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-20.10.10-rc1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Mon, 18 Oct 2021 21:40:00 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 18 Oct 2021 21:40:01 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:01 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 18 Oct 2021 21:40:02 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 18 Oct 2021 21:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:04 GMT
CMD ["sh"]
# Mon, 18 Oct 2021 21:40:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 18 Oct 2021 21:40:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:14 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 18 Oct 2021 21:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 18 Oct 2021 21:40:17 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Mon, 18 Oct 2021 21:40:17 GMT
VOLUME [/var/lib/docker]
# Mon, 18 Oct 2021 21:40:18 GMT
EXPOSE 2375 2376
# Mon, 18 Oct 2021 21:40:19 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 18 Oct 2021 21:40:20 GMT
CMD []
# Mon, 18 Oct 2021 21:40:27 GMT
RUN apk add --no-cache iproute2
# Mon, 18 Oct 2021 21:40:28 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 18 Oct 2021 21:40:29 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 18 Oct 2021 21:40:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-20.10.10-rc1.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 18 Oct 2021 21:40:33 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 18 Oct 2021 21:40:34 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 18 Oct 2021 21:40:35 GMT
USER rootless
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b9844ac93b529c1f52e7d493f8e6fe6192353fb1fb922d21c6170008e114d7`  
		Last Modified: Mon, 18 Oct 2021 21:42:47 GMT  
		Size: 1.9 MB (1909462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44145fb8198137b43c7a8143d29d785c2d628a41f9dd2d2c39a779bf8d89b128`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112f3374d6fabbfe7b2c992c077ac3658ff8d061a8e18265257b45cd60739c0d`  
		Last Modified: Mon, 18 Oct 2021 21:42:54 GMT  
		Size: 57.7 MB (57731459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ffe46428f8f4e7d13099151a78aa124e254522444b80d46bcec4e3e3fc41eb`  
		Last Modified: Mon, 18 Oct 2021 21:42:44 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6699487bf567a986ddfb631b8655b487e6922d4a86ee9ff17b738d32ae342fa7`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f64888be82e82dc404000ef04193fab09949191aa4a5abd16eb3f76de6422`  
		Last Modified: Mon, 18 Oct 2021 21:42:45 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6501ba4a4760252cf7cc02d607ee723591654cc0bb5f52520a6e33dc7a0edc25`  
		Last Modified: Mon, 18 Oct 2021 21:43:12 GMT  
		Size: 6.4 MB (6418461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a680b385ce15bb20e7ba5ac40667562dec340d2d81461023bdf90c3e3fabbebd`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f199395c417cc0c7e6398feae5d9baf39d65e2e0a7bb70170c70b89e589e8dfe`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1aee83547715d6f96b27af07d2631947e319c0f257cbebfed3719ab3e20529`  
		Last Modified: Mon, 18 Oct 2021 21:43:10 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375da3ba74accf4f4e776d8ea0d05c23a13b4b2b720c68351e5a106a84dda6e3`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 1.2 MB (1167846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ac90cf496368c08bead07501a2fb6bcf1be125a482b1ba65545eb127ade900`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1a7298291f6aaebb45b8b88842f7e71ac8c03b3ba86694de07dcba597dce8b`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f92a9eb80f5eb157bb083cbb43ee01b129e3a55ba704b5f14a5e73d3957e05f`  
		Last Modified: Mon, 18 Oct 2021 21:43:32 GMT  
		Size: 21.1 MB (21101330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6559ad5989ef407de45b61e2a3ebc564a674911a70765ee6abc411c6c43b88b2`  
		Last Modified: Mon, 18 Oct 2021 21:43:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
