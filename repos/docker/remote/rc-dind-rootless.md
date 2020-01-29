## `docker:rc-dind-rootless`

```console
$ docker pull docker@sha256:f066ad6c74a4c14595f66f14589a70da93d5f76c02c15752f6c9ae195b5b0c0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:3528a31cd28a813dc89e8180903f82b10170239a14bf14a08b9c03ce43b700a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94645373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7910b59ec98e75afa6b8c9f24f47fb741ac9383f43ee11e7ccdf790a0e2c01d9`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:18:34 GMT
RUN apk add --no-cache 		ca-certificates
# Mon, 21 Oct 2019 18:18:35 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 30 Oct 2019 23:25:35 GMT
ENV DOCKER_CHANNEL=test
# Tue, 12 Nov 2019 00:25:25 GMT
ENV DOCKER_VERSION=19.03.5-rc1
# Tue, 12 Nov 2019 00:25:30 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 12 Nov 2019 00:25:30 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:30 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Nov 2019 00:25:31 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 12 Nov 2019 00:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:31 GMT
CMD ["sh"]
# Tue, 12 Nov 2019 00:25:36 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 12 Nov 2019 00:25:37 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:25:37 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Tue, 12 Nov 2019 00:25:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 12 Nov 2019 00:25:38 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Tue, 12 Nov 2019 00:25:38 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Nov 2019 00:25:39 GMT
EXPOSE 2375 2376
# Tue, 12 Nov 2019 00:25:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Nov 2019 00:25:39 GMT
CMD []
# Tue, 12 Nov 2019 00:25:44 GMT
RUN apk add --no-cache iproute2
# Tue, 12 Nov 2019 00:25:44 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Tue, 12 Nov 2019 00:25:45 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Tue, 12 Nov 2019 00:25:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Tue, 12 Nov 2019 00:25:47 GMT
ENV ROOTLESSKIT_VERSION=0.6.0
# Tue, 12 Nov 2019 00:25:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Tue, 12 Nov 2019 00:25:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Tue, 12 Nov 2019 00:25:59 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 12 Nov 2019 00:25:59 GMT
USER rootless
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef94372a977c02d425f12c8cbda5416e372b7a869a6c2b20342c589dba3eae5`  
		Last Modified: Mon, 21 Oct 2019 18:20:06 GMT  
		Size: 301.7 KB (301722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec62c064901392a6722bb47a377c01a381f4482b1ce094b6d28682b6b6279fd`  
		Last Modified: Mon, 21 Oct 2019 18:20:05 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d00f109003f5dd9e123c11faa3270ff5790e2e94cc062ac33acd54317e15e5`  
		Last Modified: Tue, 12 Nov 2019 00:26:53 GMT  
		Size: 63.8 MB (63804789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c3bf8eedaf11dca42c6bdd3160a31267b056f30138e9a83ae6291d7a50d712`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea408e741e559862add2ec71bc27aa6e6a9d6cc900bb7ff5399a3f221c850f4`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d3ea9ec8d1db322186cdbecdc3bffb283e8b87e2f59adfa5ed06c40e9f5f40`  
		Last Modified: Tue, 12 Nov 2019 00:26:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8c4e1a890d6df2310dec90af1a5d6cb0889567e89206389d1873470591a8eb`  
		Last Modified: Tue, 12 Nov 2019 00:27:01 GMT  
		Size: 5.5 MB (5493300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b345be14caeab88468bbf27dc41c5b8751fdfce83312288386288d471f9ec8d0`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e22df429876fd6d189c1fa3bc8f82b66195923ec8881a14f78df16682a59df2`  
		Last Modified: Tue, 12 Nov 2019 00:27:00 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915977ae9ff10b427ff17d4c9152d37ee3575c87d72b5da2b7c68cd0b9556f84`  
		Last Modified: Tue, 12 Nov 2019 00:26:59 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32795880a521eae7582c0270f900fcac318a148e278f3c5f2056dbecb566c6ae`  
		Last Modified: Tue, 12 Nov 2019 00:27:08 GMT  
		Size: 722.6 KB (722572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c19ee2832c7580babdc0b08bef1837a9639bf2b7efb302d9f800fd400a53c5`  
		Last Modified: Tue, 12 Nov 2019 00:27:06 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5d7916f8600113e56597d04afd6d8d01dfa266fbc832988789b17a50764f97`  
		Last Modified: Tue, 12 Nov 2019 00:27:06 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a06f686027b0f516409ec930965e0510b34ea75f88542df6762cbc226bead62`  
		Last Modified: Tue, 12 Nov 2019 00:27:09 GMT  
		Size: 9.1 MB (9109464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60c15bf7903b46f98edc01a329c0de68aedd24774de6fcb278c1897cd6aa1bb`  
		Last Modified: Tue, 12 Nov 2019 00:27:08 GMT  
		Size: 12.4 MB (12418316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542afa5f61c8214b17bf510810c9d3147ea3de49c53bfb4adc049a62bfc9e7ae`  
		Last Modified: Tue, 12 Nov 2019 00:27:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
