## `neurodebian:bookworm`

```console
$ docker pull neurodebian@sha256:209633c2ed330c6f261ae579ff69bca5cbd47f1d080c066e307edc59eadb4960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:4bbebb1af3fa42edeb7daa76429594832677c061fbaa59f2176c8cbe40d8b607
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61305663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592dcc4b1cc3783782cfea69d58dcf8a1738781d2842c3849fd90d40df1b899a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:46:33 GMT
ADD file:168af20819ee8d7bc6ca3fd35873fe0b65f567f6fc4763ae2fed655e04826ef6 in / 
# Tue, 02 May 2023 23:46:33 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:49 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:50 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:879480f6969a02afb639ba9b35bc2df992fec064538a2e8af5e14cf6b6fbeac3`  
		Last Modified: Tue, 02 May 2023 23:49:26 GMT  
		Size: 49.3 MB (49299247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd09f14e055c828315e856789d20b8946366f27edf267f3902b57215e239d7ef`  
		Last Modified: Wed, 03 May 2023 21:27:34 GMT  
		Size: 11.7 MB (11719796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173622f5d1ba65e0d94854aa9998708f35b2a78b4a0c65ce6ec9cb2d772d4c39`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3666043593436d5565d087183a46b53a6ae13cb63c743b728fd872c3c48aa0e8`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f690a06a4d5ee8090896ae8454bdb93732d1e61586082cd7b596aad4aaf087`  
		Last Modified: Wed, 03 May 2023 21:27:32 GMT  
		Size: 284.6 KB (284613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:a80981db22ce79f3f3db70207bc0092364ef176a57c2987515b8c47548b3948e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61317834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:934fb56fccf1dde02985028c595e9ccbe712d48c421521d1ebc00b820b909d5b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:25 GMT
ADD file:1af23b8894efa507a47bf873cf69ecaa5ea13b618cae85b8c46125af6399b4fb in / 
# Wed, 03 May 2023 00:22:26 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:06:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:06:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 19:06:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 19:06:59 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15c964cdaf05fdeddcf9bddd79eba05f71f2859fee9c193ba5d19a237f7fb92e`  
		Last Modified: Wed, 03 May 2023 00:25:01 GMT  
		Size: 49.3 MB (49345335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e3d3070e602e9fb911e177cd185c101a4931dca0d639da6e18807fc49a799b`  
		Last Modified: Wed, 03 May 2023 19:08:31 GMT  
		Size: 11.7 MB (11685505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fa8b00f6084231e560eb18c348bdc14dae2a37c4d1d6c1019857500a4f487`  
		Last Modified: Wed, 03 May 2023 19:08:30 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2ab7185ac281378e315a5f2cf408933e50dca2c91dc4e17300122634da45b5`  
		Last Modified: Wed, 03 May 2023 19:08:30 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17619bd9b997d1ff16bc1feff04e21be4fc373cde7ec3852fcebdfd09644d498`  
		Last Modified: Wed, 03 May 2023 19:08:30 GMT  
		Size: 285.0 KB (284985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; 386

```console
$ docker pull neurodebian@sha256:468018d83c7365e482b84da94fd01831c32baeebb9143cb88486b84ce2347f2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62743186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:126b9b4eb830d6ebe5ccb6163c6a0d6db868355e1d60f3abb20f44a79f4e2dca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:30 GMT
ADD file:7718865253a3489583d40f8c7a7beede0c20cebbab68bb3e97ad2e84082afcb7 in / 
# Wed, 12 Apr 2023 00:38:30 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:06:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:06:45 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 12 Apr 2023 05:06:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 12 Apr 2023 05:06:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4ce9e81f634822e5166ef3eef875a4140795ac18afe0391433d72c7865bf67b`  
		Last Modified: Wed, 12 Apr 2023 00:41:43 GMT  
		Size: 50.3 MB (50317977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84da2d04e2213936972561f29d3c5c24b05c603098f55c356f500ff85c6ff72a`  
		Last Modified: Wed, 12 Apr 2023 05:08:06 GMT  
		Size: 12.1 MB (12141193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735656053c05260073c2e268f1a3dd6948d897c43a71237e34eead3d43ac135f`  
		Last Modified: Wed, 12 Apr 2023 05:08:04 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d0ea8ef8f29386c675e5ef1cd64a54b382852d99f3e19d57cce6e04a0eec72`  
		Last Modified: Wed, 12 Apr 2023 05:08:04 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46a95e50e161e774a1c7d8aba905988057369c3116e44a29c202e91dd4697ed`  
		Last Modified: Wed, 12 Apr 2023 05:08:05 GMT  
		Size: 282.0 KB (282004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
