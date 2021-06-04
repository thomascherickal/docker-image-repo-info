## `docker:20-dind`

```console
$ docker pull docker@sha256:89867815852358a38f503287ed126999c6a943845f8b3e6b89f1111f497a9f23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:a5b401c7baadaa320d68336f47eaddc57cd479dbcb41ed65ab5ef89d446a3e36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.7 MB (81726446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0a9f712488ae3b3ddf576e14e56186f709e4735fe042b01f76521878929d535`
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
# Thu, 03 Jun 2021 21:21:16 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:21:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:21:24 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:24 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:21:25 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:21:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:25 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:21:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:21:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:21:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:21:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 03 Jun 2021 21:21:35 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:21:35 GMT
VOLUME [/var/lib/docker]
# Thu, 03 Jun 2021 21:21:35 GMT
EXPOSE 2375 2376
# Thu, 03 Jun 2021 21:21:35 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 03 Jun 2021 21:21:35 GMT
CMD []
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
	-	`sha256:c521bbbd9945cde2415eae95c3a2a604ea5ca18eb86ab5cadeb589d3b8a13185`  
		Last Modified: Thu, 03 Jun 2021 21:22:44 GMT  
		Size: 70.2 MB (70247077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59707d521c45c42bbb7dbbef463d5d3800859f20122fb54894f0c79d9b435483`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abe223b186967eef77715b2c6efd147f3a203a0c7b19e61a8947dab4236397`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d806bc203610fb061281b581a0b2522c9fcbd15e55c55ac0c496c9b1dbe63b0`  
		Last Modified: Thu, 03 Jun 2021 21:22:32 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918595a0e69b201bdd25b6da798216629c61256ba541408487536b3953169aa6`  
		Last Modified: Thu, 03 Jun 2021 21:23:02 GMT  
		Size: 6.6 MB (6610580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf6f33d26f8a966febfc6cfc6677aadddee7d77d37476f660cb4b3e9d4659bd`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0522a0264f7030f681722a192902d53421d886507aac6dafeced99b9ed932a`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 978.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a966a453c72b084cc181ea4e0f49e26372de40579490016120c934d3330bf1`  
		Last Modified: Thu, 03 Jun 2021 21:23:00 GMT  
		Size: 2.5 KB (2511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:cbcb40c35425c6721a769b9161e7d3be512b46e6ada7a51edc85e57330baaf13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75712440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39383be503c3f1f4b1b00c5692be06d7c1e99ff13494f6c511df0b9e6bed2709`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 03 Jun 2021 21:42:21 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Thu, 03 Jun 2021 21:42:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Jun 2021 21:42:22 GMT
ENV DOCKER_VERSION=20.10.7
# Thu, 03 Jun 2021 21:42:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Thu, 03 Jun 2021 21:42:27 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 03 Jun 2021 21:42:27 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:42:27 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 03 Jun 2021 21:42:28 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 03 Jun 2021 21:42:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Jun 2021 21:42:28 GMT
CMD ["sh"]
# Thu, 03 Jun 2021 21:42:37 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 03 Jun 2021 21:42:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 03 Jun 2021 21:42:38 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 03 Jun 2021 21:42:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 03 Jun 2021 21:42:39 GMT
COPY file:ba8ee8770c54e5ecc99314148f702a73a1c00c3ef0cc27ff33581d2dbab7456e in /usr/local/bin/ 
# Thu, 03 Jun 2021 21:42:39 GMT
VOLUME [/var/lib/docker]
# Thu, 03 Jun 2021 21:42:40 GMT
EXPOSE 2375 2376
# Thu, 03 Jun 2021 21:42:40 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 03 Jun 2021 21:42:40 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326020c82d02571ced2efbf10ffbb5899caaabc97f84250d1e60c215ae45f425`  
		Last Modified: Thu, 03 Jun 2021 21:44:11 GMT  
		Size: 2.1 MB (2057871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b09a01aee21bda3de0ce0c740f5d2c404abcb4f8213b0a4de9e5ee65feaae4`  
		Last Modified: Thu, 03 Jun 2021 21:44:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1c38e34fc3e5371c8def96ab8d7e3bba71d32130637597ff4f3e50192087d1`  
		Last Modified: Thu, 03 Jun 2021 21:44:21 GMT  
		Size: 64.4 MB (64423222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eed933d1f7f6c0f3b1ce23d3001c184ee7ec4b38a466faa70184b615092a5d3`  
		Last Modified: Thu, 03 Jun 2021 21:44:08 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a917157686721033d8ff61a07cbce814e3a9c0b1cc11ffdf56352eed2ce0c110`  
		Last Modified: Thu, 03 Jun 2021 21:44:08 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e7b3d5975a25e0edd4d5c4e980484aecadd41615d306543b5fb616e261f534`  
		Last Modified: Thu, 03 Jun 2021 21:44:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4082ded31774b407e7954b123f004e5d4b14cd20a8b7679a7028beaee7a6e8`  
		Last Modified: Thu, 03 Jun 2021 21:44:41 GMT  
		Size: 6.5 MB (6512657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176ace821c1592597cd9c9ee57e184c9cad3e94fcdf12678bc8cc0d7b07be4b`  
		Last Modified: Thu, 03 Jun 2021 21:44:40 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65dfbdce29e3d45313ddb9928e1e461e8ddc29cee74423f4f53e269d6ea2c54`  
		Last Modified: Thu, 03 Jun 2021 21:44:40 GMT  
		Size: 976.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e8b9c69e5e4c0cee13a073888150e75c694c15fb2db5944343fbeec7533f8`  
		Last Modified: Thu, 03 Jun 2021 21:44:40 GMT  
		Size: 2.5 KB (2512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
