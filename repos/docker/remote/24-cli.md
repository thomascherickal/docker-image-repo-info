## `docker:24-cli`

```console
$ docker pull docker@sha256:43651800218f833f6d09f586df8b174866a31b38e905ef1721658243cbe460a5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-cli` - linux; amd64

```console
$ docker pull docker@sha256:056961119258dfaf178a12d087d54a07c14b558a1ec1c9104307fd5771e6ca3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57109368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57fc335287c39f07bd5d5b891f602495265edb733eaac9baa07fbcddfbf44a1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_VERSION=24.0.7
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Oct 2023 17:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:308a300cc30fe6ac962159008af174ab8d5de056d2a186cf8350b68b8d2040e8`  
		Last Modified: Fri, 27 Oct 2023 16:50:26 GMT  
		Size: 2.0 MB (2014298 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5fcb7611fd7787a35fbc3a6cf88c0a9883e2a800782a9dc2ecb2eee34e49ef05`  
		Last Modified: Fri, 27 Oct 2023 16:50:27 GMT  
		Size: 16.4 MB (16400381 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be9955e691a8bf74f82ae7a0db734885fdffaed064cdbb41be3ee66d68d33b25`  
		Last Modified: Fri, 27 Oct 2023 16:50:26 GMT  
		Size: 17.5 MB (17459265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b5ce73eb848197885a2a4977b7411de12d27698124e6ab5c3fc97bf484b3b98`  
		Last Modified: Fri, 27 Oct 2023 16:50:27 GMT  
		Size: 17.8 MB (17831746 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe45098d8d9ea39921533a83d0e5d37e6eaa7a11adaf825bf848c8b4e1556e16`  
		Last Modified: Fri, 27 Oct 2023 16:50:27 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:843bf259cc12ab466da7e4d67e99719b85179d565d6a3f100d2b1aa23607e75d`  
		Last Modified: Fri, 27 Oct 2023 16:50:28 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e56cd900ceac85789d7e36131cbd954a2c660688b4ee542c8a8df3c4d8ffb7d3`  
		Last Modified: Fri, 27 Oct 2023 16:50:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:e1976850747cd92c05d67d6db5c0333c82833f7c09868d5f29556f84eed4942c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.2 KB (377202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8a3b8b826625fb41ca6675b1f6c315a4b73bea907fbe37769f5158d116dcc0`

```dockerfile
```

-	Layers:
	-	`sha256:d4049c8d767a032751c624be00ca74971daa5b1d470e08d8ac8e6031a58ad5e9`  
		Last Modified: Fri, 27 Oct 2023 16:50:25 GMT  
		Size: 341.4 KB (341419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e0410a640531d7f440114417767b75496a2c81ea760f776d0e050ea7e0dbc338`  
		Last Modified: Fri, 27 Oct 2023 16:50:26 GMT  
		Size: 35.8 KB (35783 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-cli` - linux; arm variant v6

```console
$ docker pull docker@sha256:55a5abbe7306324e2a76470976df3a45dc5976093ac7a575d73a415e583955b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53625683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81666c8e8e46e01e99ce3c6c9c552df0664c99f4dca76deab3d94f0d871ecf3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_VERSION=24.0.7
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Oct 2023 17:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08a082128d131d4e1d89192a607dc228c41b00d2a4fec1453daaaa87ee13a2e`  
		Last Modified: Fri, 27 Oct 2023 16:50:16 GMT  
		Size: 15.1 MB (15132569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a42cba090986318d43481a0718a85667b737c9e0aee85e93f05daf7e4728d4f`  
		Last Modified: Fri, 27 Oct 2023 16:50:15 GMT  
		Size: 16.4 MB (16403194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d2490300ee3104365d359d37010b3d8a7aa1449ea93589f17a69d6b782e54`  
		Last Modified: Fri, 27 Oct 2023 16:50:15 GMT  
		Size: 16.9 MB (16854310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a4bc31d955c487231880def39db0f66c5959d150b1a6aa009274ffea3e4339`  
		Last Modified: Fri, 27 Oct 2023 16:50:12 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048277501c18e45490a5329bf1ab26c0ae0dd2df936d210a05551cd44289cfb7`  
		Last Modified: Fri, 27 Oct 2023 16:50:12 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0240102c3af553e6e963a1ffc7f43e3fcae8ee5d380b9f683ddb688c71e7cfad`  
		Last Modified: Fri, 27 Oct 2023 16:50:12 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-cli` - linux; arm variant v7

```console
$ docker pull docker@sha256:600a568bd73c13ddd6a996f5e447e01500cd747fa5377b5b0fd7334823192999
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53144231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc14b36ae77e4598efb1697642abbcad8911ddd028934cabb6350b43bb99430`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_VERSION=24.0.7
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Oct 2023 17:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:734588fa8ce31adf2dc94210cd8342f969f8b0e95bce00cca1ee11f8caeb8f81`  
		Last Modified: Fri, 27 Oct 2023 16:51:50 GMT  
		Size: 15.1 MB (15127058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d5b0b6c900ceefb2119f1cacc71ce130d0ed27b456a99c360309f65f2bb9dd6c`  
		Last Modified: Fri, 27 Oct 2023 16:51:50 GMT  
		Size: 16.4 MB (16400144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c95702615f0173beb300b96dddeb23ce007acb510cbe23abab742ac7a9ec3b8`  
		Last Modified: Fri, 27 Oct 2023 16:51:51 GMT  
		Size: 16.8 MB (16840165 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15ccb4036ca5e4eda7e051aad9ba2e340ce79e2cdd0501162dacacb7b7c72fdf`  
		Last Modified: Fri, 27 Oct 2023 16:51:49 GMT  
		Size: 542.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4c7ed22c25a5d659ebe3a98817f499ff9e5d1a9cfc680500b77a30b48929c95`  
		Last Modified: Fri, 27 Oct 2023 16:51:50 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab27a746e695695fdfb27f7c0efa764b5690dc3d45a712abf5c612ca9f5d10d0`  
		Last Modified: Fri, 27 Oct 2023 16:51:52 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:762ace034e76be0fa9a715657bbab06a18f7a7747c66d727832acf6a23c22200
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.2 KB (377223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e63cac1d0c6ecd0e40ed513e364e298438fb0e19853746296a4326ab0aa0d9`

```dockerfile
```

-	Layers:
	-	`sha256:b55ec3622aac6f5193c1806b97ed2e7bab5a9f910f82a4957be4577f10f588ad`  
		Last Modified: Fri, 27 Oct 2023 16:51:49 GMT  
		Size: 341.5 KB (341463 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e0b41917143387797cddebba7690cbad287869aa650147d4fe1d2cc066368272`  
		Last Modified: Fri, 27 Oct 2023 16:51:49 GMT  
		Size: 35.8 KB (35760 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0d5c1933367778444b22cf290f9834eb34626174f850aa5980121f02cb6a28bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52866086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d738e15591b4efed0861fd699c17c542f8c4bf644a1adfc8ee7dc563b612046f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_VERSION=24.0.7
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Oct 2023 17:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99624a4fd86a4c6eda9530ba81d64e854494d3513e2b65182d975a3e73659f6a`  
		Last Modified: Fri, 27 Oct 2023 17:27:58 GMT  
		Size: 15.4 MB (15449538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b3f207db0e410e0197c464ca661a747668aa986dba0e886a8e67971f4024bbb`  
		Last Modified: Fri, 27 Oct 2023 17:27:58 GMT  
		Size: 15.8 MB (15768060 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f21744ef4608e0abd369e1d6861c1bef08ab81c70760476571edfed7b8416ab`  
		Last Modified: Fri, 27 Oct 2023 17:27:58 GMT  
		Size: 16.3 MB (16290398 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:80fde8283b9a4c6a0a9c1cb843b622c44b271907de65002792b2251732af0b9f`  
		Last Modified: Fri, 27 Oct 2023 17:27:57 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfd52aaeb832e3a6b316d186878f5f13187c8c16ca40771fa4032629bbcdd54f`  
		Last Modified: Fri, 27 Oct 2023 17:27:58 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2aa7661f3209bca5231163ab4fbd616b34f0d8ba60d79108715250cc8efd8b59`  
		Last Modified: Fri, 27 Oct 2023 17:27:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:25c1003a0af9af87c3f0a6fe6ab97af67fb078e1a4e597ec2682fbde16ff083e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.1 KB (377061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5eaaaa61e2e311939c534c44e7816005da65af66e1e3ee0e6f53da007c4f413`

```dockerfile
```

-	Layers:
	-	`sha256:5dabe7fa6c0c118a4810e014b3dd3c8ebcd6233fc379b61d95d631f4ef3c36e2`  
		Last Modified: Fri, 27 Oct 2023 17:27:57 GMT  
		Size: 341.4 KB (341432 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:497aefacdb045c19c450c404a53d1d968c80f498ea0ecac9ee3622ace5fd8bdb`  
		Last Modified: Fri, 27 Oct 2023 17:27:57 GMT  
		Size: 35.6 KB (35629 bytes)  
		MIME: application/vnd.in-toto+json
