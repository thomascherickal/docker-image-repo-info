## `neurodebian:stretch`

```console
$ docker pull neurodebian@sha256:9f3da1fdba79f31520ce900d5d60558743a06856d43e6448d571409db11ad8e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:stretch` - linux; amd64

```console
$ docker pull neurodebian@sha256:5521b411a3d4b7796641679718c7d7bdb83d11caf5b57b619099543c3f5e8e52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52244885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eadc2abb2a4dfd1a2f8cd95e0e999f5ca113143aded12798939eaf283c009cd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:24:08 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:24:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jan 2021 10:24:12 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jan 2021 10:24:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f084dff0e60775aaf4874bbc7c4e76361daafd5a589f187c544522980e641a58`  
		Last Modified: Tue, 12 Jan 2021 10:27:26 GMT  
		Size: 6.6 MB (6569369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9901d1c3ba6f89ccea9f16da4eb9c465cdc69e63ec888b6101d74a62a724536`  
		Last Modified: Tue, 12 Jan 2021 10:27:23 GMT  
		Size: 3.1 KB (3150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cce4dca0f6a8195b3aae5d8e745f26ac19f8bb60831a0a57d4e561d074c788`  
		Last Modified: Tue, 12 Jan 2021 10:27:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c03f7051886dd81fde8dee64069b37e389d024da6586f0d7c1d1a28838df30`  
		Last Modified: Tue, 12 Jan 2021 10:27:24 GMT  
		Size: 292.1 KB (292105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
