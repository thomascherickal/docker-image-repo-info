## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:4fee672a6c8f7b877f5867639041b05b6f5295c20f6d4055a17647c1e683928a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:a70c2a25f5b55499baa18733b8d19c2ee7f345e19f9559d1280d54b57c6f5123
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61259783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5134998283e1f7dc5d8979865877ce77c7a4ab55bb9cca9ed28dcdebcdce46d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:03 GMT
ADD file:96ca7e18b6141668321140f8ae1a496641f631313035513f1f9314e9dad2cd71 in / 
# Tue, 15 Nov 2022 04:05:04 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:10:54 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:10:55 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 15 Nov 2022 13:10:56 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 15 Nov 2022 13:11:00 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:11:04 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:2730d739afad9b8ff3e3029e23fd69d9533603751d6e42053ce0068c2b58e258`  
		Last Modified: Tue, 15 Nov 2022 04:09:05 GMT  
		Size: 50.4 MB (50448823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fca1bc133dec52587564a08d86ecf97ccbd619c537a10d7523e214fd7dc979`  
		Last Modified: Tue, 15 Nov 2022 13:12:52 GMT  
		Size: 10.5 MB (10504260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e431fb20443b2100d30c4dbaee3fc077f7cdf06ea25db1a50095ae44f9bf01b4`  
		Last Modified: Tue, 15 Nov 2022 13:12:50 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5daab9e1641bf6cd75e404663309d1587f798a59e047761730a172bb06d8671`  
		Last Modified: Tue, 15 Nov 2022 13:12:50 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3932639071cd8a9aed3bca4f449664c9c7021d039099b1d7a4b562f2bfe2d8`  
		Last Modified: Tue, 15 Nov 2022 13:12:51 GMT  
		Size: 304.3 KB (304328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422d382acd10c8c2796a2643e37f5aceedb11d912150e9b632bb2b80ac2d0ca2`  
		Last Modified: Tue, 15 Nov 2022 13:13:00 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d7785f4ad7f830e08370dfd1d39fc980e5e91b538dc9d27eaa35e19894f34779
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60050588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:052d48a40b4356c8e18a71a3a54c892347056abbe7e9b01dc9d3d7e44d798d8e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:26 GMT
ADD file:2122642b8ad9a333f73cba41ff9cc829542740e0e3c88379a7c9511fbfc28991 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:24:30 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:24:31 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 15 Nov 2022 12:24:32 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 15 Nov 2022 12:24:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:24:39 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:34983cc1fd1c67f0d8b7b8b4320539206a1c098388b3a671abe88b45f157978d`  
		Last Modified: Tue, 15 Nov 2022 01:44:52 GMT  
		Size: 49.2 MB (49233786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a01cb96d12fb6eeea1353b901942dd09d0ed678226febdef17e85a911666ba0`  
		Last Modified: Tue, 15 Nov 2022 12:26:18 GMT  
		Size: 10.5 MB (10510153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a09e08b8009ba019b2c3aa56c914392ae54967449a79551a84665878d969bd`  
		Last Modified: Tue, 15 Nov 2022 12:26:16 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1403e78c83fa6547374c59ddc32abb6fde5868c505cd3dfcd7d3cb9fded86509`  
		Last Modified: Tue, 15 Nov 2022 12:26:16 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505c1d185ca4c683660c314c93fcaa2622c409883b2f8ff1000459cd2bc4e337`  
		Last Modified: Tue, 15 Nov 2022 12:26:17 GMT  
		Size: 304.3 KB (304284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38054f2236f22c750ce67afb96836292caa75662cbf25637cacc023fe65ce81`  
		Last Modified: Tue, 15 Nov 2022 12:26:26 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:02087f06598fc2afa2769e0db26c9ef36ce321bdfad9982c937f17f01f2464be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61990996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7cefda656644799350ea5ccca373c1111efd90d03ac4acefd66a7c392fef21f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:38 GMT
ADD file:e8c5010609ee5ceb22093e461dbe3f9748a4d6ca2fd436e635276b0f99e777e8 in / 
# Tue, 15 Nov 2022 01:41:39 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 09:04:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 09:04:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 15 Nov 2022 09:04:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 15 Nov 2022 09:04:10 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 09:04:16 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a9674eda0741cb717f181697e2f2695ea87fdaf557d253407a096f80ad4f9fb3`  
		Last Modified: Tue, 15 Nov 2022 01:47:27 GMT  
		Size: 51.2 MB (51207653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32b7bcd7087544177338284a50004d2e02cfac59dd38718c22498da128bbf35`  
		Last Modified: Tue, 15 Nov 2022 09:06:25 GMT  
		Size: 10.7 MB (10672283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3dbcaf37259f807fbefa9fc997c00f13a7ff211a7422ea0aa4bb5e0a988062`  
		Last Modified: Tue, 15 Nov 2022 09:06:23 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27da7b13055889d8af547a5b80c4aecfddc77e8dfc31bc6f77b3b87ac174a246`  
		Last Modified: Tue, 15 Nov 2022 09:06:24 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85d8557710c21914b39bdde005c03e499ccd54f844f892dbff926dfd8f54d7f`  
		Last Modified: Tue, 15 Nov 2022 09:06:24 GMT  
		Size: 108.7 KB (108716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898aa8fcc1d1273071a252588933e8b5bf9710ec8c945726beee1d79a3adb2cb`  
		Last Modified: Tue, 15 Nov 2022 09:06:34 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
