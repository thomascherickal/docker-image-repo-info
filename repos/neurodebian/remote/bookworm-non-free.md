## `neurodebian:bookworm-non-free`

```console
$ docker pull neurodebian@sha256:9297ea57c8e4c3f13f28668610b9ae587a610d42b430898b1819d0b02a50f882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bookworm-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:d52d4af080b7f4a4e2587186062e52d88603493ad425402cf20c95c0b116a2ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3e6a45d91905bfd06f5fbdcba0eab1a5024f5f049356cec05dd240eaaf04d6`
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
# Wed, 03 May 2023 21:25:56 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
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
	-	`sha256:2f5ffbe0a5537ef8771e9443b26e7da93ca8f8f2a26af66c24911e7d5259053a`  
		Last Modified: Wed, 03 May 2023 21:27:41 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:b69bfc4ed29a6d42fb7f32af35e35b1635ad6ed11266fabae4dead54f1adffc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61320839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:778d928a3fee1ce61884892a6b7f775f1089f3724facee289f262e14452a8abf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:42:54 GMT
ADD file:91184714f613e1768e87fad722350f471376a88cb595664e8e23864ce5d79071 in / 
# Tue, 23 May 2023 00:42:55 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:15 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 23 May 2023 02:30:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 23 May 2023 02:30:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:3485dc61c38c6db2e8092e9f4326fe6c51e867a1841f55346f74ec25847d7401`  
		Last Modified: Tue, 23 May 2023 00:45:14 GMT  
		Size: 49.3 MB (49347785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27205be5ff69de2ea80daf475b7d6782f5bd2c4eff02242061f43eaf6012d24`  
		Last Modified: Tue, 23 May 2023 02:31:39 GMT  
		Size: 11.7 MB (11685619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a91d72189acf1f099b7b4f36d85c03907fb5bacd266f36caa6b04ef2e3fd7fb`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae3bb66bd12fcefd327ecdad94e32054fc3501ea2c5f23a797f919ad31b9bc9`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e899ae9f9f58a47c33891e8ef8311f802cbff074ff152ecd2f6fa34be22900d1`  
		Last Modified: Tue, 23 May 2023 02:31:38 GMT  
		Size: 285.0 KB (284995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f11898d17a3e3cea8f36f6751eb691a7fc506a165af741c28422a9e0b52a8e5`  
		Last Modified: Tue, 23 May 2023 02:31:46 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bookworm-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:16cc40944ba50beee287eba7c32319d476c46ee7c1d316ce96367ac84fb64a5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62752596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df71d0bb8af9de01eb06854a17e811ed4938dcce437ab398a47e2992b8a637d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:00:17 GMT
ADD file:cd02b45138959c7ec7d466eff66efaa68d03b2e72f294b468f08c576643ac084 in / 
# Wed, 03 May 2023 00:00:18 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:17:02 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 23:17:04 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 23:17:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:17:14 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:028db28caf3d2a0b3bc8b8281c9f370a6ca8a97954f596e2b27e20ebf7f3b578`  
		Last Modified: Wed, 03 May 2023 00:04:07 GMT  
		Size: 50.3 MB (50321827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa3f2ae1595f6575bfc69faed0d539bf88a71f81033a72dd7cd6a6b16533a26`  
		Last Modified: Wed, 03 May 2023 23:18:26 GMT  
		Size: 12.1 MB (12143607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030d5cafe5a4885634636dec550fa431c5d4332902b7fa1e592504eb10cb4698`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc4a181c2202a0f49007cfb365321e0dc3352e79f05f6028e41b534da7b6018`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b687257037f8146aecaffcb99f883d553e938ba2d1635186ff1fde12e64952d8`  
		Last Modified: Wed, 03 May 2023 23:18:24 GMT  
		Size: 284.7 KB (284726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df75504459b747f4070dddcbeda95a33709c7b6352069c3f655621932713a20`  
		Last Modified: Wed, 03 May 2023 23:18:34 GMT  
		Size: 426.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
