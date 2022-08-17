## `docker:dind-rootless`

```console
$ docker pull docker@sha256:2adc21dc54d844ac3d7a1632670bc541d2876a2efb766ee9e412dd07a932a36c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:5105e2543dd94f57526bbf7ed48340369b0e705726540e1ca97e8cc0c95a5d3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122524699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42a5d6f040bb9ae643a0c53d5dd2ce0007f0603a7ad19b9d2191e82a97d1d49c`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:48 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 09 Aug 2022 18:20:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:21:25 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 09 Aug 2022 18:21:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 17 Aug 2022 01:38:38 GMT
ENV DOCKER_BUILDX_VERSION=0.9.0
# Wed, 17 Aug 2022 01:38:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.0/buildx-v0.9.0.linux-amd64'; 			sha256='513e2cb7e71a21e20ae7709eb2fcc98d66117bd440d98602a84835e5cd3179bf'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.0/buildx-v0.9.0.linux-arm-v6'; 			sha256='fe7390cc5a72420a5661cd580eedf08808d9271a305bdc32e00841fb2f44c5d9'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.0/buildx-v0.9.0.linux-arm-v7'; 			sha256='35d7ee9bb8ddee9715c27ad5fa1512d56dd3b3c6a13137699643d07a932eb08b'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.0/buildx-v0.9.0.linux-arm64'; 			sha256='c288ee151a30eb6afe68937600c96eb4b6e1932c9ef46584304438b85756cea6'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.0/buildx-v0.9.0.linux-ppc64le'; 			sha256='4a324d4ae294526c9e5f3c6544a9c95009537eb38530e3fbb0940dd3f9b8d6d6'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.0/buildx-v0.9.0.linux-riscv64'; 			sha256='794fdce2c09178dae2c7dafae75aa5c0d888e95164f419820b05e0674675b65d'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.0/buildx-v0.9.0.linux-s390x'; 			sha256='81d7d84d05a6e24677d22cd812a5ba1cbfb15e44ccba652f4dfa5e3076bb58ce'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 17 Aug 2022 01:38:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.9.0
# Wed, 17 Aug 2022 01:38:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-x86_64'; 			sha256='3be9ce88ecba41b734e3fc8e59a9b11531133761414a78827d1615aadb5ef1f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-armv6'; 			sha256='2ea0f36350f81ae66db2b8c12104de6ed974a328557a4967857ee6e8df4b8f26'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-armv7'; 			sha256='658db542e40c8063cdafc23f650493bedc10b41b6d6fb581b7866bfeb5ffb0ba'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-aarch64'; 			sha256='6d227b060b2bc3dc5f315a07ae4f647f042755691e2da905b1a21e60a8ae3ddf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-ppc64le'; 			sha256='101ea490283f3c862e9bb4e7ef2a3fb38393cf2139f2b78e7a7423c91ad0c1fa'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-s390x'; 			sha256='0826c101e1d1a070e8ab8d7649c0da3cb9e6ecf1e717c545188243be6e676d00'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 17 Aug 2022 01:38:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 17 Aug 2022 01:38:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 17 Aug 2022 01:38:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 17 Aug 2022 01:38:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 17 Aug 2022 01:38:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 01:38:42 GMT
CMD ["sh"]
# Wed, 17 Aug 2022 01:38:48 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 17 Aug 2022 01:38:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 17 Aug 2022 01:38:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 17 Aug 2022 01:38:54 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 17 Aug 2022 01:38:55 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 17 Aug 2022 01:38:55 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 17 Aug 2022 01:38:55 GMT
VOLUME [/var/lib/docker]
# Wed, 17 Aug 2022 01:38:55 GMT
EXPOSE 2375 2376
# Wed, 17 Aug 2022 01:38:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 17 Aug 2022 01:38:55 GMT
CMD []
# Wed, 17 Aug 2022 01:38:59 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 17 Aug 2022 01:39:00 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 17 Aug 2022 01:39:00 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 17 Aug 2022 01:39:02 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 17 Aug 2022 01:39:03 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 17 Aug 2022 01:39:03 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 17 Aug 2022 01:39:03 GMT
USER rootless
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb510456a427665c9755e7417ad432e68b6e95a1a9a6665f72f0adc6f9ec59d`  
		Last Modified: Tue, 09 Aug 2022 18:22:44 GMT  
		Size: 2.0 MB (2036045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4627ba0696d0614a94c97a4b5c212e055112e2a8f0831f342f3b138955035153`  
		Last Modified: Tue, 09 Aug 2022 18:22:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e001120e1cd4a7ea1ec2535b3ff388987a6bf3f3bd1568ba33de8157170276df`  
		Last Modified: Tue, 09 Aug 2022 18:24:12 GMT  
		Size: 13.7 MB (13668392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7891c9ff9fe8458ea343f34104986d179b5b2e3403234615c9b3cae8c646a694`  
		Last Modified: Wed, 17 Aug 2022 01:41:17 GMT  
		Size: 15.2 MB (15203446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144f1ebec263f782d6b9c68989ab35e8271419a535c01c673284747e0b8ebc8a`  
		Last Modified: Wed, 17 Aug 2022 01:41:16 GMT  
		Size: 9.4 MB (9385853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0385f958775b1ad6a100569fb631fbba5ee6e8cede7666850e4ff7a12c0501`  
		Last Modified: Wed, 17 Aug 2022 01:41:15 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30c5557bfe39bc1ba6fcd09f3f749cb7090cf9f9ff3eec7fbfad2800a7d7d0b`  
		Last Modified: Wed, 17 Aug 2022 01:41:15 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3b23cdd1545654650c86bb637e852e273ffe5919d6966281f90ce1424910c3`  
		Last Modified: Wed, 17 Aug 2022 01:41:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb14534f8459d4c14a25bdaa914629f58a7bb1364b85d81e07ff6687740b03`  
		Last Modified: Wed, 17 Aug 2022 01:41:48 GMT  
		Size: 6.9 MB (6863588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2317829903f14a69887281331a713e703e136483ddc89ed0aabc921f7948da86`  
		Last Modified: Wed, 17 Aug 2022 01:41:47 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb16b423fd52b901237c66e4fd99b86bbbc91de848a2323f33e41e6b35a7f80`  
		Last Modified: Wed, 17 Aug 2022 01:41:56 GMT  
		Size: 51.8 MB (51847180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df88fbdd82d3d96b434782440df393b887863ba3132f46376c66a1072fe76b9`  
		Last Modified: Wed, 17 Aug 2022 01:41:47 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a813a67ee7ee240c1bccee6d290554e427b3e6b1599aee944f6de61b2dfd1912`  
		Last Modified: Wed, 17 Aug 2022 01:41:47 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ecb23e84aa1bc5d6b495eb93acd1b3bd5d337647c0838842701d401228d927`  
		Last Modified: Wed, 17 Aug 2022 01:42:16 GMT  
		Size: 1.4 MB (1358638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013ddf4dd7d409f13ffa8a1d28d58008804253f5378b84717ddc3bda51436f71`  
		Last Modified: Wed, 17 Aug 2022 01:42:15 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57423722946053ff690012087ca137b3473846df0bb0b39c84bc3f26cdfe9764`  
		Last Modified: Wed, 17 Aug 2022 01:42:16 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c204f6154d03cd2676c58437672e628265fcb38c2d493502c59bda167829344`  
		Last Modified: Wed, 17 Aug 2022 01:42:18 GMT  
		Size: 19.3 MB (19346889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb70f82e41caf687e8466555bd17d9c5d6745305c7f2c835f9f493da54545de`  
		Last Modified: Wed, 17 Aug 2022 01:42:16 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4310d2a874923d8e3bb3b478e4f76a1e60f55e8410d7e971788f42cc2a5d61ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115731508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69e98f852ba5d83779facbaacc1112b96ba96d51d9b77abb1c86d4d30062123`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:24:48 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 09 Aug 2022 18:24:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:25:59 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 09 Aug 2022 18:26:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Tue, 09 Aug 2022 18:26:07 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 09 Aug 2022 18:26:09 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Tue, 09 Aug 2022 18:26:10 GMT
ENV DOCKER_COMPOSE_VERSION=2.9.0
# Tue, 09 Aug 2022 18:26:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-x86_64'; 			sha256='3be9ce88ecba41b734e3fc8e59a9b11531133761414a78827d1615aadb5ef1f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-armv6'; 			sha256='2ea0f36350f81ae66db2b8c12104de6ed974a328557a4967857ee6e8df4b8f26'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-armv7'; 			sha256='658db542e40c8063cdafc23f650493bedc10b41b6d6fb581b7866bfeb5ffb0ba'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-aarch64'; 			sha256='6d227b060b2bc3dc5f315a07ae4f647f042755691e2da905b1a21e60a8ae3ddf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-ppc64le'; 			sha256='101ea490283f3c862e9bb4e7ef2a3fb38393cf2139f2b78e7a7423c91ad0c1fa'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-s390x'; 			sha256='0826c101e1d1a070e8ab8d7649c0da3cb9e6ecf1e717c545188243be6e676d00'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 09 Aug 2022 18:26:14 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 09 Aug 2022 18:26:15 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 09 Aug 2022 18:26:15 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 09 Aug 2022 18:26:16 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 09 Aug 2022 18:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 18:26:18 GMT
CMD ["sh"]
# Tue, 09 Aug 2022 18:26:29 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 09 Aug 2022 18:26:30 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 09 Aug 2022 18:26:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Tue, 09 Aug 2022 18:26:37 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 09 Aug 2022 18:26:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 09 Aug 2022 18:26:40 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 09 Aug 2022 18:26:40 GMT
VOLUME [/var/lib/docker]
# Tue, 09 Aug 2022 18:26:41 GMT
EXPOSE 2375 2376
# Tue, 09 Aug 2022 18:26:42 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 09 Aug 2022 18:26:43 GMT
CMD []
# Tue, 09 Aug 2022 18:26:50 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Tue, 09 Aug 2022 18:26:51 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 09 Aug 2022 18:26:52 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 09 Aug 2022 18:26:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Tue, 09 Aug 2022 18:26:55 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 09 Aug 2022 18:26:56 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 09 Aug 2022 18:26:57 GMT
USER rootless
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abd6445c68b28c4fea9c5ead64de6d84bfbcf44d2ea150df466f2efe4ca7ac8`  
		Last Modified: Tue, 09 Aug 2022 18:28:29 GMT  
		Size: 2.0 MB (2010519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6c1cdde4920e39b02e2eaa9a348dd527a363263a4901b3efdf13020d24a917`  
		Last Modified: Tue, 09 Aug 2022 18:28:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596c126c4e7f951be440ca6dc23043be252de5144fad72341963255f4d1f60e1`  
		Last Modified: Tue, 09 Aug 2022 18:30:10 GMT  
		Size: 12.5 MB (12500816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cba93283e3a98d5d1fe19309fb4791774d032e44e820f3ff390f3c736ff66a`  
		Last Modified: Tue, 09 Aug 2022 18:30:10 GMT  
		Size: 13.1 MB (13097909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71968dd9063c7aa84eeadd4d6274b40fe000199f3c1802570b6bb1e2d2873d4b`  
		Last Modified: Tue, 09 Aug 2022 18:30:07 GMT  
		Size: 8.6 MB (8598397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afefa9112a5cf9f5c6b34925fa318c5a97be6f45502af846ec11da1508b9318`  
		Last Modified: Tue, 09 Aug 2022 18:30:06 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06c0831901266efad466d761ee164cc66bac89b6602a80a2418ab252b8f9da7`  
		Last Modified: Tue, 09 Aug 2022 18:30:05 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3e76e75bf71bca2dcac7f6242c22b88eb138c0a744d24903479f4e7cb78a48`  
		Last Modified: Tue, 09 Aug 2022 18:30:05 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd02cfeba59d27a10fedd47aa0833fcc8ca6fb08ea2c56c78728301dfb524ac9`  
		Last Modified: Tue, 09 Aug 2022 18:30:49 GMT  
		Size: 6.7 MB (6736484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6c7d1c8364f471027477d0b10eae7c880e66f8d6ad9fb335627cb5613df242`  
		Last Modified: Tue, 09 Aug 2022 18:30:47 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab340c9f97d3e20bb645657ee3bb53fbbd89e61829e7ad183cda77ec36cdc8c`  
		Last Modified: Tue, 09 Aug 2022 18:30:55 GMT  
		Size: 47.5 MB (47523637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b091b60945cf27631784246d5793a9f06b7df5508852e5dc159b190842929b`  
		Last Modified: Tue, 09 Aug 2022 18:30:47 GMT  
		Size: 955.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cf36c96641e69944223e6585a7e840b875459fb4b062df199a420d75482916`  
		Last Modified: Tue, 09 Aug 2022 18:30:47 GMT  
		Size: 2.7 KB (2743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7201e70e7ebc93187fe8dce1ff3d76f9e083cad47dc0b1fad61265f0434289`  
		Last Modified: Tue, 09 Aug 2022 18:31:19 GMT  
		Size: 1.4 MB (1370587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5012ddbc8ae1b20e93bb6b5fdd76beebaf279c6dce214880d8620534fcd31393`  
		Last Modified: Tue, 09 Aug 2022 18:31:18 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87c9845748870b28865b3612017c5638f4f994e2dbf5431cc9c5e0e932ec8d1`  
		Last Modified: Tue, 09 Aug 2022 18:31:19 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9633fd520042de7251792fc96145e33895cc044a8312708e8b72e179809b7e`  
		Last Modified: Tue, 09 Aug 2022 18:31:22 GMT  
		Size: 21.2 MB (21177046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a21891157a6c9f711342d021dc5302342f5968ed4bc6d89a45b85cd5240f3c4`  
		Last Modified: Tue, 09 Aug 2022 18:31:18 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
