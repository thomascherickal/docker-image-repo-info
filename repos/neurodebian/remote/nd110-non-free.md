## `neurodebian:nd110-non-free`

```console
$ docker pull neurodebian@sha256:75a5bffeebc754c9a9fd60344a0c284bb87bfa6a2491b56e221eab14b3edd11b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd110-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:efc5185ea1ea0315adfca08f92d57371878abcfca6c32ab5b4b51e2ed4fbf319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66680125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9274fa4dd6ba4308dd1ddad6b420ce33c66cba0a81e60de0e9f49ec9338ae54`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:02:18 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:02:19 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 21 Nov 2023 09:02:20 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 21 Nov 2023 09:02:23 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:02:28 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ded3b2c2e2705491306395f08e76557f7e2f3651c3afef8d378b275b64072b`  
		Last Modified: Tue, 21 Nov 2023 09:04:00 GMT  
		Size: 11.3 MB (11311866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf6d0ca7d99eecd6a7cd31df4a5c04fcc54b7bc95fbc3519c85a9d94ea0b904`  
		Last Modified: Tue, 21 Nov 2023 09:03:58 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8e54e234dff5f0348e5be547bb64b796452673f0bd183aa678099e28644718`  
		Last Modified: Tue, 21 Nov 2023 09:03:58 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b00d546a47901fba7ca367a3a5ddf441368999a84fd038f22d24edf494b1331`  
		Last Modified: Tue, 21 Nov 2023 09:03:59 GMT  
		Size: 308.0 KB (307980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2e70bf7609d3493c50eba4ba8870a2d45f74b0a94ece0dda543b8c88132f84`  
		Last Modified: Tue, 21 Nov 2023 09:04:10 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:9cb15b194da81e73a7bc555e1aba739ca44ab08e1460b99807bd7d79cbeae794
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65331488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4367b6dbb4a0d4cd561394fb567215803f00ab2024fad0d79be1d09cda37240a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:28:20 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:28:22 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Nov 2023 11:28:22 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Nov 2023 11:28:25 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:28:29 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918a7a3efaa0b614824a277c87b0b0645ce498231b25d127472f8cf1b21374e7`  
		Last Modified: Wed, 01 Nov 2023 11:29:55 GMT  
		Size: 11.3 MB (11313485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847fc8928ed4b25edde54e1a30259c987b3907a9401f34f2de6997924fa54aa4`  
		Last Modified: Wed, 01 Nov 2023 11:29:54 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ff8480b77e6f1e64715dbf9ebca0833cf162349bac0acbe1012e7ef0b6e7f8`  
		Last Modified: Wed, 01 Nov 2023 11:29:54 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd88e1c6d85ec9d08368ac3c6cd436ec0aef8357548e6aec6c58b2bc942b11dd`  
		Last Modified: Wed, 01 Nov 2023 11:29:54 GMT  
		Size: 307.9 KB (307873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f7fa6b57db4435901ab55ff8fb2650c2f7f8373b0b8b76aff97ad570f941ef`  
		Last Modified: Wed, 01 Nov 2023 11:30:07 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd110-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:408ee292857a50d9d9b699cdd1b4a99dce9df674023310b889a85db7d3c83c25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68065246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab103aee3929fdf80404d259809ea54a00c5125a930050fc4ab2dac034746e27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:30:57 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:30:58 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 21 Nov 2023 14:30:59 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 21 Nov 2023 14:31:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:31:07 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77840b98c3fa8471f66c5fd8dd6a2447440dc2414e84d31a9a0985d56d10c584`  
		Last Modified: Tue, 21 Nov 2023 14:32:40 GMT  
		Size: 11.7 MB (11708760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8e672974bdc893ee8353ae22bb6ba34f89b49b2d02ef64992f1da171572647`  
		Last Modified: Tue, 21 Nov 2023 14:32:38 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d827a4b097e5fb4b060a66b9ba4347d8d3c845ddf065117d247391a4a49ebfd4`  
		Last Modified: Tue, 21 Nov 2023 14:32:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c428c5f2820137e86d46efcccd105286d0bc1fcc875d397581a8bfbfb8b8e096`  
		Last Modified: Tue, 21 Nov 2023 14:32:38 GMT  
		Size: 307.8 KB (307812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573c3dda3f89ef5439e308319d9a6be16e9bdbffc8128df3cb285e1452a8b4b3`  
		Last Modified: Tue, 21 Nov 2023 14:32:50 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
