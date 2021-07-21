## `docker:20-dind`

```console
$ docker pull docker@sha256:b36fdccb118bfaa8d5026da5183a077b87bc790051fcd2c5686bfb8f7fa2563c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:4f0e01f764b10c633334cb44fe6926a27b06390b482cb24e1add823b2ca781fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.7 MB (81726552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca749f2062c41ad54191b9c242dd1b3f6132a11299b251fc2128e37c9800ebba`
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
# Wed, 21 Jul 2021 18:19:42 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:19:42 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:19:42 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:19:43 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:19:43 GMT
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
	-	`sha256:7f8d570be2274d0bfa2a8df30021696ca2af3e7a44553d24aa5f58314e32590b`  
		Last Modified: Wed, 21 Jul 2021 18:20:48 GMT  
		Size: 2.6 KB (2617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:778521a7c301de26994f7aca616ab10c1bc35b8f66b802345d0cad89af381dcb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75712568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a81be9fbf6452a40403d288e5b6a6c422b96bb07fc23d07ac2d46d5a92a63fa`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 22:33:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Tue, 15 Jun 2021 22:34:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 22:34:00 GMT
ENV DOCKER_VERSION=20.10.7
# Tue, 15 Jun 2021 22:34:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.7.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 15 Jun 2021 22:34:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 15 Jun 2021 22:34:06 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 15 Jun 2021 22:34:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 15 Jun 2021 22:34:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 22:34:07 GMT
CMD ["sh"]
# Tue, 15 Jun 2021 22:34:16 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 15 Jun 2021 22:34:17 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 15 Jun 2021 22:34:17 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 15 Jun 2021 22:34:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 21 Jul 2021 18:39:35 GMT
COPY file:89f2c7c1492b0cb067fc6be48e1edf3f04c0b6063371da4a48cd4ca35aa098d7 in /usr/local/bin/ 
# Wed, 21 Jul 2021 18:39:35 GMT
VOLUME [/var/lib/docker]
# Wed, 21 Jul 2021 18:39:36 GMT
EXPOSE 2375 2376
# Wed, 21 Jul 2021 18:39:36 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 21 Jul 2021 18:39:36 GMT
CMD []
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b2af61afd8be1692509633c019a7e81fa1569a3da52c9ea927e0918c359c9`  
		Last Modified: Tue, 15 Jun 2021 22:35:57 GMT  
		Size: 2.1 MB (2057868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822cd1a3e72a66f4a7545358b8beadbe33212146ff06a2622e305acd422f75d3`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829992c79f06822894e73d9a962015a75a5d65ef5a60de627fbb32a973dc0462`  
		Last Modified: Tue, 15 Jun 2021 22:36:03 GMT  
		Size: 64.4 MB (64423231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6714f1b9096eb751a830a9dd13c67cd5e669c68403f1675efd7e78ff8905896d`  
		Last Modified: Tue, 15 Jun 2021 22:35:49 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997b259c822c244af1192eb31913d45df7f269da56a37fa1c7dc5b9fe273134`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b041c447a8f648b5910833f3c76e5a3231d34a6d76b56d0c22c64b232da92519`  
		Last Modified: Tue, 15 Jun 2021 22:35:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f113d638e141615986b3c011ad91c657741ff84a21689c75c2159588d5fa89`  
		Last Modified: Tue, 15 Jun 2021 22:36:23 GMT  
		Size: 6.5 MB (6512663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b39bf84d6c6efaf352aeda8411d48487604fc126ff58dca169cff3ff189c31`  
		Last Modified: Tue, 15 Jun 2021 22:36:22 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0bd70db64874c3f0cd49b3492a9b270b52df5ed2834293a13cf84b0f2a2e54`  
		Last Modified: Tue, 15 Jun 2021 22:36:21 GMT  
		Size: 980.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79495f766691b68d3917bf6efd5a8faa1db74fe519664cf9546ac3cac184759`  
		Last Modified: Wed, 21 Jul 2021 18:41:23 GMT  
		Size: 2.6 KB (2622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
