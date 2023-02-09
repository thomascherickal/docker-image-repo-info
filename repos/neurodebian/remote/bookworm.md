## `neurodebian:bookworm`

```console
$ docker pull neurodebian@sha256:4bf980a902cb6e7571e8beaf42bbfbbe7b1bc4dc071491be355a63c9f66ae4b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm` - linux; amd64

```console
$ docker pull neurodebian@sha256:eb5a0a012ff4ce61cf3be35916cf6c57d17003f0d54cc1e73dce0f470ec5bbca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60987077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b561be2d8127b316aaf04f6bb16054759c690801338e869278a1edc135effea`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:19:36 GMT
ADD file:99a61197d7273704581c44eae01f3342e9f3562e84fe66cc2d56ce563e58450a in / 
# Thu, 09 Feb 2023 03:19:37 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:33:25 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:33:27 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 10:33:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 10:33:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45c04dd46fbf614b423b54561d34c6339a0376d1717729ef6dcf101dbfd20f8c`  
		Last Modified: Thu, 09 Feb 2023 03:24:14 GMT  
		Size: 49.1 MB (49054961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38236192934019393b60f6a155f92e7625f86d7040a25abc85f16331e3f20a9`  
		Last Modified: Thu, 09 Feb 2023 10:35:12 GMT  
		Size: 11.6 MB (11649251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ce3c24436d316066f2f512361cceecec6597a642758cd8a30a7e6be8045177`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389c3b6867a3b8b7a0990aed29d11f0ca7d3451728e8394e1ffd435a9860c08c`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3878ef31203d1f458f083c3adf2cefb760dd8bbc98002c0732519fe24393de`  
		Last Modified: Thu, 09 Feb 2023 10:35:11 GMT  
		Size: 280.9 KB (280853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:47d7a6535244ad6e95e521fd44c18618793ed1aa080c1eead00b9dcd26032188
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60978100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0990886517f471603003c7bff9a8442a9624b45903ac2c0307fba5b87c4eaf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:08 GMT
ADD file:b40ad920bd7dd081e20adf36435db50381b9998a1de3d2eac6b2c45734ce60b3 in / 
# Sat, 04 Feb 2023 06:17:09 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:49:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:49:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Feb 2023 08:49:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Feb 2023 08:49:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a43b5d5927a7651097e784be4430a6ade09951f5b6879cd06b0f51fc7c4812af`  
		Last Modified: Sat, 04 Feb 2023 06:20:30 GMT  
		Size: 49.1 MB (49081538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2178538c5bc5dcf98be54976e26e3643caa3a37f742386a75aeeda9818488236`  
		Last Modified: Sat, 04 Feb 2023 08:50:55 GMT  
		Size: 11.6 MB (11613318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5946ba90fc15d686558f937d9db8c112910bfcc60659eae41906cab00536fbd1`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d06715673a85e222fe91b40adfd40e6cf12abad4d8fc6b94aa1a329f289b576`  
		Last Modified: Sat, 04 Feb 2023 08:50:53 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302b2fd07b19b38ae39db22c7c35d3f8f01c22b33486483bc0f26dd2f8d1e600`  
		Last Modified: Sat, 04 Feb 2023 08:50:54 GMT  
		Size: 281.2 KB (281229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm` - linux; 386

```console
$ docker pull neurodebian@sha256:e37e3580493d2c03ad895fdd2504cc02a33c83c13b2a60bc1aa72e40ced14664
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62065634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7678b3f84b1c990678feca32d4533daea648cfe711fcc0e5fc012e584c6f8689`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:11 GMT
ADD file:37cc85485a8f79a4bd5557a42685805da0b367ff061d53fdf29d5f242593ea1d in / 
# Thu, 09 Feb 2023 05:12:12 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:43:50 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:43:52 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 09 Feb 2023 12:43:53 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 09 Feb 2023 12:43:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0153a17486e7cd96c30b54f1d68ab1cffaca99de43335324f16477807b1ddb1c`  
		Last Modified: Thu, 09 Feb 2023 05:17:35 GMT  
		Size: 50.1 MB (50089500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187a90aef6870d09282470d3b592e152d72bc909d4c41fc4d2a0dc6e35d578b`  
		Last Modified: Thu, 09 Feb 2023 12:46:01 GMT  
		Size: 11.9 MB (11882490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4ad0b3bec733e0fea46c5f1aa52aba6533737fae1c7ed922601bea2dbc7dbd`  
		Last Modified: Thu, 09 Feb 2023 12:45:58 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52056b4dd31d6fd76427109e57655ab7cdb36d3cdf6287f75d9ba2f4c8dcd0f`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8502cd76b08bed33327032c663ce30112feb1286d449672cffdf1346457ab1`  
		Last Modified: Thu, 09 Feb 2023 12:45:59 GMT  
		Size: 91.7 KB (91655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
