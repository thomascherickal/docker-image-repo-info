## `docker:latest`

```console
$ docker pull docker@sha256:9f4eaac084da13e1825fd469a35ed015dc6f8c18d160af6fe7bf1326f24823d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:d674ad290a5be730b751f017f5a1f012adf51b74f7d33091bfef1e66a44047ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43101659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff98ea2b23972cc7b326340e87bd37ee046188f98737e43f547eef1706fc4751`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:205d2ba86ebbaa570c80082297b768b1a711372c47e40690b861eacff75d251a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 MB (38917139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:948ae3ff2c93e94b7fdb7186f74545ca766731f6429923cfc7a79e43fea0547c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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
