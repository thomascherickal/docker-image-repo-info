## `neurodebian:bullseye-non-free`

```console
$ docker pull neurodebian@sha256:a26c1ef751f2c1ec66164348cd8a07475411551ccf0d5162426a1897fae3c3f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:bullseye-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:cd4a62ded3b2a4029d8d60b6b3ed6946fdaa85152a26fe917b5bf348d6ae5b1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66654419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6190f7d06f9fa41242c867712dd9ff36edb9a5adaec04ff63d8737a6a7281b37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:42:45 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:42:47 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Sep 2022 13:42:47 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Sep 2022 13:42:51 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:42:54 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec6dc792da68b626ddd326899c7a9f59f7ff89bad847f55024e8bcff81001c`  
		Last Modified: Tue, 13 Sep 2022 13:44:57 GMT  
		Size: 11.3 MB (11310695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fc1ec2890d12b8586af88bc30b2bd3ca0237c4e80605897261088e2919a67a`  
		Last Modified: Tue, 13 Sep 2022 13:44:56 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ade20a91842e889b19370099803ed68430d9837d27be025c9995fabc9d6ec4`  
		Last Modified: Tue, 13 Sep 2022 13:44:56 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafb459a0aeefd88f03e4560cdc2fee0c15c9edd37731b2e224b576edd82c6ab`  
		Last Modified: Tue, 13 Sep 2022 13:44:56 GMT  
		Size: 311.6 KB (311615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722c4732a1ff57d8536495ecef9a64c4aa57cd8947002958d7d4f79f42747247`  
		Last Modified: Tue, 13 Sep 2022 13:45:18 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:717f4ebdda7fa4eab149ba63da0c176bcda69205bb046ef0b75ebbc0e360e6fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64903738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48036d81e83c3a0bfca4aed5226d51de40e900592a94d74dcf2fe4b547044540`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:05:58 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:06:00 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Sep 2022 07:06:01 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Sep 2022 07:06:05 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:06:12 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf84e85c9009253ebcc229acc40978a1e42f890f70daca9386aef32223c6eb`  
		Last Modified: Tue, 13 Sep 2022 07:08:55 GMT  
		Size: 11.1 MB (11104851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92f71355e37af4ea896acc1e31e6fd69b4442303264d8aa0e2780325360d29e`  
		Last Modified: Tue, 13 Sep 2022 07:08:54 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055c2719fed71fff6dd175b00093776bc4fe9a257d377d46de5667c080040cec`  
		Last Modified: Tue, 13 Sep 2022 07:08:55 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6d431dcc3c94059b5ad51631595c2e2fe0d86c24156254e9e4510e62e71a64`  
		Last Modified: Tue, 13 Sep 2022 07:08:54 GMT  
		Size: 105.2 KB (105161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b76249264f83dc69c354f0d7aa99cac3ce2bd0b9c378bd6f0f71d4f5b778c9`  
		Last Modified: Tue, 13 Sep 2022 07:09:09 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:bullseye-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:298891862d22fa447d6c426f0413709a7de945137ca94af44b698f694a11d218
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67617114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7569a4864893f0583f90035088a7db4022bacb27441890a9502d229bb2a02a5e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:28 GMT
ADD file:7cd0a464573b537cf29f9a72bf3b895bfe96cce867ba3851402a98bca7272ca0 in / 
# Tue, 13 Sep 2022 01:39:28 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:56:23 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:56:25 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Sep 2022 06:56:26 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Sep 2022 06:56:31 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:56:36 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:c56ebffcd7db97f938c62b9ad03478fefdde78fc8b85916da5d75054970df458`  
		Last Modified: Tue, 13 Sep 2022 01:44:50 GMT  
		Size: 56.0 MB (56009860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc23c19625844dcaf8cfb318c96222a0a2ebd5bd88b44b9e19a304edc9faa5b`  
		Last Modified: Tue, 13 Sep 2022 06:58:36 GMT  
		Size: 11.5 MB (11499820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2d6cbd6b4697f0e7f266fa8d155b0674d201ab7d1616d9558b0cf65941ea25`  
		Last Modified: Tue, 13 Sep 2022 06:58:35 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f3a104dde43e346145799c0482a2ca9f3ef271bca3e7acc2fc3ee5605343ef`  
		Last Modified: Tue, 13 Sep 2022 06:58:35 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd86d5f236345628fe0621bbb590c6dc86ae7e72aa0ba22511b4c5f0411b5440`  
		Last Modified: Tue, 13 Sep 2022 06:58:35 GMT  
		Size: 105.1 KB (105085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f3a3361f66fb95146b894b4df976bf1cd0688d4764801f3e0b61fca1dc89f7`  
		Last Modified: Tue, 13 Sep 2022 06:58:50 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
