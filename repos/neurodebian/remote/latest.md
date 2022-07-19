## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:5bb987b78bd323cf6ea59f5b8ded275192f2f07a12449526a5183c07b878ae9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:db0d9d0032ac6a179ffdcd26feaedbe194d74a91e32f570a63920c279ef5d50d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66623452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be85cf6927635fd9ac13558c580f7fcaadbb8e21ec62c7d74f42d717b2298075`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:57 GMT
ADD file:3451708ab45bc1bcfc1ebb2075d3af16767477cbeb79334959e0d1ff02b0864b in / 
# Tue, 12 Jul 2022 01:19:58 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:57:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:57:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jul 2022 04:57:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jul 2022 04:57:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d836772a1c1f9c4b1f280fb2a98ace30a4c4c87370f89aa092b35dfd9556278a`  
		Last Modified: Tue, 12 Jul 2022 01:24:06 GMT  
		Size: 55.0 MB (54999406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da754c27a57572208185a71b6ac71a984627b0de5c65ef03662f8dbc5272ec0e`  
		Last Modified: Tue, 12 Jul 2022 04:59:29 GMT  
		Size: 11.3 MB (11310715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da61b5d9a6e70cf7ef7bc4d13b7baa78ca8976919df22552a39687f75732162`  
		Last Modified: Tue, 12 Jul 2022 04:59:28 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bd63f04cdfc7d5594f2e661fb39f9a0f235df8cb54f0857802e4872cf924bb`  
		Last Modified: Tue, 12 Jul 2022 04:59:28 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59532075300b5d72c0d9112603dde5e9ea7fb33b27f988295c00fa305e415f47`  
		Last Modified: Tue, 12 Jul 2022 04:59:28 GMT  
		Size: 311.3 KB (311315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:24a7991e3758c779c19467a32f564f385627ab419a0458252b4b4a403954ba81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64894748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1300ae6c61e55e73d160290c859eb94aa3d5ce235c390f07a0c6e2446348a48`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:18 GMT
ADD file:2dcc013bca5a420cad3b6a1ac61f52ea58a29ae05fe282078a744979c0e1a89e in / 
# Tue, 12 Jul 2022 00:40:19 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:12:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:12:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:12:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:13:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfc947b533a3ed8b8ce79820c7fe5e7634bf9c08479ed0aee1e74ee7b4f2b068`  
		Last Modified: Tue, 12 Jul 2022 00:45:41 GMT  
		Size: 53.7 MB (53683129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1c6db8f8c1043b93ec52bcaf2c8898e5d1db36e057b7842f15003138d04653`  
		Last Modified: Tue, 19 Jul 2022 20:16:15 GMT  
		Size: 11.1 MB (11104685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a221be54e156076a192783180f5567f9f5e6bce8b860ac8c24ff9dab6e193f`  
		Last Modified: Tue, 19 Jul 2022 20:16:14 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e1f87b7556043f88c15ff9aaa17152e87c1026eccf028a149cb401e0d77dfa`  
		Last Modified: Tue, 19 Jul 2022 20:16:14 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5e107aadc1c0162a496208fcd7b4253f0a77a0a34875df86b3883e7aa4303f`  
		Last Modified: Tue, 19 Jul 2022 20:16:14 GMT  
		Size: 104.9 KB (104948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:latest` - linux; 386

```console
$ docker pull neurodebian@sha256:1f9a5be55f0af6fad3b619b97a0e0fdba0e80dbd500915b5b47b401a6e9079d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67608299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:112785ddd0fe1949b13f2c33561ba141e2e99664be685c19a655050e95a8880e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:10 GMT
ADD file:0fe47b589e2fdec2c7f7e92ab50ee94c37df9276c6771e612d29fde3aefb04b6 in / 
# Tue, 12 Jul 2022 00:39:11 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:09:11 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:09:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:09:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:09:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:992c2740c28ef02c375c076416e9a24c9172d5343205500b8388cf087a76bbce`  
		Last Modified: Tue, 12 Jul 2022 00:44:46 GMT  
		Size: 56.0 MB (56001770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406515da26ef0398404a272604f0d4b5e06cbaca5e26707879bbecb992675a25`  
		Last Modified: Tue, 19 Jul 2022 20:11:50 GMT  
		Size: 11.5 MB (11499600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdedaaf44d7e14ac8dabb23a227554f85fbafebc5fa4a93c797b50cf5ca096a`  
		Last Modified: Tue, 19 Jul 2022 20:11:49 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ffabad20ff15f2e2f0ac1c2a06eb3758a537a046acaf4860b02d1e6a2021d31`  
		Last Modified: Tue, 19 Jul 2022 20:11:48 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6a0c7d3848cd46a98bf6fc1b4d40fe29b5b7b1790257837df8924527bfbeac`  
		Last Modified: Tue, 19 Jul 2022 20:11:49 GMT  
		Size: 104.9 KB (104945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
