## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:3ea779c45743abd02464e211b4c6816184780f088d18f7739e2a735d2b7bfca6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:5fb8ea9a5123dde129b86a480b1d341462c8e0ef22dce6eadd75cfab37eef467
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61240359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a50ad57636ca67a54ee8207060850dca605fda2affdadc364fb29b59539f43`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:51:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:51:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 22 Jul 2021 09:51:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 22 Jul 2021 09:51:41 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff66d7acb9e05c47e0621027afb45a8dfa4665301a45f8f794a16bd8c8ae8205`  
		Last Modified: Thu, 22 Jul 2021 09:54:11 GMT  
		Size: 10.5 MB (10499949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac627f2d764f56d7380099754dd943f54a31247e9400d632a215b8bc4ec5fa2`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33c3e9e07dc85213c696c81aff06d286ba379571b799845954b6cc776457e5f`  
		Last Modified: Thu, 22 Jul 2021 09:54:09 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c4b1dfc179a7cb39a5bcbff0f4d529c84d1fab9395e799ab8a0350c620e58`  
		Last Modified: Thu, 22 Jul 2021 09:54:10 GMT  
		Size: 302.8 KB (302773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
