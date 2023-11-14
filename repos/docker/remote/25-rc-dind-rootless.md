## `docker:25-rc-dind-rootless`

```console
$ docker pull docker@sha256:74aa6e0ea6b8bf4efaf8854d00d672f62d162054b5cacc1242af9ea87fb4a1bd
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:25-rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:e7dc4c02227d2d68ea1058109f16d3b21d7f8826c33db8839bc94d8b4f3313f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144891645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b3901aefb0b5e02fde282ca164d60cba90d838f1d1928ef0b73f08a1191dc96`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
USER rootless
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29d9fec024e0920642ec37a18cfe9b17faf4cbbb812053dec79277c01c278f37`  
		Last Modified: Tue, 14 Nov 2023 02:34:39 GMT  
		Size: 2.0 MB (2014281 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e22e15fb52072ccbeacf286794af3749a096b16f210e3bb9c7dd7156bbe3bd1e`  
		Last Modified: Tue, 14 Nov 2023 02:34:39 GMT  
		Size: 16.9 MB (16890685 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e1fcdb75a84600567650d3383949fa8761c6179151b55f351c5b0f597349d2`  
		Last Modified: Tue, 14 Nov 2023 02:34:39 GMT  
		Size: 17.5 MB (17459267 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1236562b8aaad6dda90fad764df4bb61098cbd79164ff48b1c1e2e90ac9a3190`  
		Last Modified: Tue, 14 Nov 2023 02:34:39 GMT  
		Size: 17.8 MB (17831740 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b6212aa982261ecf4b2efd28f9b911d57a38ca8c0ff41dc6c4aa34679e777b5`  
		Last Modified: Tue, 14 Nov 2023 02:34:40 GMT  
		Size: 542.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de5f70bc4b8fa677a04e94190e34fd8f2478f9bcae8f1116baf276f76d5e1bdf`  
		Last Modified: Tue, 14 Nov 2023 02:34:40 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df21d3045d0dca661a16bfdb67d2cbf61528abe36a18f65d799a65109c65c7ca`  
		Last Modified: Tue, 14 Nov 2023 02:34:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f17da22f0d6c1ec8c712931525e12f9c1ca39f0f7d209ed56b630c274564787`  
		Last Modified: Tue, 14 Nov 2023 03:23:50 GMT  
		Size: 9.3 MB (9274457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b645527094b4e37aea39df452e603cc01403fd99cac5724da0699c5efbd4caa`  
		Last Modified: Tue, 14 Nov 2023 03:23:49 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48b1911d82a23210569d479c4b1ab7e8b9d1b681f02c9bea258a7cfe6003a65d`  
		Last Modified: Tue, 14 Nov 2023 03:23:51 GMT  
		Size: 55.8 MB (55764176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa79fdb91133401212a0a4e50119b6eac9e905fa5c49527689b21f72ea7ea75c`  
		Last Modified: Tue, 14 Nov 2023 03:23:50 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f822926803484ce3a23a48e2dab7ef2a12176445288691193add7b68b5f9a66`  
		Last Modified: Tue, 14 Nov 2023 03:23:50 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89c0e25e7ecc7b8b47a6c62d087e8b6729dfa541dd385b524686aec0f1c4affa`  
		Last Modified: Tue, 14 Nov 2023 04:16:15 GMT  
		Size: 1.4 MB (1362175 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef220f2a242e6ed3e75033f3bf885d5911d08d969825a85ce79a60b89d9212d2`  
		Last Modified: Tue, 14 Nov 2023 04:16:15 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3876ea659caced97be589f64256395cc973a50a065b10c4d88c5cbad3ae76902`  
		Last Modified: Tue, 14 Nov 2023 04:16:15 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3524b8c9159ded1ebe0e5021b23886bc972a4feb6515e3f8ce9ab8c65191b281`  
		Last Modified: Tue, 14 Nov 2023 04:16:16 GMT  
		Size: 20.9 MB (20884439 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f81efe2d1fe8cce50ab831b8b4c93a26ab90c36243e6748d8481d6d0dc2203d`  
		Last Modified: Tue, 14 Nov 2023 04:16:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:25-rc-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:f9a6d74cc58ef4f1c27f1cf62eba621e1381cae98d0ae641b386dc73e42c5a82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **753.6 KB (753609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b428b09e19ddde93886a3eb9bb6a7b592de8652288ac52ba8faad91ff5b5ee5`

```dockerfile
```

-	Layers:
	-	`sha256:deab1b6410debe803de67fdd46fd184d5acbdd3776181e448da7820cf4d6cd6f`  
		Last Modified: Tue, 14 Nov 2023 04:16:15 GMT  
		Size: 722.8 KB (722752 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9e993dba09616b508f8c22be18c5900b35fef91c33e595234c8441add9f29553`  
		Last Modified: Tue, 14 Nov 2023 04:16:15 GMT  
		Size: 30.9 KB (30857 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:25-rc-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:bccd7663c87a441a5df51988198a8d3efad1dcc37d062e0df1f212c1bbeddc7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138227946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49d48ce95283af26dd7ccb64f58f8ffd69ce36bfe6a31fedc0940a545ba292e7`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-x86_64'; 			sha256='6e06123399e5428fbd603564afdac74821fa0a7b4465e8a1a2359b362fc42fc4'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv6'; 			sha256='75889ad81c5b0b07805920e398eaa7fb41c1321c81942daa07a5b5c5a1a27bdb'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-armv7'; 			sha256='2cd4af627462720384cfd2ba24d951854707d7c1fa37618c9e0319139f8a2012'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-aarch64'; 			sha256='5c09e2c6b1cd9fc1be535690ee62712687ad12f0d08b14c27d30442f0e85b955'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-ppc64le'; 			sha256='ff524f6d11050483abda01c5b1b33626c6c2f1b835df8514db6a42148d5095fc'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-riscv64'; 			sha256='00302be14ad7d981eb86b834c09deb8186231b416c16454f9971bfcc0ec7e22f'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-linux-s390x'; 			sha256='323c2e92b3150ef94dc4201770e06ed7bacbe811abd77a23108cceea032fcf63'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
USER rootless
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
	-	`sha256:b751039a3d1e1f4c5da518d2c0ab210d9dde6bb4b882239669c537ca0cca4750`  
		Last Modified: Tue, 14 Nov 2023 02:44:03 GMT  
		Size: 15.9 MB (15893478 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3b663e15ed23f8d36fa0c7d779d617215ef3e3e2380ff3cfaea5e0924389766`  
		Last Modified: Tue, 14 Nov 2023 02:44:03 GMT  
		Size: 15.8 MB (15768057 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ce63029d26a78f18e74b1c2f75561405ca543644120b5a970c1a7c268ad1283`  
		Last Modified: Tue, 14 Nov 2023 02:44:03 GMT  
		Size: 16.3 MB (16290393 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a633ba00be8d31065fe4dc80c98163b8349efb20baae2f0cc6c7a36502f7544`  
		Last Modified: Tue, 14 Nov 2023 02:44:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d2c38a8de1e8d754fbd7176498e2d5b7f368c9d98b8ed402b0ab05f5134c182`  
		Last Modified: Tue, 14 Nov 2023 02:44:03 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbdf299ef56c4eb2f5fe65bfe4d96a64ba78afdac32f0e954e464c88fa0d0a61`  
		Last Modified: Tue, 14 Nov 2023 02:44:04 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37b9c763e9253b1ad1f92ebcec18c2fab25069dd178ecc3653db9965ed951c43`  
		Last Modified: Tue, 14 Nov 2023 03:30:33 GMT  
		Size: 9.4 MB (9362895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d54f121c9b844437de6ca15f39b2d2c052403d5799862183b11aed89e1ab907`  
		Last Modified: Tue, 14 Nov 2023 03:30:33 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e35743148a48f9ec4d60db179456a8a08c135e65795d2319d4bd9e148ecc768f`  
		Last Modified: Tue, 14 Nov 2023 03:30:35 GMT  
		Size: 51.4 MB (51388580 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e913c48647e4a8705489a75dbca256e7c04e992e208030627ceca0327c5b2a72`  
		Last Modified: Tue, 14 Nov 2023 03:30:33 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0dc1e715fe3a30110d77402f22e7ceea8b8a78b64364ab6172742454aa13d9b4`  
		Last Modified: Tue, 14 Nov 2023 03:30:35 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f6d93a41821afa7ad5cf341ae90c4e951844f108640162b968b257067d64cd0b`  
		Last Modified: Tue, 14 Nov 2023 04:25:35 GMT  
		Size: 1.4 MB (1413167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:303da4d381a8514d93750ec8655812f8224f08a9696941ed7aa75f5adc98ef13`  
		Last Modified: Tue, 14 Nov 2023 04:25:34 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53a528836f64b486c9f32beba44e207017b55f1bdf29def80ac5f6696da8fb1`  
		Last Modified: Tue, 14 Nov 2023 04:25:34 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65160afc9aabd599f00e3a7e9b7d360add9b53acce995c1a162a6d64d5d2b32e`  
		Last Modified: Tue, 14 Nov 2023 04:25:36 GMT  
		Size: 22.7 MB (22746533 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:784b17c9d655c7d156f21134ccb3c302a2f8ab1895883ec7d38938dcc57d2cee`  
		Last Modified: Tue, 14 Nov 2023 04:25:35 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:25-rc-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:20414b13dc8558671653dca3befa8fbc3804534ac61a3722b2ad96f780adf5b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **753.7 KB (753674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef95cac8f7bffb74d7e0194733dfed916f4cd6feef2f13c1edda5edb5fbb410`

```dockerfile
```

-	Layers:
	-	`sha256:8e66aecfb09acdc3378b9c398e9f65b9b4fc98ab5a96effd8692967585e9f65d`  
		Last Modified: Tue, 14 Nov 2023 04:25:34 GMT  
		Size: 722.8 KB (722761 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0519dac2f0e6abdb9b066fa2f2a1a7bbc89ebf8d48fb1216e016cb05193e640c`  
		Last Modified: Tue, 14 Nov 2023 04:25:33 GMT  
		Size: 30.9 KB (30913 bytes)  
		MIME: application/vnd.in-toto+json
