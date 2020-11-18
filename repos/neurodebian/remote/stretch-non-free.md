## `neurodebian:stretch-non-free`

```console
$ docker pull neurodebian@sha256:bfb0c0abff1d2d46932a55d247cc7e542afffa7fe193041ca6da380d585df5f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:stretch-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:3225f9256e9e2b185dd0ca28766fab2d8518d5cd8ad95c33a6d1a73870a2e100
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52241687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:105ffe03e56b37363a870f86f7cb0ac2dcd1a528bc003dc2c655cb300304cb33`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:10 GMT
ADD file:373a8875589f170b51fa677a3bf736feeb46ea278c553950a3eb3169a2056c12 in / 
# Tue, 17 Nov 2020 20:24:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:09:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:09:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 18 Nov 2020 00:09:51 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 18 Nov 2020 00:09:57 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:10:06 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:7919f5b7d60254cafc73c0d097b8ccffb72e0b6472957ece4dd5b378c5ca7cc1`  
		Last Modified: Tue, 17 Nov 2020 20:30:26 GMT  
		Size: 45.4 MB (45377037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4adc15799008b8b30772727b975f351ee0fe838ef246a90d627d51c0e86d9b6`  
		Last Modified: Wed, 18 Nov 2020 00:12:59 GMT  
		Size: 6.6 MB (6568740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae6a0a28cdc83bec018673698ba5877a952a28489fba0415728c429b60318bf`  
		Last Modified: Wed, 18 Nov 2020 00:12:58 GMT  
		Size: 3.2 KB (3152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5233b3c1d6c149e3db32f7a7c87276403cbb9d1b720ae95be2ef31c22e9a30ff`  
		Last Modified: Wed, 18 Nov 2020 00:12:58 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a05331609d78cd7bb8bf911446160b536977633c3616e1b869cdff5b73eec`  
		Last Modified: Wed, 18 Nov 2020 00:12:58 GMT  
		Size: 292.1 KB (292146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9c34cb2a4e42d057252ddc53a277c13f83935d2e8ab8795816cba1b846af55`  
		Last Modified: Wed, 18 Nov 2020 00:13:04 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
