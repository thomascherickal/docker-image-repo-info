## `neurodebian:nd-non-free`

```console
$ docker pull neurodebian@sha256:03525c8236075c36d3706ab57d18cea68b6205db8e7c798b226f2520e63f3c8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:8bf257824aefa8385ad61f019be968c3ad774b46de888ffc6a0289f589144be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65213680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b299f8fa9025b01fda6c1a485c3d1d8ae5587c500753eb30e0d3fb7912b860e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:23:12 GMT
ADD file:67c1d3c6f8f2705b6f6d6b4762836596ce976447eae7be0ec98e100a9231ebce in / 
# Tue, 21 Nov 2023 05:23:12 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:03:01 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:03:02 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 21 Nov 2023 09:03:03 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 21 Nov 2023 09:03:07 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:03:12 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:5af5a460cbb647bf09bd5ad2cdefd21714ccd512b0a7fba09506cd06308c9d18`  
		Last Modified: Tue, 21 Nov 2023 05:28:47 GMT  
		Size: 52.1 MB (52122268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5637e2505f3efe6a087f0f58c43c8fa65c0d83fd30901d7560db79c143a89afe`  
		Last Modified: Tue, 21 Nov 2023 09:04:40 GMT  
		Size: 12.8 MB (12802830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bd83037a1745411887e11ab89e62bb031e2361c3db34862b23ca31dee441e1`  
		Last Modified: Tue, 21 Nov 2023 09:04:38 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837ae61a5f7f79b1d181aaba6974a82f53dcc648a239770ffeef958fdfb6a5fb`  
		Last Modified: Tue, 21 Nov 2023 09:04:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536170650855aec71462bc8423f1f5c9bb8c63968ba94830b610238d565d624c`  
		Last Modified: Tue, 21 Nov 2023 09:04:38 GMT  
		Size: 286.2 KB (286177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2248e03a81aac3ef875d327ae662c63d1e610cff26c081cb48860b88ee6b82`  
		Last Modified: Tue, 21 Nov 2023 09:04:48 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:b60b35b544c37e3992af9ba8f34583a596793ff6f3baa73fd2f496fabe4100b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (63952425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:534c5c4f00ea7262fb367c1afe91f242add4bbbcce3c0903e2e3f56012396f70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:45 GMT
ADD file:1a4ef85bba464538c4f87a65a055d954fc8edc51f26efd06b43d8ae9f7e54f7a in / 
# Wed, 01 Nov 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:28:53 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:28:54 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 01 Nov 2023 11:28:55 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 01 Nov 2023 11:28:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:29:05 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:ba6956ade110f0fe56bbad19a8d10b1eb0ae1b1006ccba5fadff0026a00dbc20`  
		Last Modified: Wed, 01 Nov 2023 00:45:46 GMT  
		Size: 49.6 MB (49552835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fbbac0d173796cda178a2a5a16ef5653fd220176a8c1565a0e86578dfd5b43`  
		Last Modified: Wed, 01 Nov 2023 11:30:38 GMT  
		Size: 14.1 MB (14110787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ad058d489d17b39a4da4559d4d1da74e03361e46fa5e3670d997ec2851b10d`  
		Last Modified: Wed, 01 Nov 2023 11:30:36 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f70086a1d7c6eaf83af96a052b81bf45319b8dc5ed934fe6f18df5d0b9ee2cb`  
		Last Modified: Wed, 01 Nov 2023 11:30:38 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72569af24d4890ff6a8af7435d326bafb016e91e61cceff66cadaa06b017c6b3`  
		Last Modified: Wed, 01 Nov 2023 11:30:36 GMT  
		Size: 286.4 KB (286401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c467fbd63429b91d1c94869d85f3dbc1a01abf80c565ed8574b528fa3e4e2bf`  
		Last Modified: Wed, 01 Nov 2023 11:30:47 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:d222c9085205ffd8cdd192873b2c15989742731a462f656fc3c567c25e7b3c6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66616506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:809282ab9702dd2dc7d06cb5a02a90fa332eae02fb13dc23702ca522f4f250a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:41:31 GMT
ADD file:bfc7d40a1647cd24272e8bfe066e6291b5008d468149e8da8912743fb73ca9d1 in / 
# Tue, 21 Nov 2023 04:41:32 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:31:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:31:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 21 Nov 2023 14:31:48 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 21 Nov 2023 14:31:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 14:32:00 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:949c066c0a11d2827a1530818a7ddd8a28c5483bc3fa53f584688eb4a8d87843`  
		Last Modified: Tue, 21 Nov 2023 04:47:52 GMT  
		Size: 50.5 MB (50513831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182b5c261bb2841cbe40eccea3d06d6ae29ec07bbab7906c62e6fac5870ea4f`  
		Last Modified: Tue, 21 Nov 2023 14:33:22 GMT  
		Size: 15.8 MB (15814181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540ee0846cd3a515615f86a4f84d28ee1905b0e5152373e2803718696ef9f1c1`  
		Last Modified: Tue, 21 Nov 2023 14:33:20 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64a49d53f3b0bb91225a9b455e0b1a38fc6e97317572314c641cb2e2fa44658`  
		Last Modified: Tue, 21 Nov 2023 14:33:20 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dcdb49c52ddc53f6fbe10b48b8325990951e4ee8a4ae9d84ae592b34ed006c`  
		Last Modified: Tue, 21 Nov 2023 14:33:20 GMT  
		Size: 286.1 KB (286088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e00755984ceeb9a5cfe155639c8dfb376643e8464565bdb3775399a3c28224`  
		Last Modified: Tue, 21 Nov 2023 14:33:31 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
