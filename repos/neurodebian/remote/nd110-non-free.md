## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:15999f52939cf28d4de2cd484c9b555987530460d65ba939ac503aacfc68c4a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:5c9c87273826dee00930a85da52cc9df5e969d56aafed84c107c32e0cfb77ad9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63073452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5732070bf7622d9abe382d2d9533f43f04607c5868ddf4fe1479039407a264c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:21:21 GMT
ADD file:d8f8a66e04b091b1ee6d1d330b5cd80472768f8cef96db861ba4dfaa2472fe20 in / 
# Thu, 16 Apr 2020 03:21:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:01:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:01:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 16 Apr 2020 10:01:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 16 Apr 2020 10:01:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:01:49 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:3d9ec154a243cb2fcf510aa97241fa4d7c075add5b018b19db3f1dca9f93c83a`  
		Last Modified: Thu, 16 Apr 2020 03:30:54 GMT  
		Size: 52.0 MB (51968339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa85732a9920a84bda2b17d3ef9bbb0a38e893f804f99d8dc8751336331efd4f`  
		Last Modified: Thu, 16 Apr 2020 10:03:39 GMT  
		Size: 10.8 MB (10803315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8509b6a59a421ac767c6408357532b0a4b4971ea0aa4b541a9409a22797f045f`  
		Last Modified: Thu, 16 Apr 2020 10:03:37 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c5ff3d2f038411f6ec09c4800a727f2be16d8e7b67d5045b4a58545e79c56e`  
		Last Modified: Thu, 16 Apr 2020 10:03:37 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da320bc2fb08423a50441875c7bf7302f351f1876674a75f31cf7374bfd85ae3`  
		Last Modified: Thu, 16 Apr 2020 10:03:37 GMT  
		Size: 299.5 KB (299465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471d1137ec98b1de6e63aa351923468d7c214af2d7a41cd317d4ec368d979bae`  
		Last Modified: Thu, 16 Apr 2020 10:03:42 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
