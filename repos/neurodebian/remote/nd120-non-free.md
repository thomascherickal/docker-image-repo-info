## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:85d9b0cce56cb4538829179399caa5ae863ceefa821ec8a974cdb6b74023d447
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:11fcfec56adf85a2a6c29c74003c27c609ab851766ab333489431968d368e217
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64963218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8c42a3decbabec306dd86b81fd9f936e9909cab4b3166521bf63bbe058e3083`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:34 GMT
ADD file:e413c7d61ecdc96ab067e1f8bff6ce03c792c94b9d1f54e80cf633052c5d975a in / 
# Tue, 12 Jul 2022 01:19:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:57:51 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:57:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jul 2022 04:57:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jul 2022 04:57:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:58:01 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:7c7a32fcf1e30b18b7a9a032acf892763291bef7159859a35297bf81217bbee4`  
		Last Modified: Tue, 12 Jul 2022 01:23:29 GMT  
		Size: 53.0 MB (53022393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622b9e64a13adb2ec39801de6daa43bf1188cfd935031f612cb89c8120020347`  
		Last Modified: Tue, 12 Jul 2022 04:59:54 GMT  
		Size: 11.6 MB (11647040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb18285d163a3e7c2adc17ff28b99d1d4a5929e73bb8c30683af77986b88aac`  
		Last Modified: Tue, 12 Jul 2022 04:59:52 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e95e4a223c5b60da47a199e50dd435545b3dada916b9e2b8aae3aeed6d6767`  
		Last Modified: Tue, 12 Jul 2022 04:59:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38f3844b946448047ddc8a537538ba4589325ed4f642b8d43bd5284ce345c16`  
		Last Modified: Tue, 12 Jul 2022 04:59:53 GMT  
		Size: 291.4 KB (291412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd69fff3733db1fb0d33ccfd161c8d46cb35a531a38787dc27aaf0c7b4661a93`  
		Last Modified: Tue, 12 Jul 2022 05:00:03 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
