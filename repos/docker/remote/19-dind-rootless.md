## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:320f5a070df42168eb218c0e383ed83c52266d71fc5bba64b4e95fa4b05115b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:cd286a187d9dac72c6d9a085cfb9bf16b8504124c3852a974e7a595010a8fb79
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94877382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55073a55c2edafcdac3145714f508c3b5c38020e0e4af848ac155147b8044c7e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:16:58 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 14 Apr 2021 20:16:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:17:37 GMT
ENV DOCKER_VERSION=19.03.15
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-19.03.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-19.03.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-19.03.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 14 Apr 2021 20:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 14 Apr 2021 20:17:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 14 Apr 2021 20:17:46 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 14 Apr 2021 20:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:46 GMT
CMD ["sh"]
# Wed, 14 Apr 2021 20:17:52 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 14 Apr 2021 20:17:53 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 14 Apr 2021 20:17:53 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Wed, 14 Apr 2021 20:17:54 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 14 Apr 2021 20:17:55 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:17:55 GMT
VOLUME [/var/lib/docker]
# Wed, 14 Apr 2021 20:17:55 GMT
EXPOSE 2375 2376
# Wed, 14 Apr 2021 20:17:55 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 14 Apr 2021 20:17:55 GMT
CMD []
# Wed, 14 Apr 2021 20:18:00 GMT
RUN apk add --no-cache iproute2
# Wed, 14 Apr 2021 20:18:01 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 14 Apr 2021 20:18:02 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 14 Apr 2021 20:18:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-19.03.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 14 Apr 2021 20:18:06 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 14 Apr 2021 20:18:06 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 14 Apr 2021 20:18:06 GMT
USER rootless
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a38b3726f4b24fa93b80450be63ad67fd3239c2f3b83695118d7b1a88447d84`  
		Last Modified: Wed, 14 Apr 2021 20:18:49 GMT  
		Size: 2.1 MB (2050156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fa5deb334027202841b051d10e7c7137fa3b63e97734309cedf6b48804df5f`  
		Last Modified: Wed, 14 Apr 2021 20:18:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09182082685c0a1147c9f22948720af9bb3544411a1b50562d18071cf31b8e21`  
		Last Modified: Wed, 14 Apr 2021 20:20:33 GMT  
		Size: 62.9 MB (62882940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562e3055ed2549b93e450d764e41b62a485d16bafb1f1ed6b67fd610444aa44`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4de57a4336a3a0ab0e109ff4c769bce1d354c121fe62fd5f6063c53fd009d61`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542e5df0dc5eda03440d4a00ca01ceefa7cb8282a9d7b406fd54dabcdf4197c0`  
		Last Modified: Wed, 14 Apr 2021 20:20:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8586280a334732de42259c879b0c7d8a9a16bfcb8764f797a9cdd720aac766bf`  
		Last Modified: Wed, 14 Apr 2021 20:20:50 GMT  
		Size: 6.6 MB (6569726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8926df9acf368d91f3a21b4465c45354ea1b091727a6297d78629f0e963576ca`  
		Last Modified: Wed, 14 Apr 2021 20:20:49 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e915ef07afac6a26ee62e4ef7ac115461ba80a6be5450982cccaacae041adbb9`  
		Last Modified: Wed, 14 Apr 2021 20:20:49 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d284661b3d49b778a5dd8f40c9c34e25a983a44b304f035451f58a5354c2a8a0`  
		Last Modified: Wed, 14 Apr 2021 20:20:49 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdee2f5aa804bab47c0a1a82ef6e334322c0b3b11596a8da470471a82502599`  
		Last Modified: Wed, 14 Apr 2021 20:21:04 GMT  
		Size: 1.1 MB (1131578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88a89490c27104db5148fcc04529f666a12f76880f8cad73a947d893ceaf9b5`  
		Last Modified: Wed, 14 Apr 2021 20:21:04 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34e502f8004a84efb3f908dbfdb9e9f9b1b28e33367b582fcfcfdd620dd07db`  
		Last Modified: Wed, 14 Apr 2021 20:21:04 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa95f47ecb99f69121d90b605c2cb85a4c695bbf05878a34ef2fb4086716808`  
		Last Modified: Wed, 14 Apr 2021 20:21:08 GMT  
		Size: 19.4 MB (19422691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9bffba89ff6d560f0723305d725e24c6f85d1788e9b25d2f53a97e51a69023`  
		Last Modified: Wed, 14 Apr 2021 20:21:04 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
