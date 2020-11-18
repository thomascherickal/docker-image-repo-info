## `neurodebian:jessie-non-free`

```console
$ docker pull neurodebian@sha256:c16c61cb17553ba862a6773e0b50df2787ca2d0c81581f93493d85eb2ce9d80b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:jessie-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:0bd7a95582cf51e73a9c7fcf045d9f90bd7c9ed93e4c95b3ed011da26457c633
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54694462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a992bdb7906eee392e36d37c271f392ef744869bd03abfbbffe96fa0aea7061`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:33 GMT
ADD file:a6871f73455488933c1b46ec3a892d3db537f631c01e75573369c7c45b41d017 in / 
# Tue, 17 Nov 2020 20:21:33 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:06:34 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:07:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 18 Nov 2020 00:07:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian jessie main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel jessie main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 18 Nov 2020 00:09:08 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:09:29 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:dbcd895dc67d5ce0b25d47678d747226ed725a22e31901fc021fd23879b1ccfe`  
		Last Modified: Tue, 17 Nov 2020 20:27:44 GMT  
		Size: 54.4 MB (54388442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137bcdee1f4be51accbb09b8a0a23d2e43d4993c6a71cb42cf7fe40ce8a78d19`  
		Last Modified: Wed, 18 Nov 2020 00:12:42 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0d97b2a59729a6a163e84ae6f3bc9064649ecb2fbe6182257c9ec3d5ab65e8`  
		Last Modified: Wed, 18 Nov 2020 00:12:45 GMT  
		Size: 3.2 KB (3155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd07396237864c106886ba126f4499dbe6a88762870cbc74a7eb1d089a49c23d`  
		Last Modified: Wed, 18 Nov 2020 00:12:46 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea22a65f019bfdffc8d8175a5d31118547e8a79ab67ac15523c2c588c69783d3`  
		Last Modified: Wed, 18 Nov 2020 00:12:43 GMT  
		Size: 302.0 KB (301959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5e828b7c7dcbc61eb2a2ebf03289a8405367ae3bdc78e8fc883bfa7961e468`  
		Last Modified: Wed, 18 Nov 2020 00:12:53 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
