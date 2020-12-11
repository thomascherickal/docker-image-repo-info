## `docker:dind-rootless`

```console
$ docker pull docker@sha256:53e4c1ec262c4a6e14ce863b72b23aa21c33c1c2a5b9d9417989096c80260f8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:6921c855c141f3c87dd9736b3783aaead17b83c564a1afae678afe546c555f82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101524776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd272bd50bff353249e99ef1c016e4465c8cd75b28f749659b6ca4af12b81d5`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:29:33 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Fri, 11 Dec 2020 05:29:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 05:29:34 GMT
ENV DOCKER_VERSION=20.10.0
# Fri, 11 Dec 2020 05:29:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 11 Dec 2020 05:29:41 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:41 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 11 Dec 2020 05:29:42 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 11 Dec 2020 05:29:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:42 GMT
CMD ["sh"]
# Fri, 11 Dec 2020 05:29:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 11 Dec 2020 05:29:50 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:29:50 GMT
ENV DIND_COMMIT=ed89041433a031cafc0a0f19cfe573c31688d377
# Fri, 11 Dec 2020 05:29:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 11 Dec 2020 05:29:51 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:29:52 GMT
VOLUME [/var/lib/docker]
# Fri, 11 Dec 2020 05:29:52 GMT
EXPOSE 2375 2376
# Fri, 11 Dec 2020 05:29:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 11 Dec 2020 05:29:52 GMT
CMD []
# Fri, 11 Dec 2020 05:30:00 GMT
RUN apk add --no-cache iproute2
# Fri, 11 Dec 2020 05:30:02 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 11 Dec 2020 05:30:03 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 11 Dec 2020 05:30:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.0.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 11 Dec 2020 05:30:09 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 11 Dec 2020 05:30:10 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 11 Dec 2020 05:30:10 GMT
USER rootless
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db28d0fdbf69ee580b35224bf77ef5e71f9a061c0aafab87064af9708035d9d`  
		Last Modified: Fri, 11 Dec 2020 05:31:33 GMT  
		Size: 2.0 MB (2039048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292df0bc6bf3350f306af7623bc14f00386239bb27303d3047104b9cfdb55460`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e060f4bd70b333ccaa7ae441b42f1068621b39bbe8eb9c71b5a4e06d10b4ff3`  
		Last Modified: Fri, 11 Dec 2020 05:31:46 GMT  
		Size: 69.5 MB (69457871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8d568a22304aafab5a456040525abd0b705efad0b6e60e64847ebe1c6e4e6`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc6ef1a942a0f6b2ab0993eecb7ce30d31f06af50a2ae40893e1a160c9a0892`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2312dd95470aa8eaccef80bbca7892390ca777559b50fab574e65147a35107fc`  
		Last Modified: Fri, 11 Dec 2020 05:31:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705044911461d972356a560402ae7212ac5b9e0cf5650c9e90e82c0168e363f4`  
		Last Modified: Fri, 11 Dec 2020 05:31:55 GMT  
		Size: 6.0 MB (5958710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca03bf2650888a6dd094e66dc51a4c7e9cf6e2d540eb0e6ee60447b670644cb`  
		Last Modified: Fri, 11 Dec 2020 05:31:54 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f30abe54315eba4800bca902658bb857afd12015cb658e13874c43042c93400`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc682ce81f04b09d573611856b1c36f71a3da08529300ee33214d7d31432df2b`  
		Last Modified: Fri, 11 Dec 2020 05:31:53 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3bb12715694c8d4d06340e7dee1e3254c8e3b7b70a93186d608231e3d078e2`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 1.1 MB (1092673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a839f28eb57bd36d3aacb29facc913d8ab0f88f7dc151a1c4ed01678b588b880`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0a6ba5f373ec6316a1554ce6f2b7006f8a1b8125ecd9d2b5a10737eccc0f39`  
		Last Modified: Fri, 11 Dec 2020 05:32:03 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa1dd6e35f0eddbcae4e4ce8274d76308a2b6c591c73a5265567a52e237f12e`  
		Last Modified: Fri, 11 Dec 2020 05:32:07 GMT  
		Size: 20.2 MB (20171373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348a90887c16fa0075d15a6c8c9a7c23ba9733360f2e894b4274351566a1e557`  
		Last Modified: Fri, 11 Dec 2020 05:32:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
