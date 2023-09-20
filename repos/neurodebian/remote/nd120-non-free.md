## `neurodebian:nd120-non-free`

```console
$ docker pull neurodebian@sha256:08c4c3675caedc12adbda27737515740a36d9099ded1417e34068312d0615172
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd120-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:87dba6b9d8adee3f99273d50ee9ea3b4724362e9ae3fe495c8505080f11a009a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61310413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d5f41241bfaf1663c9a139b958367a80a11dc884ce6f3f7838928b5bcd26b4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:26 GMT
ADD file:ce04d6a354feaef93795269c859f36667fce9efda23c61b37d7060263b66ed4e in / 
# Wed, 20 Sep 2023 04:55:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 05:57:28 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:57:29 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Sep 2023 05:57:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Sep 2023 05:57:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:57:38 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:167b8a53ca4504bc6aa3182e336fa96f4ef76875d158c1933d3e2fa19c57e0c3`  
		Last Modified: Wed, 20 Sep 2023 04:59:55 GMT  
		Size: 49.6 MB (49557601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c419a0a1c8188a62c978c93260a8f9485b838e24cdd4b2f909204fe27ab0536`  
		Last Modified: Wed, 20 Sep 2023 05:59:05 GMT  
		Size: 11.5 MB (11463248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a442d8d1d593aebb6ee13cbd20afa90c396ea27d0716a638b5542d5179896ef`  
		Last Modified: Wed, 20 Sep 2023 05:59:03 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e887b385fcf90d26836d084c5116c780426caf59160025b4a549897404dba8`  
		Last Modified: Wed, 20 Sep 2023 05:59:03 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fdda28a81436332727d65db51a0d0e60eeb821587da5445180971d48b2af1f`  
		Last Modified: Wed, 20 Sep 2023 05:59:04 GMT  
		Size: 287.1 KB (287121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed060b55919cf78ea9c4bbe8ca634506ba9e846cbcb1fee6ecc0287ad1ebda9`  
		Last Modified: Wed, 20 Sep 2023 05:59:12 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:0e5a16242497ab0950c20f83f44ffde4f4acd394a7fdbb4000faf103a14a8e24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61308918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:191ab35fd4a93ea9629aa5e5eef3519fd574dd07854819222cf4591ae0bbe196`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:04 GMT
ADD file:7a0adbde6e967e2bcaafa69f04fabdec993025645c8d0d51acc991a31b404eed in / 
# Wed, 20 Sep 2023 02:44:05 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 16:39:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 16:39:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Sep 2023 16:39:31 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Sep 2023 16:39:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 16:39:37 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:796cc43785ac3cd0081892bd48e545a0615415265b60c794fdf81ac95b034213`  
		Last Modified: Wed, 20 Sep 2023 02:47:15 GMT  
		Size: 49.6 MB (49591881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da51d753a850f35cf2debc231b1c55344eb625ad11f8ec6e27b9ad849f2521`  
		Last Modified: Wed, 20 Sep 2023 16:41:04 GMT  
		Size: 11.4 MB (11426864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b615409dac2aeb2079b2835c33bb00cfc9eed155f874cf01931c870ed2a0e57`  
		Last Modified: Wed, 20 Sep 2023 16:41:03 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30080343cbfab5b6bf2b415949d623b22431f9d54af8679d92c1ec417c431709`  
		Last Modified: Wed, 20 Sep 2023 16:41:03 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4065b62dcf85149f96430c4a01925696d8792bb19cf2bfde60e8253e6bf04b9`  
		Last Modified: Wed, 20 Sep 2023 16:41:03 GMT  
		Size: 287.7 KB (287736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e998b052f4edba735dda0f35e0a85dadf95cc86c64245b96bdd0f061aad678`  
		Last Modified: Wed, 20 Sep 2023 16:41:12 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd120-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:bce291bfdfe7796a12fc42948a03ffe94e95621aa424a4ce54f7a53c1f342c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62742099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86dfcc2462c99e1119dde6b9dc68f70e3bfcc7d239bba8c5f71c82abc4bfd3d3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:41:42 GMT
ADD file:23c52eb6ca90f95eb3fff17deef5cfb900f1807fd50deae367183075f49aa81d in / 
# Wed, 20 Sep 2023 00:41:45 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:50:55 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:50:57 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Sep 2023 15:50:58 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Sep 2023 15:51:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:51:06 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b3de420baafed4c606a756da9f1ab4e930a007eb8cb0a1104bc280c0b7820cbf`  
		Last Modified: Wed, 20 Sep 2023 00:46:20 GMT  
		Size: 50.6 MB (50568965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d407e7dd48917b15ce3615b6941645bb2b8f6674e483a184612c4572359271e`  
		Last Modified: Wed, 20 Sep 2023 15:52:35 GMT  
		Size: 11.9 MB (11883277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a799390c5cb146e9fe812f9e5dd4b77466095c7195341978547e07842a43bc`  
		Last Modified: Wed, 20 Sep 2023 15:52:32 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80267344449c2bd0370e055810a0acc1571ba88e727a6f564c31e3317adef97f`  
		Last Modified: Wed, 20 Sep 2023 15:52:32 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0955d6969dd3e05da720ac7ab68a5bfa407607a3741859eec4507e536344d54`  
		Last Modified: Wed, 20 Sep 2023 15:52:32 GMT  
		Size: 287.4 KB (287416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5f8f04dd7f13c783dae4238f77db68e2a9a927ef4a26f819b16692ffbbf11d`  
		Last Modified: Wed, 20 Sep 2023 15:52:43 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
