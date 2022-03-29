## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:77d76cfdb1b09f4e7e8c9504de60946505cd9e6f4cd1e51a2739c6bbed8874fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:4e4e5426e9189d088d01d49d5f12495257c1b6f833966205cd34375f9c83fe76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96431045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:901a49bfc43b7f98ffcdd1aa26811571d1eb434164d9c35ba0dd3ec8e1fd7113`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 16:14:46 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Wed, 23 Mar 2022 16:14:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 05:19:29 GMT
ENV DOCKER_VERSION=20.10.14
# Thu, 24 Mar 2022 05:19:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 24 Mar 2022 05:19:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 24 Mar 2022 05:19:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 24 Mar 2022 05:19:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 24 Mar 2022 05:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:38 GMT
CMD ["sh"]
# Thu, 24 Mar 2022 05:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 24 Mar 2022 05:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:45 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 24 Mar 2022 05:19:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 24 Mar 2022 05:19:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 24 Mar 2022 05:19:46 GMT
VOLUME [/var/lib/docker]
# Thu, 24 Mar 2022 05:19:46 GMT
EXPOSE 2375 2376
# Thu, 24 Mar 2022 05:19:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 24 Mar 2022 05:19:46 GMT
CMD []
# Thu, 24 Mar 2022 05:19:50 GMT
RUN apk add --no-cache iproute2
# Thu, 24 Mar 2022 05:19:50 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 24 Mar 2022 05:19:51 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 24 Mar 2022 05:19:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 24 Mar 2022 05:19:54 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 24 Mar 2022 05:19:54 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 24 Mar 2022 05:19:54 GMT
USER rootless
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236b952b9466b604bbc4e060a2667d7a7a335bee006fd5104c151dbdb4bf787`  
		Last Modified: Wed, 23 Mar 2022 16:15:39 GMT  
		Size: 2.0 MB (1969538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2580f7437ec44a9dd3670ee6fd964ecb068808106d1bd8b961e7a568ef3ceb4f`  
		Last Modified: Wed, 23 Mar 2022 16:15:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0577d395ae504f47fad1c4d36855a3577354d4f0eca32daf7e0b13cf768c17`  
		Last Modified: Thu, 24 Mar 2022 05:20:29 GMT  
		Size: 64.6 MB (64611627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a33444f604b483769f304acdb1c976a4ea78d16943f3be3f9814e1a1e495f`  
		Last Modified: Thu, 24 Mar 2022 05:20:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8453fa1b01e46b0305c4d091304622803430cc8d0b3edb47c7be3a951e62e3`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2e8e864d7d32b260f5ca60b2065242e7c51ccaa371f2cc9807d0c32b2ec06f`  
		Last Modified: Thu, 24 Mar 2022 05:20:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a66f354bc1c7dbe0f8a4b91950340d2866bdbc96f2242a3bfa44d783c053f9c`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 6.7 MB (6734776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c10722ade4d16c23d283767216f390533cfb55769e6033eea8c7f4a8a4dc2`  
		Last Modified: Thu, 24 Mar 2022 05:20:47 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78397fa147a16e3ed2f3d8231cf9588472123760e352ca95983aeb96d333a43e`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa763b179fa70cb6a2ad1b6bf60c036a10f3b92e0372b67ed05efdf265e1fea`  
		Last Modified: Thu, 24 Mar 2022 05:20:46 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6085587cb5f72c79568b29cd55f4c3913866e9ed6397eaa76661ce55d266be`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.2 MB (1161988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a25e47e24f1be9958fc51661a544e64751645608e5cedff2dda9dbc3f4e39c`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05797a2b73a664a83ba4a1baf3ec188f150e43ced3f5c9b0d9b695f614e82e31`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a221d919a583960b7e36174c14532d2a479dbff4a227c548323d06c4b423ab`  
		Last Modified: Thu, 24 Mar 2022 05:21:09 GMT  
		Size: 19.1 MB (19131826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daedd33adc3be410c282f07f922a10bbbfa3f6b0564eb37b71b60de416300b2a`  
		Last Modified: Thu, 24 Mar 2022 05:21:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:7de587d995b63425b4259e844f4b7fae2da8aace781cef932a9527543d848276
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92134278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0cd8574e21f5c51c032be3097f830805605216e2002fc98285c751e5c876d39`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:26:13 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 29 Mar 2022 08:26:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:26:15 GMT
ENV DOCKER_VERSION=20.10.14
# Tue, 29 Mar 2022 08:26:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.14.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.14.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 29 Mar 2022 08:26:23 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 29 Mar 2022 08:26:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:26:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 29 Mar 2022 08:26:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 29 Mar 2022 08:26:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 08:26:27 GMT
CMD ["sh"]
# Tue, 29 Mar 2022 08:26:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 29 Mar 2022 08:26:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 29 Mar 2022 08:26:39 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 29 Mar 2022 08:26:40 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 29 Mar 2022 08:26:42 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:26:42 GMT
VOLUME [/var/lib/docker]
# Tue, 29 Mar 2022 08:26:43 GMT
EXPOSE 2375 2376
# Tue, 29 Mar 2022 08:26:44 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 29 Mar 2022 08:26:45 GMT
CMD []
# Tue, 29 Mar 2022 08:26:54 GMT
RUN apk add --no-cache iproute2
# Tue, 29 Mar 2022 08:26:54 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 29 Mar 2022 08:26:55 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 29 Mar 2022 08:26:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.14.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.14.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 29 Mar 2022 08:26:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 29 Mar 2022 08:27:00 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 29 Mar 2022 08:27:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab8992fcbba1f8070f63d991ae72bed38408b25db7ffa00f7221352fe9275c5`  
		Last Modified: Tue, 29 Mar 2022 08:27:55 GMT  
		Size: 1.9 MB (1938918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afedb10a1343d3055a1a213063d8f8f6ea1882b01069a44faf0453b0041a802d`  
		Last Modified: Tue, 29 Mar 2022 08:27:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f3009765e88f09be3c6e87a57258d5bea877cf248e4b0a6acd198692f300ef`  
		Last Modified: Tue, 29 Mar 2022 08:28:02 GMT  
		Size: 58.6 MB (58565750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae115253e7c71f61aa1bcdfde46cc38e0de6c3fb34bf4d1cebeca0b9bc91cc4`  
		Last Modified: Tue, 29 Mar 2022 08:27:52 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb3afcdfd642c0cd2ac3c0e03dfccaf3352874a7ccf06e91ce2e8c9d5a5a513`  
		Last Modified: Tue, 29 Mar 2022 08:27:52 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d2cdfcd569d13d88d038acf7b68fdc926a532b0f7e7480c3c80ebcf05bd31`  
		Last Modified: Tue, 29 Mar 2022 08:27:52 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d864000173cc86daa6e55100b01d994be24f6b8c559c5e76ef99bde7be746d`  
		Last Modified: Tue, 29 Mar 2022 08:28:23 GMT  
		Size: 6.6 MB (6615610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9335a5b964e837fcf57af4a0bb908694439e5c2353921af801ef7bf8c6e85a`  
		Last Modified: Tue, 29 Mar 2022 08:28:22 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0095e6dad21f8818c0137577f1ca43ac3aec53dea5ae540842f0aa5f3876e78`  
		Last Modified: Tue, 29 Mar 2022 08:28:22 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e754d309d56b8d770f6b3859fc6c3996c840f31decd785e6c644d432c93ab458`  
		Last Modified: Tue, 29 Mar 2022 08:28:22 GMT  
		Size: 2.7 KB (2745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9cd2d9598f1fe4d3e31f530b587846630feeddf9f81e758bc6e2be58dfee75`  
		Last Modified: Tue, 29 Mar 2022 08:28:44 GMT  
		Size: 1.2 MB (1177968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f04c0a5e9bca029e1cb5248b4a3b240b8076292c568464ebad797be38ccd1b7`  
		Last Modified: Tue, 29 Mar 2022 08:28:43 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab7129a628a3e4c5ee9c74357935e9145f0a302df09d25c508ba16215018a05`  
		Last Modified: Tue, 29 Mar 2022 08:28:44 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af21fbff071b5dfc4a65fcfd9c1bd353541f4e0fed929a4a68e3cf594e3c00b5`  
		Last Modified: Tue, 29 Mar 2022 08:28:47 GMT  
		Size: 21.1 MB (21111240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e31c8efa4d57102244c35627faef6bcdf00649b089f2f0a100fdf6d1b2c5c1`  
		Last Modified: Tue, 29 Mar 2022 08:28:43 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
