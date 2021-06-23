## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:4521b5c4d5d7c927d54eb537aa801ea9b7d927515f15be1f538cc332e449f0b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:4fb75c98fe97616941fa8de3bbb9a7e3a091c7efce0ae660abf71ac7edec0ab6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61240829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97dc77a4561c8b4a799760c347f015a4ecab3c3fe755fc968ae8cfff25dcd5d7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 07:22:15 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:22:17 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 23 Jun 2021 07:22:19 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 23 Jun 2021 07:22:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 07:22:33 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df29a956644daed756498991df53ce80b516215727180fbb718335925a1e2a2b`  
		Last Modified: Wed, 23 Jun 2021 07:24:57 GMT  
		Size: 10.5 MB (10500040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78ec42a303e5fd5a1d8a5a4c29232fb159ae1a2a7a611e46af13bd5c869e3d4`  
		Last Modified: Wed, 23 Jun 2021 07:24:57 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980be1b50dda2165cf411d4db248ad169510abb0d30bdfdc304d2e076ac45d5f`  
		Last Modified: Wed, 23 Jun 2021 07:24:56 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe62a196f9ddc5ae0124fcb8352824c1ab367b92de87f3793d8bbdaec4326128`  
		Last Modified: Wed, 23 Jun 2021 07:24:56 GMT  
		Size: 302.8 KB (302792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bc2741cfd1575b635bc4e7290429ee22147216812b0cc12d6e950ee66fc679`  
		Last Modified: Wed, 23 Jun 2021 07:25:11 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
