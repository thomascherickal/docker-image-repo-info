## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:0f5caf6ff3b68f1e9a1a4df0f5018df40d31e98a8b5248f6e6fa40a4cfc55f3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:ae6e1df013b07c2f8e42580da1322753030a87403dd3460b6ba33c7a78d487cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61315570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b4bd21363d3603ebce350347a80c9a2f6bd4e1aada22c9adb09370a21d04ab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:15 GMT
ADD file:7d8adf68670e8dc2af6b8603870ea610fc65ecbb08799f2ca6a3134f5d47d289 in / 
# Tue, 19 Dec 2023 01:20:16 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:26:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:10 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:26:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:26:15 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:26:19 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:bc0734b949dcdcabe5bfdf0c8b9f44491e0fce04cb10c9c6e76282b9f6abdf01`  
		Last Modified: Tue, 19 Dec 2023 01:24:35 GMT  
		Size: 49.6 MB (49561579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60813851d3d4129f056f873cc009e941a14179ae49d530351dee04ec0df8ad54`  
		Last Modified: Tue, 19 Dec 2023 17:27:54 GMT  
		Size: 11.5 MB (11463884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cfe18d5147ef1fe4b9a42ed7b57ca5c19f4ebe238093c00b4b7dbe943b7016`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de660d6bb77b3b3cc331a91c9a465ef1f3e4edbe3d63d0cbdc857fd691b63f1f`  
		Last Modified: Tue, 19 Dec 2023 17:27:52 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e384fde624b03e6309d39f76a15ddeff56a9ee7e8b1bf190f416e635708dcf98`  
		Last Modified: Tue, 19 Dec 2023 17:27:53 GMT  
		Size: 287.7 KB (287661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbb4d41320b96049bbafe069a4274f3ed09e0f6516709d539b0fc3096b204eb`  
		Last Modified: Tue, 19 Dec 2023 17:28:02 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:97e4b885432424139b795ac305ffa9735c8271a48c8540d8f7054494d8c8bf69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61310687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6557c9b6f643f36bfd3aecc7cd482c215de4f6ca556ef892d21dc013d02a4e08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:02 GMT
ADD file:412f80f75ed3e520f767e70b6b27fc81807f62fc5c6e5adf756507e33af9fa6b in / 
# Tue, 19 Dec 2023 01:41:02 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:06:22 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:23 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:06:24 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:06:27 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:06:31 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b66b4ecd3ecfb67b3b7a2a44b0199cbdfc94965c8bd3fefab75cd2e612799740`  
		Last Modified: Tue, 19 Dec 2023 01:44:14 GMT  
		Size: 49.6 MB (49592259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536d08fe62d16991ed44688b2a03cf0a9ad4c1a6a3c91a38aabff54d8dc121f2`  
		Last Modified: Tue, 19 Dec 2023 03:07:57 GMT  
		Size: 11.4 MB (11427684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17a3a06500c5196e68b32c08163cef7f17f514e1edc70f4d842ef892c4f5c5b`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edf619636202804b32b3951669c4b66707bb7af37e67f8a0be202699c87cb64`  
		Last Modified: Tue, 19 Dec 2023 03:07:55 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dcde0e73627274650648744924524389f5a680d3b32383a3b53fe1c475259a`  
		Last Modified: Tue, 19 Dec 2023 03:07:56 GMT  
		Size: 288.3 KB (288298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8378c25bd9411f0a142fee243394a286cc6f1f7c217d86581f263bb24ab74ea2`  
		Last Modified: Tue, 19 Dec 2023 03:08:05 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:f99434b0d8bcbdc85a6f4a6dc4f2d572af83eb4e4a853a144933fc1e19bc4606
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62756668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d8f03971e633e63c99322029d9a69b024c210cf1bab077dfb26f38441ef4f81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:38:52 GMT
ADD file:c20aace531a43765f8c1b69c75d7f46a4ab443377a663ab47e0bb2ceb013a611 in / 
# Tue, 19 Dec 2023 01:38:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:51:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:51:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:51:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:41 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:9b51fe964cb335e4bc3b61dca07146c7a0aa4c31e5ae9fec90f2a950818a21a4`  
		Last Modified: Tue, 19 Dec 2023 01:43:18 GMT  
		Size: 50.6 MB (50582312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2f81c47b7b130f3418b0d116d480499c54496b48208ed47c1d8fc839bf85d`  
		Last Modified: Tue, 19 Dec 2023 03:53:03 GMT  
		Size: 11.9 MB (11883835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a351a4d22f54a27ecd69f950120d824c9f9f5e6a6b20e9f258285459822f274`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205522c289f7b88de70a28984bb914948c84a0cc7c29500f7e1f730e0e9db0a4`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5dc22a3c30fe732622f96301ac945a4566da973563854c515b5ca6fac7855f`  
		Last Modified: Tue, 19 Dec 2023 03:53:01 GMT  
		Size: 288.1 KB (288078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5084ee365b51d3a05cddbfc8d59c329e46ad420b9fed6adfc9993e92d775d100`  
		Last Modified: Tue, 19 Dec 2023 03:53:11 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
