## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:6676dae888d70b8f8685f77320790077d191118c0df57b8d42f8a4ca8b37b409
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:f6f5065be23c37fd5d00a5d30a13cbfc0868b89ea18bcee4ed3d7692465af799
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66565350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97b1895aa3040850109e5e34f141d6af4b174388d9dd0391be6bb7ba9561c27`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:15 GMT
ADD file:3a81c181c66f226bd6abd48d0c7ed8a9c599c9f521ec7229286c83161afec8c2 in / 
# Wed, 20 Apr 2022 04:43:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:08:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:08:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Apr 2022 10:08:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Apr 2022 10:08:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6aefca2dc61dcbcd268b8a9861e552f9cdb69e57242faec64ac120d2355a9c1a`  
		Last Modified: Wed, 20 Apr 2022 04:47:57 GMT  
		Size: 54.9 MB (54941777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6773754bf9ecd6c3ef4926d332fa264c60397b845f1de6b4508ad0749fb5d39`  
		Last Modified: Wed, 20 Apr 2022 10:11:12 GMT  
		Size: 11.3 MB (11310328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03de105527d54617eace6cf869ef56b94d72d749c15123fab207d51932e7ec0f`  
		Last Modified: Wed, 20 Apr 2022 10:11:11 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88faf4d740b7e0d694752c5883749ff5be835fbfd2f31c0cbbce0156f5438a8`  
		Last Modified: Wed, 20 Apr 2022 10:11:11 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6f61b3dcb23749d796c1e7c9bfff0747655d4e78bbfc17969aff09eb7ebbc1`  
		Last Modified: Wed, 20 Apr 2022 10:11:11 GMT  
		Size: 311.2 KB (311236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
