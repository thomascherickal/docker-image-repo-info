<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `irssi`

-	[`irssi:1`](#irssi1)
-	[`irssi:1-alpine`](#irssi1-alpine)
-	[`irssi:1-alpine3.18`](#irssi1-alpine318)
-	[`irssi:1-bookworm`](#irssi1-bookworm)
-	[`irssi:1.4`](#irssi14)
-	[`irssi:1.4-alpine`](#irssi14-alpine)
-	[`irssi:1.4-alpine3.18`](#irssi14-alpine318)
-	[`irssi:1.4-bookworm`](#irssi14-bookworm)
-	[`irssi:1.4.5`](#irssi145)
-	[`irssi:1.4.5-alpine`](#irssi145-alpine)
-	[`irssi:1.4.5-alpine3.18`](#irssi145-alpine318)
-	[`irssi:1.4.5-bookworm`](#irssi145-bookworm)
-	[`irssi:alpine`](#irssialpine)
-	[`irssi:alpine3.18`](#irssialpine318)
-	[`irssi:bookworm`](#irssibookworm)
-	[`irssi:latest`](#irssilatest)

## `irssi:1`

```console
$ docker pull irssi@sha256:9a77d1df6e590fef8eaae7ba475f2e5a9c43724bec98aff23d9b1631b9220d75
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1` - linux; amd64

```console
$ docker pull irssi@sha256:5d9147f3379e4b79b86271b8b280d77d7b23212e3a1877b71225a508538a41c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75862383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9176b56d5f8434c83bfe4ca38d64d1fd86b07a0fd49ffe1208f4b5efa59f9fd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1eea906c30d3d0487ae55380baa41c0f4d8b8e35308aac724e9ff9bcec124642`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 18.3 MB (18260013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f0ebb89009ec7651e1ddcb8eb0a59774e42c3bc06a4b223df4b200220914da4`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54234223781082d0352cc2ea4da765bdd0ac4e5c9cc00c8081a79eced99414b9`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 28.5 MB (28473044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1` - unknown; unknown

```console
$ docker pull irssi@sha256:19511cb18b259e0e6c94ab3fce7c9be3ba16ef514db9f61cb7a30193f7fdec1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6634888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381d2efeff58df84e748ac3cbe9d2e46d374c1cd2291648e8a039a13c5393e0`

```dockerfile
```

-	Layers:
	-	`sha256:90cbaa48e8b08df31e60931aabf94fc30837256b3c5d3ca4c4972ce0e97b7d26`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 6.6 MB (6616285 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:448eaa4bf506a9b017f8a3d2fc48ee0633391d71aa6df73781d518620d86b965`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 18.6 KB (18603 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:4286526b50c80fffe45f3d033e3fdc13e3f5c04cd6ad1ec14790c2ee8d039a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70039481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf2812ad5e9e3913d5e6e2487a3c5f13f004f7e92d10c414267119db631dba3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd87cc8398be751321cd22ca920bc62183e34f8b4b4ac4a608f07888091da0ce`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 17.0 MB (17034983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a18da79d125b945cad0e400520adaca406e8180d56d64777eac37d6b3d3a97b`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1bcc51f403f8b1d911866ad57127a5c25094f2229c92b9fe5c866e89f4c3ec4`  
		Last Modified: Wed, 20 Dec 2023 20:20:22 GMT  
		Size: 26.1 MB (26115697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1` - unknown; unknown

```console
$ docker pull irssi@sha256:57091b62d44164148afa83ea653c4e3ece0305c5481a3c9797e4c134c4bdc593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b36f2f3830b001060929f79c17d21c3bbcf8522ec030c4585413ef64492300`

```dockerfile
```

-	Layers:
	-	`sha256:be69a9e6f839e05382bfccafc02a33265cb58de10a9d4d54c62ca261eae2ceda`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 18.3 KB (18349 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:cb8f06b471dfaa3cd90e41f16b16b6dceaa08f113006002eb02a575759530ad3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66361909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9f07d2e179897cabf0bd0385a54c12835d517ff49a2acc7e2548f54f3c529c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9af19116d503c60c4477fb97778e4d00ec874702ca31ef19d4be65bd203ce75`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 16.6 MB (16627433 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b0e896ad984d1556dc3df25f1f24d17abd4bad05bd68f1ae582f687d457ae7b`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72a4105a0adfa8587dcd54b4600d7f905af063873577b5ff9b0fca192542e045`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 25.0 MB (25012958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1` - unknown; unknown

```console
$ docker pull irssi@sha256:bf41c4ef33d0cc113632b1d9778922afd7d5091de5188addeb1066d5b441420e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6609143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e21deee85550008b9520c1299b0e2697ab56f7d45900ae612816b74feed26d`

```dockerfile
```

-	Layers:
	-	`sha256:789bc7a90003a2b096536fa12b6be4abbef105dc07fbdd85f0ab2e91ecc6c42f`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 6.6 MB (6590579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:37d0d4185472fed8e3e965d668e307726812a2cd1b7543b76085eef8c33e4318`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 18.6 KB (18564 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:4448d99fff66a402267a1326cf56befb11179adc9a588d74d9d232ac6896d13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74613777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6be87e358baeb4ebdb34e1b0bf058728b4c9b4791df705a97af2459aa4b112`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:560bf72e987fd6edd06c8b56f9b1566b5262ee2c254adf3863299dd47c78fa92`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 18.0 MB (18021745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:980da2332d71ffeb3fb18a84dbd721f5c4a52f7dee942f6e1d8e85713a3890cc`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d851282e78a89fab2fca7d86db4275a5e68bb52ea170ef151be24211ee1ea9f`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 27.4 MB (27431401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1` - unknown; unknown

```console
$ docker pull irssi@sha256:51ef1e0b32d9b59ab96443e4f12015237b4289ae8365567cc267e8be313328b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6615458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae12ce93fbd3b325957885cb40c6582cd97d4d8fe0e69b96b92e469e333a84b`

```dockerfile
```

-	Layers:
	-	`sha256:e31580db9e488826eb1086346c8be3366de013ebbcd231d60ced6faca6d545ea`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 6.6 MB (6597004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1fdc10f0e5fa4cb00a3930219cf8bf8c5ea4d37cb721a83bc8eb8006e95dec45`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 18.5 KB (18454 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:6a8475ff3c12f74fc70976a5161b3fe205b5de6af186234af5f1b589963f5412
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76291252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bd0be5ca51091c547885af81aa5f9ce44a235139086622e3a6cc4425f42abb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f7dc5be6fb0db696a5c82ed11d73cbf826f8b763876f18c25833f1ac9db5a9e`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 17.8 MB (17785994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb9836a268b33d7bfd41001911da5ce8ade91fd68ae9ad1ad4a1444f46d5c802`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc2f90db82b28b52fb5cc5805f4a587ece1c5d91add681edbab73eb99d5829c5`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 28.4 MB (28358032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1` - unknown; unknown

```console
$ docker pull irssi@sha256:ca9217a9d59d109bd6ab0e81c9843708540d923c98f8f4089a0203337f0fb516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9feee74d3925e1773ca2cbdd6daa9468885e693129cf04d99d2b862d2ded7f`

```dockerfile
```

-	Layers:
	-	`sha256:f528901de35025479bc79bcbdceac123bb7b194efcd16d5831474114de792022`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 18.3 KB (18335 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:8cbeb7cfde7d32b8433e1c01c415fbd6ad8fa9cd259edd4313c1182a978eac09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74063255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b791cfba3e8bc5162ca9521ffdbb0820710918bc04a13a33e6f8be224f55438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:13:36 GMT
ADD file:dcd5696ac281b24df52a518e2402c7f7a4caedfcba0d82e195b7c06cd3a38fdd in / 
# Tue, 19 Dec 2023 02:13:40 GMT
CMD ["bash"]
# Wed, 20 Dec 2023 13:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Dec 2023 13:30:09 GMT
ENV HOME=/home/user
# Wed, 20 Dec 2023 13:30:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Dec 2023 13:30:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 13:30:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 20 Dec 2023 13:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Dec 2023 13:34:25 GMT
WORKDIR /home/user
# Wed, 20 Dec 2023 13:34:29 GMT
USER user
# Wed, 20 Dec 2023 13:34:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:12b1322ffb17b8e81ca1c6d9d7118e2fcee0b9d971aa3c90601e6345804a60d1`  
		Last Modified: Tue, 19 Dec 2023 02:24:36 GMT  
		Size: 29.1 MB (29121427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ad670e672d195ec763bd204f894d09cdc183c6ce311eba2ffc439612121ee`  
		Last Modified: Wed, 20 Dec 2023 13:35:14 GMT  
		Size: 16.9 MB (16929535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb1cb4c20719f053a8b365e7ae8908e7f3fc0b57887a9c01af2cff96600f8e7`  
		Last Modified: Wed, 20 Dec 2023 13:34:58 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fabfead7d49f06de8058ccfeab86b5aee8284be57ed979452324699df85abd1`  
		Last Modified: Wed, 20 Dec 2023 13:35:19 GMT  
		Size: 28.0 MB (28008995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:575ef209f28f4f7ed0a9a7b1c99df2bb2f87cd950a7977188d8be9408323b055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81858507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e1e484a868196a76e57f555fecc46159723e455f87f03731192a645f49205e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c6980c5acfb61420bec3fecb79e92baf26848104c2f1a8cf0d1754bca2bac3e`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 18.8 MB (18757646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:765deb34181ae86766afbb92b8adb60ed2d09436f8b805be2169b2f85c496f0b`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:622166be7f78a644c3966afdbc21cd1d72d5b61221fc50ec222cc6ff1bef82aa`  
		Last Modified: Wed, 20 Dec 2023 21:08:23 GMT  
		Size: 30.0 MB (29976941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1` - unknown; unknown

```console
$ docker pull irssi@sha256:1afc854d3abba98f2eb32986720d792629f71ee99d2d03d0f7c005f41125ae57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6627152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4510d937df9c77199f03f2ffc9c0d973e60235ae776b09cd1ddf79d983389`

```dockerfile
```

-	Layers:
	-	`sha256:8f0991cfc927c50f1f4496eb5371bc577a375f262aebd9f969e6fc90aa5b4f27`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 6.6 MB (6608650 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7204444fbb4c105206ab3f29c0589fc495706f2d07570acbc522140d7a09eb4d`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 18.5 KB (18502 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:60a482b86f2db7fd10d491938f31901c7f6adbac8c2463cb2e2fa62c3c30cf5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72724499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1a2b7df92545b5f83cf7c3dc5f7a38e9573ef5035b06654c733958586e67e7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0caafde47a3e9a6dd324ed419bf5fbf3927b27845c745b95d9c37e1bb7d63a8`  
		Last Modified: Wed, 20 Dec 2023 21:18:34 GMT  
		Size: 18.2 MB (18207265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3d931210f84c8b8a6fbeae35b4a75acad3d2255b470db4a1a421d40c38e2abc`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a383a09d5e97936abef74784a8ef9413735c27dd1a73de75fd3fe595c5719fd`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 27.0 MB (27021999 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1` - unknown; unknown

```console
$ docker pull irssi@sha256:f49bf849702833ecb1a8740440767542d2c5b9980182fde5e48de04801a43a0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6623640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ed98bb6c8dc6a0f89cdc2d7b3d5386486f3daadbfdf2b7237d3bfe0fcbeb41`

```dockerfile
```

-	Layers:
	-	`sha256:65127003855e314eb1d3819c53d0fbe07edefc65c019685ffaaed55b5556af43`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 6.6 MB (6605204 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:055af2286d41963c455bd993dbb42a317414c6a8b4b231e164463af193d45837`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 18.4 KB (18436 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:79451b25b3472ba9e2eaea3b2ac29fe6fe096d29e2c8906f5bc613d00d0aa5f5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:105fa5e67e4e73efc68a46251ccc88bcdd20c1f00791c024d72049ec8c262192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90a1bb4955c1fa1c41936729e39aea9920194ea59a1c610b1a3403c3f0c6150`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e0489114318ebbbb358ac5d32aee84c3a4b5533810fa6706b0648de63eada38`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 9.6 MB (9645476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdf0d195e7f83acc9eedf0071d583bf6af6349889841e7635cf29c43c629c640`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d108ad9c820b6d6e8e249ebc6d8880815c65c45f26892e8a6ab3c9ae45685853`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 5.4 MB (5402203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:d20bcdc49a8bcf8dc91e15bca6c781ebcd7c4dc4198b20d4e313fc2c9c439bee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.5 KB (992458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb852ef521ea46c7682f4f7119f23851f36317e79cce4556e2e9e416fbde2cf`

```dockerfile
```

-	Layers:
	-	`sha256:4cd7f1f45cebca0db6e6b84a0d40d4291bd1884fe3a99cd8699e1f85cc855931`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 975.0 KB (975030 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc7b354d55ff368937c54932656d0c6e35d054544cd811ae952e5339e561af61`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 17.4 KB (17428 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:502678281e0a8fc11e5e60ab54cf7dd84c2ee569f3f870ef4adcaab298fb417b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17270398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899b60c73aa2cd976bff10c64aadf2960af1ce82aa7137f963033a1c8a9e01ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410e5270be4aa0f019d84c2b63359fe74822bbb5d0b839fe7016fc64dfbc7ae0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 8.9 MB (8880076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1571fb6473dae031bdc723dcc05df8bcedb8e7949fe43e60b88b84d28de6359`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c99573a422ea748e601e3fc5a3c7147a082b13fa4b63b41d7410e26fe7185d0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 5.2 MB (5242159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:464a826b2af15230d1a2d27c265fe0c4cdfa1911cc91aa09aea53ed9cfba65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 KB (17341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9858ff23fdfea20d8cc88ee6f6d49900d4a8b83f719dc1bbab498204aa70e95b`

```dockerfile
```

-	Layers:
	-	`sha256:c698656fcb6933453517855d73664fa233a7df879ad29c65c2c7e6c9bd6af2b1`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 17.3 KB (17341 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:781db50a278b2665670bc3112c5c0397014ab37ff3c9f3d9a515449d00407b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5613a41dc765b890dc98b0f1b3c5ff9a53edd2e1445eb87311c9fc626682efe9`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:831415ea41c64b7ebb180f4f1da27bcf8dff3a9c5857deefa938de6334bc05c8`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 8.7 MB (8721217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95002d0dfc5013bc236502c1d58e95122a36e7ced9325e458f87721e74424053`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfcc5163f111398aff0073ad800b7fe8d98fa110ae443c658242fe5979989243`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 5.0 MB (5006513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:80029ca5ee21b65a87e5bffcd0f6e982ab1939bd3a2fd22627ae42ed2677e9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **995.0 KB (994964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be9e8234e96256b98972c25f2a33d5b2f9af93030aa1c99e11688eec589a33`

```dockerfile
```

-	Layers:
	-	`sha256:647518d13f1ec703d0cc9f34b31e2b53de88cb2616b0cb39b44211edcd1de409`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 977.6 KB (977574 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:76183270a354928c61dc0a73762989852386c1f766eb7a8a6f5773870e87ad5f`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 17.4 KB (17390 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9231eee1fd711f485f49771ef585253227fe5803335d2301087e2cb083f099a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18315846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4729d538632dda020f3bcd9bae8a2249d9cad5ae76a8f02f431fc37137c71a14`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86f46af68b50326d6225714f933de969fae879fd66189bbd1edbda8e47ab9343`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 9.7 MB (9673040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183fe6397c74bb1e7159b0a06eebe92da8dbd1b6af699e543a7618777a0bf315`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e28fc2012c204a8e8b903e0d3b7a042e4d5c0867e2e9eeb2340b29cd64ee66f`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 5.3 MB (5308483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:1c785db37c195270ba3ac1385d0509431549621d5ef5ef558ba9c4c1efa77e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.3 KB (992329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5548d8fc5c59a6fd473580a6b28b02ec1f638378bf3a473bf92331dc86e4db05`

```dockerfile
```

-	Layers:
	-	`sha256:90fad57a08e8809e193e2d976c2a6a59a19c5aaaba7933737ca575c34031f786`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 975.0 KB (975049 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:833e49bd915ced6aed85ab32c68fdbcc2809eac8f325ae4d6054353f2b8c1831`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 17.3 KB (17280 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:a1f46da9d4d08c6ee70f056809a0b2ff79fae6cf722de2cfeb95261aa38bd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff78bbd9939209b5459ddead2d5e68cdea113746073e595135cace9e852ac2bc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afaf371c77ae0674d22138365f359b4ac14ab68be729fe05c7a79e10d726b117`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 8.9 MB (8904451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efe2cca0d709017c0c09011188dd71a937d9f8b4bebc918d2715769719a2f16b`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50bd6dc1d315e6329e05543858a9c8fe102bc166e11901747897745475fa8386`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 5.4 MB (5413019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:6b8364870daa037625c5a97cca22cfda0428edadd69cb3c8a1d00dcfbd6d361a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 KB (17160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b3895d731ba30f2fc6f8e5011be07f0b49d6a34b0cbc66d53c7b5b7b11a335`

```dockerfile
```

-	Layers:
	-	`sha256:c1ddea5c446d03568ddef362b94f90e3f0eef9a1d9953f26955878608f254c4c`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 17.2 KB (17160 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:9c9e58cecb2a60d8f94969085766c8889efbf766f96f59995d5c7b98d1098ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47be3724f03dc5882cc67a78b812dd6776c63edffaba6e670d48085ce1472f7a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d37696a9b7f09eb3052928fc0b0a2bf6b1a9d8a79f15198f00b8f3d7c6f2180e`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 9.7 MB (9736559 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d528e90d2e0d255c01bbbc4d2ead9da704d8bdd46c9941f6e25e61535c53d4e0`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6afb000755ce978e9c79e6e950a600241bef0c449da1370170c9ed808493a309`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 5.6 MB (5630879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:dc9c2d5721c50d04edfdd24dff32af69861be9998efaa742fe7a60cbb6910e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.8 KB (990779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e21d3be4a225b0dee4f04888c254c8da7545ae5d64238735a130e36cf0b3ca5`

```dockerfile
```

-	Layers:
	-	`sha256:a940fbde6476c7e256b3940a1c2571f77dc47966416e58880da03224a07fc411`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 973.5 KB (973452 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:83574fc30d526c7e54ab92e98efeac06578035a04067c1ff1e80c611f8171a86`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 17.3 KB (17327 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:5e2a23003f460cd14e9bc7690c38f6cf05f8a8b254aeae4eafe9164679748305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18707567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95225b5cd25d8f282a3244a872e6e4a783f373df46a5542928d2be3a9ff4bce4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bdf85127dd33246430604be8364aad59011ec1408e05f2760d4365bd707acf5`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 10.1 MB (10083022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3884e11e9a45bef8f46aa3a109d16b19156260a3446a960d36030cda38e2c32d`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97af07dc776076badee757665cb2b7671730020e1c388a5f061fd4314ea988ab`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 5.4 MB (5405800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:05c6dcc8971095fe5681ef8bed84db1a50569df548468626288a5fcc3d2ed038
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.7 KB (990660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152c5fd0322f65eabee1d5613d5f8d91bff738d7a560de9dd19de26507b21a88`

```dockerfile
```

-	Layers:
	-	`sha256:631809d2b169208a798334a1300be704693429072ad3e80adccdcd04bd0fd3c6`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 973.4 KB (973394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7a2cc8c102e1399aff2d9b99a53977edfb5ea139a7b3ef1f0faf71a24a879f`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 17.3 KB (17266 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1-alpine3.18`

```console
$ docker pull irssi@sha256:79451b25b3472ba9e2eaea3b2ac29fe6fe096d29e2c8906f5bc613d00d0aa5f5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1-alpine3.18` - linux; amd64

```console
$ docker pull irssi@sha256:105fa5e67e4e73efc68a46251ccc88bcdd20c1f00791c024d72049ec8c262192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90a1bb4955c1fa1c41936729e39aea9920194ea59a1c610b1a3403c3f0c6150`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e0489114318ebbbb358ac5d32aee84c3a4b5533810fa6706b0648de63eada38`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 9.6 MB (9645476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdf0d195e7f83acc9eedf0071d583bf6af6349889841e7635cf29c43c629c640`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d108ad9c820b6d6e8e249ebc6d8880815c65c45f26892e8a6ab3c9ae45685853`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 5.4 MB (5402203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:d20bcdc49a8bcf8dc91e15bca6c781ebcd7c4dc4198b20d4e313fc2c9c439bee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.5 KB (992458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb852ef521ea46c7682f4f7119f23851f36317e79cce4556e2e9e416fbde2cf`

```dockerfile
```

-	Layers:
	-	`sha256:4cd7f1f45cebca0db6e6b84a0d40d4291bd1884fe3a99cd8699e1f85cc855931`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 975.0 KB (975030 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc7b354d55ff368937c54932656d0c6e35d054544cd811ae952e5339e561af61`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 17.4 KB (17428 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:502678281e0a8fc11e5e60ab54cf7dd84c2ee569f3f870ef4adcaab298fb417b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17270398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899b60c73aa2cd976bff10c64aadf2960af1ce82aa7137f963033a1c8a9e01ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410e5270be4aa0f019d84c2b63359fe74822bbb5d0b839fe7016fc64dfbc7ae0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 8.9 MB (8880076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1571fb6473dae031bdc723dcc05df8bcedb8e7949fe43e60b88b84d28de6359`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c99573a422ea748e601e3fc5a3c7147a082b13fa4b63b41d7410e26fe7185d0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 5.2 MB (5242159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:464a826b2af15230d1a2d27c265fe0c4cdfa1911cc91aa09aea53ed9cfba65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 KB (17341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9858ff23fdfea20d8cc88ee6f6d49900d4a8b83f719dc1bbab498204aa70e95b`

```dockerfile
```

-	Layers:
	-	`sha256:c698656fcb6933453517855d73664fa233a7df879ad29c65c2c7e6c9bd6af2b1`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 17.3 KB (17341 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:781db50a278b2665670bc3112c5c0397014ab37ff3c9f3d9a515449d00407b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5613a41dc765b890dc98b0f1b3c5ff9a53edd2e1445eb87311c9fc626682efe9`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:831415ea41c64b7ebb180f4f1da27bcf8dff3a9c5857deefa938de6334bc05c8`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 8.7 MB (8721217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95002d0dfc5013bc236502c1d58e95122a36e7ced9325e458f87721e74424053`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfcc5163f111398aff0073ad800b7fe8d98fa110ae443c658242fe5979989243`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 5.0 MB (5006513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:80029ca5ee21b65a87e5bffcd0f6e982ab1939bd3a2fd22627ae42ed2677e9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **995.0 KB (994964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be9e8234e96256b98972c25f2a33d5b2f9af93030aa1c99e11688eec589a33`

```dockerfile
```

-	Layers:
	-	`sha256:647518d13f1ec703d0cc9f34b31e2b53de88cb2616b0cb39b44211edcd1de409`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 977.6 KB (977574 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:76183270a354928c61dc0a73762989852386c1f766eb7a8a6f5773870e87ad5f`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 17.4 KB (17390 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9231eee1fd711f485f49771ef585253227fe5803335d2301087e2cb083f099a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18315846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4729d538632dda020f3bcd9bae8a2249d9cad5ae76a8f02f431fc37137c71a14`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86f46af68b50326d6225714f933de969fae879fd66189bbd1edbda8e47ab9343`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 9.7 MB (9673040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183fe6397c74bb1e7159b0a06eebe92da8dbd1b6af699e543a7618777a0bf315`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e28fc2012c204a8e8b903e0d3b7a042e4d5c0867e2e9eeb2340b29cd64ee66f`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 5.3 MB (5308483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:1c785db37c195270ba3ac1385d0509431549621d5ef5ef558ba9c4c1efa77e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.3 KB (992329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5548d8fc5c59a6fd473580a6b28b02ec1f638378bf3a473bf92331dc86e4db05`

```dockerfile
```

-	Layers:
	-	`sha256:90fad57a08e8809e193e2d976c2a6a59a19c5aaaba7933737ca575c34031f786`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 975.0 KB (975049 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:833e49bd915ced6aed85ab32c68fdbcc2809eac8f325ae4d6054353f2b8c1831`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 17.3 KB (17280 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:a1f46da9d4d08c6ee70f056809a0b2ff79fae6cf722de2cfeb95261aa38bd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff78bbd9939209b5459ddead2d5e68cdea113746073e595135cace9e852ac2bc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afaf371c77ae0674d22138365f359b4ac14ab68be729fe05c7a79e10d726b117`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 8.9 MB (8904451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efe2cca0d709017c0c09011188dd71a937d9f8b4bebc918d2715769719a2f16b`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50bd6dc1d315e6329e05543858a9c8fe102bc166e11901747897745475fa8386`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 5.4 MB (5413019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:6b8364870daa037625c5a97cca22cfda0428edadd69cb3c8a1d00dcfbd6d361a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 KB (17160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b3895d731ba30f2fc6f8e5011be07f0b49d6a34b0cbc66d53c7b5b7b11a335`

```dockerfile
```

-	Layers:
	-	`sha256:c1ddea5c446d03568ddef362b94f90e3f0eef9a1d9953f26955878608f254c4c`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 17.2 KB (17160 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:9c9e58cecb2a60d8f94969085766c8889efbf766f96f59995d5c7b98d1098ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47be3724f03dc5882cc67a78b812dd6776c63edffaba6e670d48085ce1472f7a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d37696a9b7f09eb3052928fc0b0a2bf6b1a9d8a79f15198f00b8f3d7c6f2180e`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 9.7 MB (9736559 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d528e90d2e0d255c01bbbc4d2ead9da704d8bdd46c9941f6e25e61535c53d4e0`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6afb000755ce978e9c79e6e950a600241bef0c449da1370170c9ed808493a309`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 5.6 MB (5630879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:dc9c2d5721c50d04edfdd24dff32af69861be9998efaa742fe7a60cbb6910e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.8 KB (990779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e21d3be4a225b0dee4f04888c254c8da7545ae5d64238735a130e36cf0b3ca5`

```dockerfile
```

-	Layers:
	-	`sha256:a940fbde6476c7e256b3940a1c2571f77dc47966416e58880da03224a07fc411`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 973.5 KB (973452 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:83574fc30d526c7e54ab92e98efeac06578035a04067c1ff1e80c611f8171a86`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 17.3 KB (17327 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:5e2a23003f460cd14e9bc7690c38f6cf05f8a8b254aeae4eafe9164679748305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18707567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95225b5cd25d8f282a3244a872e6e4a783f373df46a5542928d2be3a9ff4bce4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bdf85127dd33246430604be8364aad59011ec1408e05f2760d4365bd707acf5`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 10.1 MB (10083022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3884e11e9a45bef8f46aa3a109d16b19156260a3446a960d36030cda38e2c32d`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97af07dc776076badee757665cb2b7671730020e1c388a5f061fd4314ea988ab`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 5.4 MB (5405800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:05c6dcc8971095fe5681ef8bed84db1a50569df548468626288a5fcc3d2ed038
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.7 KB (990660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152c5fd0322f65eabee1d5613d5f8d91bff738d7a560de9dd19de26507b21a88`

```dockerfile
```

-	Layers:
	-	`sha256:631809d2b169208a798334a1300be704693429072ad3e80adccdcd04bd0fd3c6`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 973.4 KB (973394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7a2cc8c102e1399aff2d9b99a53977edfb5ea139a7b3ef1f0faf71a24a879f`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 17.3 KB (17266 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1-bookworm`

```console
$ docker pull irssi@sha256:9a77d1df6e590fef8eaae7ba475f2e5a9c43724bec98aff23d9b1631b9220d75
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1-bookworm` - linux; amd64

```console
$ docker pull irssi@sha256:5d9147f3379e4b79b86271b8b280d77d7b23212e3a1877b71225a508538a41c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75862383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9176b56d5f8434c83bfe4ca38d64d1fd86b07a0fd49ffe1208f4b5efa59f9fd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1eea906c30d3d0487ae55380baa41c0f4d8b8e35308aac724e9ff9bcec124642`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 18.3 MB (18260013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f0ebb89009ec7651e1ddcb8eb0a59774e42c3bc06a4b223df4b200220914da4`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54234223781082d0352cc2ea4da765bdd0ac4e5c9cc00c8081a79eced99414b9`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 28.5 MB (28473044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:19511cb18b259e0e6c94ab3fce7c9be3ba16ef514db9f61cb7a30193f7fdec1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6634888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381d2efeff58df84e748ac3cbe9d2e46d374c1cd2291648e8a039a13c5393e0`

```dockerfile
```

-	Layers:
	-	`sha256:90cbaa48e8b08df31e60931aabf94fc30837256b3c5d3ca4c4972ce0e97b7d26`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 6.6 MB (6616285 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:448eaa4bf506a9b017f8a3d2fc48ee0633391d71aa6df73781d518620d86b965`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 18.6 KB (18603 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:4286526b50c80fffe45f3d033e3fdc13e3f5c04cd6ad1ec14790c2ee8d039a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70039481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf2812ad5e9e3913d5e6e2487a3c5f13f004f7e92d10c414267119db631dba3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd87cc8398be751321cd22ca920bc62183e34f8b4b4ac4a608f07888091da0ce`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 17.0 MB (17034983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a18da79d125b945cad0e400520adaca406e8180d56d64777eac37d6b3d3a97b`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1bcc51f403f8b1d911866ad57127a5c25094f2229c92b9fe5c866e89f4c3ec4`  
		Last Modified: Wed, 20 Dec 2023 20:20:22 GMT  
		Size: 26.1 MB (26115697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:57091b62d44164148afa83ea653c4e3ece0305c5481a3c9797e4c134c4bdc593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b36f2f3830b001060929f79c17d21c3bbcf8522ec030c4585413ef64492300`

```dockerfile
```

-	Layers:
	-	`sha256:be69a9e6f839e05382bfccafc02a33265cb58de10a9d4d54c62ca261eae2ceda`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 18.3 KB (18349 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:cb8f06b471dfaa3cd90e41f16b16b6dceaa08f113006002eb02a575759530ad3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66361909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9f07d2e179897cabf0bd0385a54c12835d517ff49a2acc7e2548f54f3c529c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9af19116d503c60c4477fb97778e4d00ec874702ca31ef19d4be65bd203ce75`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 16.6 MB (16627433 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b0e896ad984d1556dc3df25f1f24d17abd4bad05bd68f1ae582f687d457ae7b`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72a4105a0adfa8587dcd54b4600d7f905af063873577b5ff9b0fca192542e045`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 25.0 MB (25012958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:bf41c4ef33d0cc113632b1d9778922afd7d5091de5188addeb1066d5b441420e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6609143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e21deee85550008b9520c1299b0e2697ab56f7d45900ae612816b74feed26d`

```dockerfile
```

-	Layers:
	-	`sha256:789bc7a90003a2b096536fa12b6be4abbef105dc07fbdd85f0ab2e91ecc6c42f`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 6.6 MB (6590579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:37d0d4185472fed8e3e965d668e307726812a2cd1b7543b76085eef8c33e4318`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 18.6 KB (18564 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:4448d99fff66a402267a1326cf56befb11179adc9a588d74d9d232ac6896d13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74613777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6be87e358baeb4ebdb34e1b0bf058728b4c9b4791df705a97af2459aa4b112`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:560bf72e987fd6edd06c8b56f9b1566b5262ee2c254adf3863299dd47c78fa92`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 18.0 MB (18021745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:980da2332d71ffeb3fb18a84dbd721f5c4a52f7dee942f6e1d8e85713a3890cc`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d851282e78a89fab2fca7d86db4275a5e68bb52ea170ef151be24211ee1ea9f`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 27.4 MB (27431401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:51ef1e0b32d9b59ab96443e4f12015237b4289ae8365567cc267e8be313328b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6615458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae12ce93fbd3b325957885cb40c6582cd97d4d8fe0e69b96b92e469e333a84b`

```dockerfile
```

-	Layers:
	-	`sha256:e31580db9e488826eb1086346c8be3366de013ebbcd231d60ced6faca6d545ea`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 6.6 MB (6597004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1fdc10f0e5fa4cb00a3930219cf8bf8c5ea4d37cb721a83bc8eb8006e95dec45`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 18.5 KB (18454 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:6a8475ff3c12f74fc70976a5161b3fe205b5de6af186234af5f1b589963f5412
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76291252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bd0be5ca51091c547885af81aa5f9ce44a235139086622e3a6cc4425f42abb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f7dc5be6fb0db696a5c82ed11d73cbf826f8b763876f18c25833f1ac9db5a9e`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 17.8 MB (17785994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb9836a268b33d7bfd41001911da5ce8ade91fd68ae9ad1ad4a1444f46d5c802`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc2f90db82b28b52fb5cc5805f4a587ece1c5d91add681edbab73eb99d5829c5`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 28.4 MB (28358032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:ca9217a9d59d109bd6ab0e81c9843708540d923c98f8f4089a0203337f0fb516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9feee74d3925e1773ca2cbdd6daa9468885e693129cf04d99d2b862d2ded7f`

```dockerfile
```

-	Layers:
	-	`sha256:f528901de35025479bc79bcbdceac123bb7b194efcd16d5831474114de792022`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 18.3 KB (18335 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:8cbeb7cfde7d32b8433e1c01c415fbd6ad8fa9cd259edd4313c1182a978eac09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74063255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b791cfba3e8bc5162ca9521ffdbb0820710918bc04a13a33e6f8be224f55438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:13:36 GMT
ADD file:dcd5696ac281b24df52a518e2402c7f7a4caedfcba0d82e195b7c06cd3a38fdd in / 
# Tue, 19 Dec 2023 02:13:40 GMT
CMD ["bash"]
# Wed, 20 Dec 2023 13:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Dec 2023 13:30:09 GMT
ENV HOME=/home/user
# Wed, 20 Dec 2023 13:30:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Dec 2023 13:30:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 13:30:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 20 Dec 2023 13:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Dec 2023 13:34:25 GMT
WORKDIR /home/user
# Wed, 20 Dec 2023 13:34:29 GMT
USER user
# Wed, 20 Dec 2023 13:34:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:12b1322ffb17b8e81ca1c6d9d7118e2fcee0b9d971aa3c90601e6345804a60d1`  
		Last Modified: Tue, 19 Dec 2023 02:24:36 GMT  
		Size: 29.1 MB (29121427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ad670e672d195ec763bd204f894d09cdc183c6ce311eba2ffc439612121ee`  
		Last Modified: Wed, 20 Dec 2023 13:35:14 GMT  
		Size: 16.9 MB (16929535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb1cb4c20719f053a8b365e7ae8908e7f3fc0b57887a9c01af2cff96600f8e7`  
		Last Modified: Wed, 20 Dec 2023 13:34:58 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fabfead7d49f06de8058ccfeab86b5aee8284be57ed979452324699df85abd1`  
		Last Modified: Wed, 20 Dec 2023 13:35:19 GMT  
		Size: 28.0 MB (28008995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:575ef209f28f4f7ed0a9a7b1c99df2bb2f87cd950a7977188d8be9408323b055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81858507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e1e484a868196a76e57f555fecc46159723e455f87f03731192a645f49205e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c6980c5acfb61420bec3fecb79e92baf26848104c2f1a8cf0d1754bca2bac3e`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 18.8 MB (18757646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:765deb34181ae86766afbb92b8adb60ed2d09436f8b805be2169b2f85c496f0b`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:622166be7f78a644c3966afdbc21cd1d72d5b61221fc50ec222cc6ff1bef82aa`  
		Last Modified: Wed, 20 Dec 2023 21:08:23 GMT  
		Size: 30.0 MB (29976941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:1afc854d3abba98f2eb32986720d792629f71ee99d2d03d0f7c005f41125ae57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6627152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4510d937df9c77199f03f2ffc9c0d973e60235ae776b09cd1ddf79d983389`

```dockerfile
```

-	Layers:
	-	`sha256:8f0991cfc927c50f1f4496eb5371bc577a375f262aebd9f969e6fc90aa5b4f27`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 6.6 MB (6608650 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7204444fbb4c105206ab3f29c0589fc495706f2d07570acbc522140d7a09eb4d`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 18.5 KB (18502 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:60a482b86f2db7fd10d491938f31901c7f6adbac8c2463cb2e2fa62c3c30cf5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72724499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1a2b7df92545b5f83cf7c3dc5f7a38e9573ef5035b06654c733958586e67e7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0caafde47a3e9a6dd324ed419bf5fbf3927b27845c745b95d9c37e1bb7d63a8`  
		Last Modified: Wed, 20 Dec 2023 21:18:34 GMT  
		Size: 18.2 MB (18207265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3d931210f84c8b8a6fbeae35b4a75acad3d2255b470db4a1a421d40c38e2abc`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a383a09d5e97936abef74784a8ef9413735c27dd1a73de75fd3fe595c5719fd`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 27.0 MB (27021999 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:f49bf849702833ecb1a8740440767542d2c5b9980182fde5e48de04801a43a0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6623640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ed98bb6c8dc6a0f89cdc2d7b3d5386486f3daadbfdf2b7237d3bfe0fcbeb41`

```dockerfile
```

-	Layers:
	-	`sha256:65127003855e314eb1d3819c53d0fbe07edefc65c019685ffaaed55b5556af43`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 6.6 MB (6605204 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:055af2286d41963c455bd993dbb42a317414c6a8b4b231e164463af193d45837`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 18.4 KB (18436 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1.4`

```console
$ docker pull irssi@sha256:9a77d1df6e590fef8eaae7ba475f2e5a9c43724bec98aff23d9b1631b9220d75
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1.4` - linux; amd64

```console
$ docker pull irssi@sha256:5d9147f3379e4b79b86271b8b280d77d7b23212e3a1877b71225a508538a41c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75862383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9176b56d5f8434c83bfe4ca38d64d1fd86b07a0fd49ffe1208f4b5efa59f9fd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1eea906c30d3d0487ae55380baa41c0f4d8b8e35308aac724e9ff9bcec124642`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 18.3 MB (18260013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f0ebb89009ec7651e1ddcb8eb0a59774e42c3bc06a4b223df4b200220914da4`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54234223781082d0352cc2ea4da765bdd0ac4e5c9cc00c8081a79eced99414b9`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 28.5 MB (28473044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4` - unknown; unknown

```console
$ docker pull irssi@sha256:19511cb18b259e0e6c94ab3fce7c9be3ba16ef514db9f61cb7a30193f7fdec1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6634888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381d2efeff58df84e748ac3cbe9d2e46d374c1cd2291648e8a039a13c5393e0`

```dockerfile
```

-	Layers:
	-	`sha256:90cbaa48e8b08df31e60931aabf94fc30837256b3c5d3ca4c4972ce0e97b7d26`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 6.6 MB (6616285 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:448eaa4bf506a9b017f8a3d2fc48ee0633391d71aa6df73781d518620d86b965`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 18.6 KB (18603 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4` - linux; arm variant v5

```console
$ docker pull irssi@sha256:4286526b50c80fffe45f3d033e3fdc13e3f5c04cd6ad1ec14790c2ee8d039a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70039481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf2812ad5e9e3913d5e6e2487a3c5f13f004f7e92d10c414267119db631dba3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd87cc8398be751321cd22ca920bc62183e34f8b4b4ac4a608f07888091da0ce`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 17.0 MB (17034983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a18da79d125b945cad0e400520adaca406e8180d56d64777eac37d6b3d3a97b`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1bcc51f403f8b1d911866ad57127a5c25094f2229c92b9fe5c866e89f4c3ec4`  
		Last Modified: Wed, 20 Dec 2023 20:20:22 GMT  
		Size: 26.1 MB (26115697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4` - unknown; unknown

```console
$ docker pull irssi@sha256:57091b62d44164148afa83ea653c4e3ece0305c5481a3c9797e4c134c4bdc593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b36f2f3830b001060929f79c17d21c3bbcf8522ec030c4585413ef64492300`

```dockerfile
```

-	Layers:
	-	`sha256:be69a9e6f839e05382bfccafc02a33265cb58de10a9d4d54c62ca261eae2ceda`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 18.3 KB (18349 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4` - linux; arm variant v7

```console
$ docker pull irssi@sha256:cb8f06b471dfaa3cd90e41f16b16b6dceaa08f113006002eb02a575759530ad3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66361909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9f07d2e179897cabf0bd0385a54c12835d517ff49a2acc7e2548f54f3c529c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9af19116d503c60c4477fb97778e4d00ec874702ca31ef19d4be65bd203ce75`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 16.6 MB (16627433 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b0e896ad984d1556dc3df25f1f24d17abd4bad05bd68f1ae582f687d457ae7b`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72a4105a0adfa8587dcd54b4600d7f905af063873577b5ff9b0fca192542e045`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 25.0 MB (25012958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4` - unknown; unknown

```console
$ docker pull irssi@sha256:bf41c4ef33d0cc113632b1d9778922afd7d5091de5188addeb1066d5b441420e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6609143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e21deee85550008b9520c1299b0e2697ab56f7d45900ae612816b74feed26d`

```dockerfile
```

-	Layers:
	-	`sha256:789bc7a90003a2b096536fa12b6be4abbef105dc07fbdd85f0ab2e91ecc6c42f`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 6.6 MB (6590579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:37d0d4185472fed8e3e965d668e307726812a2cd1b7543b76085eef8c33e4318`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 18.6 KB (18564 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:4448d99fff66a402267a1326cf56befb11179adc9a588d74d9d232ac6896d13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74613777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6be87e358baeb4ebdb34e1b0bf058728b4c9b4791df705a97af2459aa4b112`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:560bf72e987fd6edd06c8b56f9b1566b5262ee2c254adf3863299dd47c78fa92`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 18.0 MB (18021745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:980da2332d71ffeb3fb18a84dbd721f5c4a52f7dee942f6e1d8e85713a3890cc`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d851282e78a89fab2fca7d86db4275a5e68bb52ea170ef151be24211ee1ea9f`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 27.4 MB (27431401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4` - unknown; unknown

```console
$ docker pull irssi@sha256:51ef1e0b32d9b59ab96443e4f12015237b4289ae8365567cc267e8be313328b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6615458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae12ce93fbd3b325957885cb40c6582cd97d4d8fe0e69b96b92e469e333a84b`

```dockerfile
```

-	Layers:
	-	`sha256:e31580db9e488826eb1086346c8be3366de013ebbcd231d60ced6faca6d545ea`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 6.6 MB (6597004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1fdc10f0e5fa4cb00a3930219cf8bf8c5ea4d37cb721a83bc8eb8006e95dec45`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 18.5 KB (18454 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4` - linux; 386

```console
$ docker pull irssi@sha256:6a8475ff3c12f74fc70976a5161b3fe205b5de6af186234af5f1b589963f5412
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76291252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bd0be5ca51091c547885af81aa5f9ce44a235139086622e3a6cc4425f42abb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f7dc5be6fb0db696a5c82ed11d73cbf826f8b763876f18c25833f1ac9db5a9e`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 17.8 MB (17785994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb9836a268b33d7bfd41001911da5ce8ade91fd68ae9ad1ad4a1444f46d5c802`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc2f90db82b28b52fb5cc5805f4a587ece1c5d91add681edbab73eb99d5829c5`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 28.4 MB (28358032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4` - unknown; unknown

```console
$ docker pull irssi@sha256:ca9217a9d59d109bd6ab0e81c9843708540d923c98f8f4089a0203337f0fb516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9feee74d3925e1773ca2cbdd6daa9468885e693129cf04d99d2b862d2ded7f`

```dockerfile
```

-	Layers:
	-	`sha256:f528901de35025479bc79bcbdceac123bb7b194efcd16d5831474114de792022`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 18.3 KB (18335 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4` - linux; mips64le

```console
$ docker pull irssi@sha256:8cbeb7cfde7d32b8433e1c01c415fbd6ad8fa9cd259edd4313c1182a978eac09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74063255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b791cfba3e8bc5162ca9521ffdbb0820710918bc04a13a33e6f8be224f55438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:13:36 GMT
ADD file:dcd5696ac281b24df52a518e2402c7f7a4caedfcba0d82e195b7c06cd3a38fdd in / 
# Tue, 19 Dec 2023 02:13:40 GMT
CMD ["bash"]
# Wed, 20 Dec 2023 13:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Dec 2023 13:30:09 GMT
ENV HOME=/home/user
# Wed, 20 Dec 2023 13:30:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Dec 2023 13:30:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 13:30:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 20 Dec 2023 13:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Dec 2023 13:34:25 GMT
WORKDIR /home/user
# Wed, 20 Dec 2023 13:34:29 GMT
USER user
# Wed, 20 Dec 2023 13:34:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:12b1322ffb17b8e81ca1c6d9d7118e2fcee0b9d971aa3c90601e6345804a60d1`  
		Last Modified: Tue, 19 Dec 2023 02:24:36 GMT  
		Size: 29.1 MB (29121427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ad670e672d195ec763bd204f894d09cdc183c6ce311eba2ffc439612121ee`  
		Last Modified: Wed, 20 Dec 2023 13:35:14 GMT  
		Size: 16.9 MB (16929535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb1cb4c20719f053a8b365e7ae8908e7f3fc0b57887a9c01af2cff96600f8e7`  
		Last Modified: Wed, 20 Dec 2023 13:34:58 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fabfead7d49f06de8058ccfeab86b5aee8284be57ed979452324699df85abd1`  
		Last Modified: Wed, 20 Dec 2023 13:35:19 GMT  
		Size: 28.0 MB (28008995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4` - linux; ppc64le

```console
$ docker pull irssi@sha256:575ef209f28f4f7ed0a9a7b1c99df2bb2f87cd950a7977188d8be9408323b055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81858507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e1e484a868196a76e57f555fecc46159723e455f87f03731192a645f49205e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c6980c5acfb61420bec3fecb79e92baf26848104c2f1a8cf0d1754bca2bac3e`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 18.8 MB (18757646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:765deb34181ae86766afbb92b8adb60ed2d09436f8b805be2169b2f85c496f0b`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:622166be7f78a644c3966afdbc21cd1d72d5b61221fc50ec222cc6ff1bef82aa`  
		Last Modified: Wed, 20 Dec 2023 21:08:23 GMT  
		Size: 30.0 MB (29976941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4` - unknown; unknown

```console
$ docker pull irssi@sha256:1afc854d3abba98f2eb32986720d792629f71ee99d2d03d0f7c005f41125ae57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6627152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4510d937df9c77199f03f2ffc9c0d973e60235ae776b09cd1ddf79d983389`

```dockerfile
```

-	Layers:
	-	`sha256:8f0991cfc927c50f1f4496eb5371bc577a375f262aebd9f969e6fc90aa5b4f27`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 6.6 MB (6608650 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7204444fbb4c105206ab3f29c0589fc495706f2d07570acbc522140d7a09eb4d`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 18.5 KB (18502 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4` - linux; s390x

```console
$ docker pull irssi@sha256:60a482b86f2db7fd10d491938f31901c7f6adbac8c2463cb2e2fa62c3c30cf5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72724499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1a2b7df92545b5f83cf7c3dc5f7a38e9573ef5035b06654c733958586e67e7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0caafde47a3e9a6dd324ed419bf5fbf3927b27845c745b95d9c37e1bb7d63a8`  
		Last Modified: Wed, 20 Dec 2023 21:18:34 GMT  
		Size: 18.2 MB (18207265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3d931210f84c8b8a6fbeae35b4a75acad3d2255b470db4a1a421d40c38e2abc`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a383a09d5e97936abef74784a8ef9413735c27dd1a73de75fd3fe595c5719fd`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 27.0 MB (27021999 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4` - unknown; unknown

```console
$ docker pull irssi@sha256:f49bf849702833ecb1a8740440767542d2c5b9980182fde5e48de04801a43a0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6623640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ed98bb6c8dc6a0f89cdc2d7b3d5386486f3daadbfdf2b7237d3bfe0fcbeb41`

```dockerfile
```

-	Layers:
	-	`sha256:65127003855e314eb1d3819c53d0fbe07edefc65c019685ffaaed55b5556af43`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 6.6 MB (6605204 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:055af2286d41963c455bd993dbb42a317414c6a8b4b231e164463af193d45837`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 18.4 KB (18436 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1.4-alpine`

```console
$ docker pull irssi@sha256:79451b25b3472ba9e2eaea3b2ac29fe6fe096d29e2c8906f5bc613d00d0aa5f5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1.4-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:105fa5e67e4e73efc68a46251ccc88bcdd20c1f00791c024d72049ec8c262192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90a1bb4955c1fa1c41936729e39aea9920194ea59a1c610b1a3403c3f0c6150`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e0489114318ebbbb358ac5d32aee84c3a4b5533810fa6706b0648de63eada38`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 9.6 MB (9645476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdf0d195e7f83acc9eedf0071d583bf6af6349889841e7635cf29c43c629c640`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d108ad9c820b6d6e8e249ebc6d8880815c65c45f26892e8a6ab3c9ae45685853`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 5.4 MB (5402203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:d20bcdc49a8bcf8dc91e15bca6c781ebcd7c4dc4198b20d4e313fc2c9c439bee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.5 KB (992458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb852ef521ea46c7682f4f7119f23851f36317e79cce4556e2e9e416fbde2cf`

```dockerfile
```

-	Layers:
	-	`sha256:4cd7f1f45cebca0db6e6b84a0d40d4291bd1884fe3a99cd8699e1f85cc855931`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 975.0 KB (975030 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc7b354d55ff368937c54932656d0c6e35d054544cd811ae952e5339e561af61`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 17.4 KB (17428 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:502678281e0a8fc11e5e60ab54cf7dd84c2ee569f3f870ef4adcaab298fb417b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17270398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899b60c73aa2cd976bff10c64aadf2960af1ce82aa7137f963033a1c8a9e01ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410e5270be4aa0f019d84c2b63359fe74822bbb5d0b839fe7016fc64dfbc7ae0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 8.9 MB (8880076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1571fb6473dae031bdc723dcc05df8bcedb8e7949fe43e60b88b84d28de6359`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c99573a422ea748e601e3fc5a3c7147a082b13fa4b63b41d7410e26fe7185d0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 5.2 MB (5242159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:464a826b2af15230d1a2d27c265fe0c4cdfa1911cc91aa09aea53ed9cfba65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 KB (17341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9858ff23fdfea20d8cc88ee6f6d49900d4a8b83f719dc1bbab498204aa70e95b`

```dockerfile
```

-	Layers:
	-	`sha256:c698656fcb6933453517855d73664fa233a7df879ad29c65c2c7e6c9bd6af2b1`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 17.3 KB (17341 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:781db50a278b2665670bc3112c5c0397014ab37ff3c9f3d9a515449d00407b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5613a41dc765b890dc98b0f1b3c5ff9a53edd2e1445eb87311c9fc626682efe9`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:831415ea41c64b7ebb180f4f1da27bcf8dff3a9c5857deefa938de6334bc05c8`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 8.7 MB (8721217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95002d0dfc5013bc236502c1d58e95122a36e7ced9325e458f87721e74424053`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfcc5163f111398aff0073ad800b7fe8d98fa110ae443c658242fe5979989243`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 5.0 MB (5006513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:80029ca5ee21b65a87e5bffcd0f6e982ab1939bd3a2fd22627ae42ed2677e9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **995.0 KB (994964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be9e8234e96256b98972c25f2a33d5b2f9af93030aa1c99e11688eec589a33`

```dockerfile
```

-	Layers:
	-	`sha256:647518d13f1ec703d0cc9f34b31e2b53de88cb2616b0cb39b44211edcd1de409`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 977.6 KB (977574 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:76183270a354928c61dc0a73762989852386c1f766eb7a8a6f5773870e87ad5f`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 17.4 KB (17390 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9231eee1fd711f485f49771ef585253227fe5803335d2301087e2cb083f099a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18315846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4729d538632dda020f3bcd9bae8a2249d9cad5ae76a8f02f431fc37137c71a14`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86f46af68b50326d6225714f933de969fae879fd66189bbd1edbda8e47ab9343`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 9.7 MB (9673040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183fe6397c74bb1e7159b0a06eebe92da8dbd1b6af699e543a7618777a0bf315`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e28fc2012c204a8e8b903e0d3b7a042e4d5c0867e2e9eeb2340b29cd64ee66f`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 5.3 MB (5308483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:1c785db37c195270ba3ac1385d0509431549621d5ef5ef558ba9c4c1efa77e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.3 KB (992329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5548d8fc5c59a6fd473580a6b28b02ec1f638378bf3a473bf92331dc86e4db05`

```dockerfile
```

-	Layers:
	-	`sha256:90fad57a08e8809e193e2d976c2a6a59a19c5aaaba7933737ca575c34031f786`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 975.0 KB (975049 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:833e49bd915ced6aed85ab32c68fdbcc2809eac8f325ae4d6054353f2b8c1831`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 17.3 KB (17280 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine` - linux; 386

```console
$ docker pull irssi@sha256:a1f46da9d4d08c6ee70f056809a0b2ff79fae6cf722de2cfeb95261aa38bd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff78bbd9939209b5459ddead2d5e68cdea113746073e595135cace9e852ac2bc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afaf371c77ae0674d22138365f359b4ac14ab68be729fe05c7a79e10d726b117`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 8.9 MB (8904451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efe2cca0d709017c0c09011188dd71a937d9f8b4bebc918d2715769719a2f16b`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50bd6dc1d315e6329e05543858a9c8fe102bc166e11901747897745475fa8386`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 5.4 MB (5413019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:6b8364870daa037625c5a97cca22cfda0428edadd69cb3c8a1d00dcfbd6d361a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 KB (17160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b3895d731ba30f2fc6f8e5011be07f0b49d6a34b0cbc66d53c7b5b7b11a335`

```dockerfile
```

-	Layers:
	-	`sha256:c1ddea5c446d03568ddef362b94f90e3f0eef9a1d9953f26955878608f254c4c`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 17.2 KB (17160 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:9c9e58cecb2a60d8f94969085766c8889efbf766f96f59995d5c7b98d1098ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47be3724f03dc5882cc67a78b812dd6776c63edffaba6e670d48085ce1472f7a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d37696a9b7f09eb3052928fc0b0a2bf6b1a9d8a79f15198f00b8f3d7c6f2180e`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 9.7 MB (9736559 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d528e90d2e0d255c01bbbc4d2ead9da704d8bdd46c9941f6e25e61535c53d4e0`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6afb000755ce978e9c79e6e950a600241bef0c449da1370170c9ed808493a309`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 5.6 MB (5630879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:dc9c2d5721c50d04edfdd24dff32af69861be9998efaa742fe7a60cbb6910e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.8 KB (990779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e21d3be4a225b0dee4f04888c254c8da7545ae5d64238735a130e36cf0b3ca5`

```dockerfile
```

-	Layers:
	-	`sha256:a940fbde6476c7e256b3940a1c2571f77dc47966416e58880da03224a07fc411`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 973.5 KB (973452 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:83574fc30d526c7e54ab92e98efeac06578035a04067c1ff1e80c611f8171a86`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 17.3 KB (17327 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:5e2a23003f460cd14e9bc7690c38f6cf05f8a8b254aeae4eafe9164679748305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18707567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95225b5cd25d8f282a3244a872e6e4a783f373df46a5542928d2be3a9ff4bce4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bdf85127dd33246430604be8364aad59011ec1408e05f2760d4365bd707acf5`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 10.1 MB (10083022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3884e11e9a45bef8f46aa3a109d16b19156260a3446a960d36030cda38e2c32d`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97af07dc776076badee757665cb2b7671730020e1c388a5f061fd4314ea988ab`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 5.4 MB (5405800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:05c6dcc8971095fe5681ef8bed84db1a50569df548468626288a5fcc3d2ed038
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.7 KB (990660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152c5fd0322f65eabee1d5613d5f8d91bff738d7a560de9dd19de26507b21a88`

```dockerfile
```

-	Layers:
	-	`sha256:631809d2b169208a798334a1300be704693429072ad3e80adccdcd04bd0fd3c6`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 973.4 KB (973394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7a2cc8c102e1399aff2d9b99a53977edfb5ea139a7b3ef1f0faf71a24a879f`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 17.3 KB (17266 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1.4-alpine3.18`

```console
$ docker pull irssi@sha256:79451b25b3472ba9e2eaea3b2ac29fe6fe096d29e2c8906f5bc613d00d0aa5f5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1.4-alpine3.18` - linux; amd64

```console
$ docker pull irssi@sha256:105fa5e67e4e73efc68a46251ccc88bcdd20c1f00791c024d72049ec8c262192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90a1bb4955c1fa1c41936729e39aea9920194ea59a1c610b1a3403c3f0c6150`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e0489114318ebbbb358ac5d32aee84c3a4b5533810fa6706b0648de63eada38`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 9.6 MB (9645476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdf0d195e7f83acc9eedf0071d583bf6af6349889841e7635cf29c43c629c640`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d108ad9c820b6d6e8e249ebc6d8880815c65c45f26892e8a6ab3c9ae45685853`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 5.4 MB (5402203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:d20bcdc49a8bcf8dc91e15bca6c781ebcd7c4dc4198b20d4e313fc2c9c439bee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.5 KB (992458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb852ef521ea46c7682f4f7119f23851f36317e79cce4556e2e9e416fbde2cf`

```dockerfile
```

-	Layers:
	-	`sha256:4cd7f1f45cebca0db6e6b84a0d40d4291bd1884fe3a99cd8699e1f85cc855931`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 975.0 KB (975030 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc7b354d55ff368937c54932656d0c6e35d054544cd811ae952e5339e561af61`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 17.4 KB (17428 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:502678281e0a8fc11e5e60ab54cf7dd84c2ee569f3f870ef4adcaab298fb417b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17270398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899b60c73aa2cd976bff10c64aadf2960af1ce82aa7137f963033a1c8a9e01ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410e5270be4aa0f019d84c2b63359fe74822bbb5d0b839fe7016fc64dfbc7ae0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 8.9 MB (8880076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1571fb6473dae031bdc723dcc05df8bcedb8e7949fe43e60b88b84d28de6359`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c99573a422ea748e601e3fc5a3c7147a082b13fa4b63b41d7410e26fe7185d0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 5.2 MB (5242159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:464a826b2af15230d1a2d27c265fe0c4cdfa1911cc91aa09aea53ed9cfba65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 KB (17341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9858ff23fdfea20d8cc88ee6f6d49900d4a8b83f719dc1bbab498204aa70e95b`

```dockerfile
```

-	Layers:
	-	`sha256:c698656fcb6933453517855d73664fa233a7df879ad29c65c2c7e6c9bd6af2b1`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 17.3 KB (17341 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:781db50a278b2665670bc3112c5c0397014ab37ff3c9f3d9a515449d00407b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5613a41dc765b890dc98b0f1b3c5ff9a53edd2e1445eb87311c9fc626682efe9`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:831415ea41c64b7ebb180f4f1da27bcf8dff3a9c5857deefa938de6334bc05c8`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 8.7 MB (8721217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95002d0dfc5013bc236502c1d58e95122a36e7ced9325e458f87721e74424053`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfcc5163f111398aff0073ad800b7fe8d98fa110ae443c658242fe5979989243`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 5.0 MB (5006513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:80029ca5ee21b65a87e5bffcd0f6e982ab1939bd3a2fd22627ae42ed2677e9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **995.0 KB (994964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be9e8234e96256b98972c25f2a33d5b2f9af93030aa1c99e11688eec589a33`

```dockerfile
```

-	Layers:
	-	`sha256:647518d13f1ec703d0cc9f34b31e2b53de88cb2616b0cb39b44211edcd1de409`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 977.6 KB (977574 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:76183270a354928c61dc0a73762989852386c1f766eb7a8a6f5773870e87ad5f`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 17.4 KB (17390 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9231eee1fd711f485f49771ef585253227fe5803335d2301087e2cb083f099a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18315846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4729d538632dda020f3bcd9bae8a2249d9cad5ae76a8f02f431fc37137c71a14`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86f46af68b50326d6225714f933de969fae879fd66189bbd1edbda8e47ab9343`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 9.7 MB (9673040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183fe6397c74bb1e7159b0a06eebe92da8dbd1b6af699e543a7618777a0bf315`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e28fc2012c204a8e8b903e0d3b7a042e4d5c0867e2e9eeb2340b29cd64ee66f`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 5.3 MB (5308483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:1c785db37c195270ba3ac1385d0509431549621d5ef5ef558ba9c4c1efa77e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.3 KB (992329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5548d8fc5c59a6fd473580a6b28b02ec1f638378bf3a473bf92331dc86e4db05`

```dockerfile
```

-	Layers:
	-	`sha256:90fad57a08e8809e193e2d976c2a6a59a19c5aaaba7933737ca575c34031f786`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 975.0 KB (975049 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:833e49bd915ced6aed85ab32c68fdbcc2809eac8f325ae4d6054353f2b8c1831`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 17.3 KB (17280 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:a1f46da9d4d08c6ee70f056809a0b2ff79fae6cf722de2cfeb95261aa38bd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff78bbd9939209b5459ddead2d5e68cdea113746073e595135cace9e852ac2bc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afaf371c77ae0674d22138365f359b4ac14ab68be729fe05c7a79e10d726b117`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 8.9 MB (8904451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efe2cca0d709017c0c09011188dd71a937d9f8b4bebc918d2715769719a2f16b`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50bd6dc1d315e6329e05543858a9c8fe102bc166e11901747897745475fa8386`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 5.4 MB (5413019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:6b8364870daa037625c5a97cca22cfda0428edadd69cb3c8a1d00dcfbd6d361a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 KB (17160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b3895d731ba30f2fc6f8e5011be07f0b49d6a34b0cbc66d53c7b5b7b11a335`

```dockerfile
```

-	Layers:
	-	`sha256:c1ddea5c446d03568ddef362b94f90e3f0eef9a1d9953f26955878608f254c4c`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 17.2 KB (17160 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:9c9e58cecb2a60d8f94969085766c8889efbf766f96f59995d5c7b98d1098ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47be3724f03dc5882cc67a78b812dd6776c63edffaba6e670d48085ce1472f7a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d37696a9b7f09eb3052928fc0b0a2bf6b1a9d8a79f15198f00b8f3d7c6f2180e`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 9.7 MB (9736559 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d528e90d2e0d255c01bbbc4d2ead9da704d8bdd46c9941f6e25e61535c53d4e0`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6afb000755ce978e9c79e6e950a600241bef0c449da1370170c9ed808493a309`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 5.6 MB (5630879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:dc9c2d5721c50d04edfdd24dff32af69861be9998efaa742fe7a60cbb6910e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.8 KB (990779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e21d3be4a225b0dee4f04888c254c8da7545ae5d64238735a130e36cf0b3ca5`

```dockerfile
```

-	Layers:
	-	`sha256:a940fbde6476c7e256b3940a1c2571f77dc47966416e58880da03224a07fc411`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 973.5 KB (973452 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:83574fc30d526c7e54ab92e98efeac06578035a04067c1ff1e80c611f8171a86`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 17.3 KB (17327 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:5e2a23003f460cd14e9bc7690c38f6cf05f8a8b254aeae4eafe9164679748305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18707567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95225b5cd25d8f282a3244a872e6e4a783f373df46a5542928d2be3a9ff4bce4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bdf85127dd33246430604be8364aad59011ec1408e05f2760d4365bd707acf5`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 10.1 MB (10083022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3884e11e9a45bef8f46aa3a109d16b19156260a3446a960d36030cda38e2c32d`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97af07dc776076badee757665cb2b7671730020e1c388a5f061fd4314ea988ab`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 5.4 MB (5405800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:05c6dcc8971095fe5681ef8bed84db1a50569df548468626288a5fcc3d2ed038
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.7 KB (990660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152c5fd0322f65eabee1d5613d5f8d91bff738d7a560de9dd19de26507b21a88`

```dockerfile
```

-	Layers:
	-	`sha256:631809d2b169208a798334a1300be704693429072ad3e80adccdcd04bd0fd3c6`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 973.4 KB (973394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7a2cc8c102e1399aff2d9b99a53977edfb5ea139a7b3ef1f0faf71a24a879f`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 17.3 KB (17266 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1.4-bookworm`

```console
$ docker pull irssi@sha256:9a77d1df6e590fef8eaae7ba475f2e5a9c43724bec98aff23d9b1631b9220d75
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1.4-bookworm` - linux; amd64

```console
$ docker pull irssi@sha256:5d9147f3379e4b79b86271b8b280d77d7b23212e3a1877b71225a508538a41c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75862383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9176b56d5f8434c83bfe4ca38d64d1fd86b07a0fd49ffe1208f4b5efa59f9fd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1eea906c30d3d0487ae55380baa41c0f4d8b8e35308aac724e9ff9bcec124642`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 18.3 MB (18260013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f0ebb89009ec7651e1ddcb8eb0a59774e42c3bc06a4b223df4b200220914da4`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54234223781082d0352cc2ea4da765bdd0ac4e5c9cc00c8081a79eced99414b9`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 28.5 MB (28473044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:19511cb18b259e0e6c94ab3fce7c9be3ba16ef514db9f61cb7a30193f7fdec1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6634888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381d2efeff58df84e748ac3cbe9d2e46d374c1cd2291648e8a039a13c5393e0`

```dockerfile
```

-	Layers:
	-	`sha256:90cbaa48e8b08df31e60931aabf94fc30837256b3c5d3ca4c4972ce0e97b7d26`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 6.6 MB (6616285 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:448eaa4bf506a9b017f8a3d2fc48ee0633391d71aa6df73781d518620d86b965`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 18.6 KB (18603 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:4286526b50c80fffe45f3d033e3fdc13e3f5c04cd6ad1ec14790c2ee8d039a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70039481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf2812ad5e9e3913d5e6e2487a3c5f13f004f7e92d10c414267119db631dba3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd87cc8398be751321cd22ca920bc62183e34f8b4b4ac4a608f07888091da0ce`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 17.0 MB (17034983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a18da79d125b945cad0e400520adaca406e8180d56d64777eac37d6b3d3a97b`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1bcc51f403f8b1d911866ad57127a5c25094f2229c92b9fe5c866e89f4c3ec4`  
		Last Modified: Wed, 20 Dec 2023 20:20:22 GMT  
		Size: 26.1 MB (26115697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:57091b62d44164148afa83ea653c4e3ece0305c5481a3c9797e4c134c4bdc593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b36f2f3830b001060929f79c17d21c3bbcf8522ec030c4585413ef64492300`

```dockerfile
```

-	Layers:
	-	`sha256:be69a9e6f839e05382bfccafc02a33265cb58de10a9d4d54c62ca261eae2ceda`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 18.3 KB (18349 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:cb8f06b471dfaa3cd90e41f16b16b6dceaa08f113006002eb02a575759530ad3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66361909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9f07d2e179897cabf0bd0385a54c12835d517ff49a2acc7e2548f54f3c529c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9af19116d503c60c4477fb97778e4d00ec874702ca31ef19d4be65bd203ce75`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 16.6 MB (16627433 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b0e896ad984d1556dc3df25f1f24d17abd4bad05bd68f1ae582f687d457ae7b`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72a4105a0adfa8587dcd54b4600d7f905af063873577b5ff9b0fca192542e045`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 25.0 MB (25012958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:bf41c4ef33d0cc113632b1d9778922afd7d5091de5188addeb1066d5b441420e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6609143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e21deee85550008b9520c1299b0e2697ab56f7d45900ae612816b74feed26d`

```dockerfile
```

-	Layers:
	-	`sha256:789bc7a90003a2b096536fa12b6be4abbef105dc07fbdd85f0ab2e91ecc6c42f`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 6.6 MB (6590579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:37d0d4185472fed8e3e965d668e307726812a2cd1b7543b76085eef8c33e4318`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 18.6 KB (18564 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:4448d99fff66a402267a1326cf56befb11179adc9a588d74d9d232ac6896d13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74613777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6be87e358baeb4ebdb34e1b0bf058728b4c9b4791df705a97af2459aa4b112`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:560bf72e987fd6edd06c8b56f9b1566b5262ee2c254adf3863299dd47c78fa92`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 18.0 MB (18021745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:980da2332d71ffeb3fb18a84dbd721f5c4a52f7dee942f6e1d8e85713a3890cc`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d851282e78a89fab2fca7d86db4275a5e68bb52ea170ef151be24211ee1ea9f`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 27.4 MB (27431401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:51ef1e0b32d9b59ab96443e4f12015237b4289ae8365567cc267e8be313328b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6615458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae12ce93fbd3b325957885cb40c6582cd97d4d8fe0e69b96b92e469e333a84b`

```dockerfile
```

-	Layers:
	-	`sha256:e31580db9e488826eb1086346c8be3366de013ebbcd231d60ced6faca6d545ea`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 6.6 MB (6597004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1fdc10f0e5fa4cb00a3930219cf8bf8c5ea4d37cb721a83bc8eb8006e95dec45`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 18.5 KB (18454 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:6a8475ff3c12f74fc70976a5161b3fe205b5de6af186234af5f1b589963f5412
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76291252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bd0be5ca51091c547885af81aa5f9ce44a235139086622e3a6cc4425f42abb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f7dc5be6fb0db696a5c82ed11d73cbf826f8b763876f18c25833f1ac9db5a9e`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 17.8 MB (17785994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb9836a268b33d7bfd41001911da5ce8ade91fd68ae9ad1ad4a1444f46d5c802`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc2f90db82b28b52fb5cc5805f4a587ece1c5d91add681edbab73eb99d5829c5`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 28.4 MB (28358032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:ca9217a9d59d109bd6ab0e81c9843708540d923c98f8f4089a0203337f0fb516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9feee74d3925e1773ca2cbdd6daa9468885e693129cf04d99d2b862d2ded7f`

```dockerfile
```

-	Layers:
	-	`sha256:f528901de35025479bc79bcbdceac123bb7b194efcd16d5831474114de792022`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 18.3 KB (18335 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:8cbeb7cfde7d32b8433e1c01c415fbd6ad8fa9cd259edd4313c1182a978eac09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74063255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b791cfba3e8bc5162ca9521ffdbb0820710918bc04a13a33e6f8be224f55438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:13:36 GMT
ADD file:dcd5696ac281b24df52a518e2402c7f7a4caedfcba0d82e195b7c06cd3a38fdd in / 
# Tue, 19 Dec 2023 02:13:40 GMT
CMD ["bash"]
# Wed, 20 Dec 2023 13:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Dec 2023 13:30:09 GMT
ENV HOME=/home/user
# Wed, 20 Dec 2023 13:30:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Dec 2023 13:30:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 13:30:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 20 Dec 2023 13:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Dec 2023 13:34:25 GMT
WORKDIR /home/user
# Wed, 20 Dec 2023 13:34:29 GMT
USER user
# Wed, 20 Dec 2023 13:34:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:12b1322ffb17b8e81ca1c6d9d7118e2fcee0b9d971aa3c90601e6345804a60d1`  
		Last Modified: Tue, 19 Dec 2023 02:24:36 GMT  
		Size: 29.1 MB (29121427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ad670e672d195ec763bd204f894d09cdc183c6ce311eba2ffc439612121ee`  
		Last Modified: Wed, 20 Dec 2023 13:35:14 GMT  
		Size: 16.9 MB (16929535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb1cb4c20719f053a8b365e7ae8908e7f3fc0b57887a9c01af2cff96600f8e7`  
		Last Modified: Wed, 20 Dec 2023 13:34:58 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fabfead7d49f06de8058ccfeab86b5aee8284be57ed979452324699df85abd1`  
		Last Modified: Wed, 20 Dec 2023 13:35:19 GMT  
		Size: 28.0 MB (28008995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:575ef209f28f4f7ed0a9a7b1c99df2bb2f87cd950a7977188d8be9408323b055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81858507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e1e484a868196a76e57f555fecc46159723e455f87f03731192a645f49205e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c6980c5acfb61420bec3fecb79e92baf26848104c2f1a8cf0d1754bca2bac3e`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 18.8 MB (18757646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:765deb34181ae86766afbb92b8adb60ed2d09436f8b805be2169b2f85c496f0b`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:622166be7f78a644c3966afdbc21cd1d72d5b61221fc50ec222cc6ff1bef82aa`  
		Last Modified: Wed, 20 Dec 2023 21:08:23 GMT  
		Size: 30.0 MB (29976941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:1afc854d3abba98f2eb32986720d792629f71ee99d2d03d0f7c005f41125ae57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6627152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4510d937df9c77199f03f2ffc9c0d973e60235ae776b09cd1ddf79d983389`

```dockerfile
```

-	Layers:
	-	`sha256:8f0991cfc927c50f1f4496eb5371bc577a375f262aebd9f969e6fc90aa5b4f27`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 6.6 MB (6608650 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7204444fbb4c105206ab3f29c0589fc495706f2d07570acbc522140d7a09eb4d`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 18.5 KB (18502 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:60a482b86f2db7fd10d491938f31901c7f6adbac8c2463cb2e2fa62c3c30cf5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72724499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1a2b7df92545b5f83cf7c3dc5f7a38e9573ef5035b06654c733958586e67e7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0caafde47a3e9a6dd324ed419bf5fbf3927b27845c745b95d9c37e1bb7d63a8`  
		Last Modified: Wed, 20 Dec 2023 21:18:34 GMT  
		Size: 18.2 MB (18207265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3d931210f84c8b8a6fbeae35b4a75acad3d2255b470db4a1a421d40c38e2abc`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a383a09d5e97936abef74784a8ef9413735c27dd1a73de75fd3fe595c5719fd`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 27.0 MB (27021999 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:f49bf849702833ecb1a8740440767542d2c5b9980182fde5e48de04801a43a0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6623640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ed98bb6c8dc6a0f89cdc2d7b3d5386486f3daadbfdf2b7237d3bfe0fcbeb41`

```dockerfile
```

-	Layers:
	-	`sha256:65127003855e314eb1d3819c53d0fbe07edefc65c019685ffaaed55b5556af43`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 6.6 MB (6605204 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:055af2286d41963c455bd993dbb42a317414c6a8b4b231e164463af193d45837`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 18.4 KB (18436 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1.4.5`

```console
$ docker pull irssi@sha256:9a77d1df6e590fef8eaae7ba475f2e5a9c43724bec98aff23d9b1631b9220d75
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1.4.5` - linux; amd64

```console
$ docker pull irssi@sha256:5d9147f3379e4b79b86271b8b280d77d7b23212e3a1877b71225a508538a41c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75862383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9176b56d5f8434c83bfe4ca38d64d1fd86b07a0fd49ffe1208f4b5efa59f9fd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1eea906c30d3d0487ae55380baa41c0f4d8b8e35308aac724e9ff9bcec124642`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 18.3 MB (18260013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f0ebb89009ec7651e1ddcb8eb0a59774e42c3bc06a4b223df4b200220914da4`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54234223781082d0352cc2ea4da765bdd0ac4e5c9cc00c8081a79eced99414b9`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 28.5 MB (28473044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5` - unknown; unknown

```console
$ docker pull irssi@sha256:19511cb18b259e0e6c94ab3fce7c9be3ba16ef514db9f61cb7a30193f7fdec1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6634888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381d2efeff58df84e748ac3cbe9d2e46d374c1cd2291648e8a039a13c5393e0`

```dockerfile
```

-	Layers:
	-	`sha256:90cbaa48e8b08df31e60931aabf94fc30837256b3c5d3ca4c4972ce0e97b7d26`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 6.6 MB (6616285 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:448eaa4bf506a9b017f8a3d2fc48ee0633391d71aa6df73781d518620d86b965`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 18.6 KB (18603 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5` - linux; arm variant v5

```console
$ docker pull irssi@sha256:4286526b50c80fffe45f3d033e3fdc13e3f5c04cd6ad1ec14790c2ee8d039a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70039481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf2812ad5e9e3913d5e6e2487a3c5f13f004f7e92d10c414267119db631dba3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd87cc8398be751321cd22ca920bc62183e34f8b4b4ac4a608f07888091da0ce`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 17.0 MB (17034983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a18da79d125b945cad0e400520adaca406e8180d56d64777eac37d6b3d3a97b`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1bcc51f403f8b1d911866ad57127a5c25094f2229c92b9fe5c866e89f4c3ec4`  
		Last Modified: Wed, 20 Dec 2023 20:20:22 GMT  
		Size: 26.1 MB (26115697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5` - unknown; unknown

```console
$ docker pull irssi@sha256:57091b62d44164148afa83ea653c4e3ece0305c5481a3c9797e4c134c4bdc593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b36f2f3830b001060929f79c17d21c3bbcf8522ec030c4585413ef64492300`

```dockerfile
```

-	Layers:
	-	`sha256:be69a9e6f839e05382bfccafc02a33265cb58de10a9d4d54c62ca261eae2ceda`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 18.3 KB (18349 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5` - linux; arm variant v7

```console
$ docker pull irssi@sha256:cb8f06b471dfaa3cd90e41f16b16b6dceaa08f113006002eb02a575759530ad3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66361909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9f07d2e179897cabf0bd0385a54c12835d517ff49a2acc7e2548f54f3c529c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9af19116d503c60c4477fb97778e4d00ec874702ca31ef19d4be65bd203ce75`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 16.6 MB (16627433 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b0e896ad984d1556dc3df25f1f24d17abd4bad05bd68f1ae582f687d457ae7b`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72a4105a0adfa8587dcd54b4600d7f905af063873577b5ff9b0fca192542e045`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 25.0 MB (25012958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5` - unknown; unknown

```console
$ docker pull irssi@sha256:bf41c4ef33d0cc113632b1d9778922afd7d5091de5188addeb1066d5b441420e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6609143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e21deee85550008b9520c1299b0e2697ab56f7d45900ae612816b74feed26d`

```dockerfile
```

-	Layers:
	-	`sha256:789bc7a90003a2b096536fa12b6be4abbef105dc07fbdd85f0ab2e91ecc6c42f`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 6.6 MB (6590579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:37d0d4185472fed8e3e965d668e307726812a2cd1b7543b76085eef8c33e4318`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 18.6 KB (18564 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:4448d99fff66a402267a1326cf56befb11179adc9a588d74d9d232ac6896d13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74613777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6be87e358baeb4ebdb34e1b0bf058728b4c9b4791df705a97af2459aa4b112`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:560bf72e987fd6edd06c8b56f9b1566b5262ee2c254adf3863299dd47c78fa92`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 18.0 MB (18021745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:980da2332d71ffeb3fb18a84dbd721f5c4a52f7dee942f6e1d8e85713a3890cc`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d851282e78a89fab2fca7d86db4275a5e68bb52ea170ef151be24211ee1ea9f`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 27.4 MB (27431401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5` - unknown; unknown

```console
$ docker pull irssi@sha256:51ef1e0b32d9b59ab96443e4f12015237b4289ae8365567cc267e8be313328b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6615458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae12ce93fbd3b325957885cb40c6582cd97d4d8fe0e69b96b92e469e333a84b`

```dockerfile
```

-	Layers:
	-	`sha256:e31580db9e488826eb1086346c8be3366de013ebbcd231d60ced6faca6d545ea`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 6.6 MB (6597004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1fdc10f0e5fa4cb00a3930219cf8bf8c5ea4d37cb721a83bc8eb8006e95dec45`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 18.5 KB (18454 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5` - linux; 386

```console
$ docker pull irssi@sha256:6a8475ff3c12f74fc70976a5161b3fe205b5de6af186234af5f1b589963f5412
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76291252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bd0be5ca51091c547885af81aa5f9ce44a235139086622e3a6cc4425f42abb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f7dc5be6fb0db696a5c82ed11d73cbf826f8b763876f18c25833f1ac9db5a9e`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 17.8 MB (17785994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb9836a268b33d7bfd41001911da5ce8ade91fd68ae9ad1ad4a1444f46d5c802`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc2f90db82b28b52fb5cc5805f4a587ece1c5d91add681edbab73eb99d5829c5`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 28.4 MB (28358032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5` - unknown; unknown

```console
$ docker pull irssi@sha256:ca9217a9d59d109bd6ab0e81c9843708540d923c98f8f4089a0203337f0fb516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9feee74d3925e1773ca2cbdd6daa9468885e693129cf04d99d2b862d2ded7f`

```dockerfile
```

-	Layers:
	-	`sha256:f528901de35025479bc79bcbdceac123bb7b194efcd16d5831474114de792022`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 18.3 KB (18335 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5` - linux; mips64le

```console
$ docker pull irssi@sha256:8cbeb7cfde7d32b8433e1c01c415fbd6ad8fa9cd259edd4313c1182a978eac09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74063255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b791cfba3e8bc5162ca9521ffdbb0820710918bc04a13a33e6f8be224f55438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:13:36 GMT
ADD file:dcd5696ac281b24df52a518e2402c7f7a4caedfcba0d82e195b7c06cd3a38fdd in / 
# Tue, 19 Dec 2023 02:13:40 GMT
CMD ["bash"]
# Wed, 20 Dec 2023 13:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Dec 2023 13:30:09 GMT
ENV HOME=/home/user
# Wed, 20 Dec 2023 13:30:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Dec 2023 13:30:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 13:30:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 20 Dec 2023 13:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Dec 2023 13:34:25 GMT
WORKDIR /home/user
# Wed, 20 Dec 2023 13:34:29 GMT
USER user
# Wed, 20 Dec 2023 13:34:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:12b1322ffb17b8e81ca1c6d9d7118e2fcee0b9d971aa3c90601e6345804a60d1`  
		Last Modified: Tue, 19 Dec 2023 02:24:36 GMT  
		Size: 29.1 MB (29121427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ad670e672d195ec763bd204f894d09cdc183c6ce311eba2ffc439612121ee`  
		Last Modified: Wed, 20 Dec 2023 13:35:14 GMT  
		Size: 16.9 MB (16929535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb1cb4c20719f053a8b365e7ae8908e7f3fc0b57887a9c01af2cff96600f8e7`  
		Last Modified: Wed, 20 Dec 2023 13:34:58 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fabfead7d49f06de8058ccfeab86b5aee8284be57ed979452324699df85abd1`  
		Last Modified: Wed, 20 Dec 2023 13:35:19 GMT  
		Size: 28.0 MB (28008995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5` - linux; ppc64le

```console
$ docker pull irssi@sha256:575ef209f28f4f7ed0a9a7b1c99df2bb2f87cd950a7977188d8be9408323b055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81858507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e1e484a868196a76e57f555fecc46159723e455f87f03731192a645f49205e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c6980c5acfb61420bec3fecb79e92baf26848104c2f1a8cf0d1754bca2bac3e`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 18.8 MB (18757646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:765deb34181ae86766afbb92b8adb60ed2d09436f8b805be2169b2f85c496f0b`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:622166be7f78a644c3966afdbc21cd1d72d5b61221fc50ec222cc6ff1bef82aa`  
		Last Modified: Wed, 20 Dec 2023 21:08:23 GMT  
		Size: 30.0 MB (29976941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5` - unknown; unknown

```console
$ docker pull irssi@sha256:1afc854d3abba98f2eb32986720d792629f71ee99d2d03d0f7c005f41125ae57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6627152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4510d937df9c77199f03f2ffc9c0d973e60235ae776b09cd1ddf79d983389`

```dockerfile
```

-	Layers:
	-	`sha256:8f0991cfc927c50f1f4496eb5371bc577a375f262aebd9f969e6fc90aa5b4f27`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 6.6 MB (6608650 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7204444fbb4c105206ab3f29c0589fc495706f2d07570acbc522140d7a09eb4d`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 18.5 KB (18502 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5` - linux; s390x

```console
$ docker pull irssi@sha256:60a482b86f2db7fd10d491938f31901c7f6adbac8c2463cb2e2fa62c3c30cf5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72724499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1a2b7df92545b5f83cf7c3dc5f7a38e9573ef5035b06654c733958586e67e7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0caafde47a3e9a6dd324ed419bf5fbf3927b27845c745b95d9c37e1bb7d63a8`  
		Last Modified: Wed, 20 Dec 2023 21:18:34 GMT  
		Size: 18.2 MB (18207265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3d931210f84c8b8a6fbeae35b4a75acad3d2255b470db4a1a421d40c38e2abc`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a383a09d5e97936abef74784a8ef9413735c27dd1a73de75fd3fe595c5719fd`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 27.0 MB (27021999 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5` - unknown; unknown

```console
$ docker pull irssi@sha256:f49bf849702833ecb1a8740440767542d2c5b9980182fde5e48de04801a43a0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6623640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ed98bb6c8dc6a0f89cdc2d7b3d5386486f3daadbfdf2b7237d3bfe0fcbeb41`

```dockerfile
```

-	Layers:
	-	`sha256:65127003855e314eb1d3819c53d0fbe07edefc65c019685ffaaed55b5556af43`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 6.6 MB (6605204 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:055af2286d41963c455bd993dbb42a317414c6a8b4b231e164463af193d45837`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 18.4 KB (18436 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1.4.5-alpine`

```console
$ docker pull irssi@sha256:79451b25b3472ba9e2eaea3b2ac29fe6fe096d29e2c8906f5bc613d00d0aa5f5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1.4.5-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:105fa5e67e4e73efc68a46251ccc88bcdd20c1f00791c024d72049ec8c262192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90a1bb4955c1fa1c41936729e39aea9920194ea59a1c610b1a3403c3f0c6150`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e0489114318ebbbb358ac5d32aee84c3a4b5533810fa6706b0648de63eada38`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 9.6 MB (9645476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdf0d195e7f83acc9eedf0071d583bf6af6349889841e7635cf29c43c629c640`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d108ad9c820b6d6e8e249ebc6d8880815c65c45f26892e8a6ab3c9ae45685853`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 5.4 MB (5402203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:d20bcdc49a8bcf8dc91e15bca6c781ebcd7c4dc4198b20d4e313fc2c9c439bee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.5 KB (992458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb852ef521ea46c7682f4f7119f23851f36317e79cce4556e2e9e416fbde2cf`

```dockerfile
```

-	Layers:
	-	`sha256:4cd7f1f45cebca0db6e6b84a0d40d4291bd1884fe3a99cd8699e1f85cc855931`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 975.0 KB (975030 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc7b354d55ff368937c54932656d0c6e35d054544cd811ae952e5339e561af61`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 17.4 KB (17428 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:502678281e0a8fc11e5e60ab54cf7dd84c2ee569f3f870ef4adcaab298fb417b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17270398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899b60c73aa2cd976bff10c64aadf2960af1ce82aa7137f963033a1c8a9e01ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410e5270be4aa0f019d84c2b63359fe74822bbb5d0b839fe7016fc64dfbc7ae0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 8.9 MB (8880076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1571fb6473dae031bdc723dcc05df8bcedb8e7949fe43e60b88b84d28de6359`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c99573a422ea748e601e3fc5a3c7147a082b13fa4b63b41d7410e26fe7185d0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 5.2 MB (5242159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:464a826b2af15230d1a2d27c265fe0c4cdfa1911cc91aa09aea53ed9cfba65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 KB (17341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9858ff23fdfea20d8cc88ee6f6d49900d4a8b83f719dc1bbab498204aa70e95b`

```dockerfile
```

-	Layers:
	-	`sha256:c698656fcb6933453517855d73664fa233a7df879ad29c65c2c7e6c9bd6af2b1`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 17.3 KB (17341 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:781db50a278b2665670bc3112c5c0397014ab37ff3c9f3d9a515449d00407b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5613a41dc765b890dc98b0f1b3c5ff9a53edd2e1445eb87311c9fc626682efe9`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:831415ea41c64b7ebb180f4f1da27bcf8dff3a9c5857deefa938de6334bc05c8`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 8.7 MB (8721217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95002d0dfc5013bc236502c1d58e95122a36e7ced9325e458f87721e74424053`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfcc5163f111398aff0073ad800b7fe8d98fa110ae443c658242fe5979989243`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 5.0 MB (5006513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:80029ca5ee21b65a87e5bffcd0f6e982ab1939bd3a2fd22627ae42ed2677e9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **995.0 KB (994964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be9e8234e96256b98972c25f2a33d5b2f9af93030aa1c99e11688eec589a33`

```dockerfile
```

-	Layers:
	-	`sha256:647518d13f1ec703d0cc9f34b31e2b53de88cb2616b0cb39b44211edcd1de409`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 977.6 KB (977574 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:76183270a354928c61dc0a73762989852386c1f766eb7a8a6f5773870e87ad5f`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 17.4 KB (17390 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9231eee1fd711f485f49771ef585253227fe5803335d2301087e2cb083f099a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18315846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4729d538632dda020f3bcd9bae8a2249d9cad5ae76a8f02f431fc37137c71a14`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86f46af68b50326d6225714f933de969fae879fd66189bbd1edbda8e47ab9343`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 9.7 MB (9673040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183fe6397c74bb1e7159b0a06eebe92da8dbd1b6af699e543a7618777a0bf315`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e28fc2012c204a8e8b903e0d3b7a042e4d5c0867e2e9eeb2340b29cd64ee66f`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 5.3 MB (5308483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:1c785db37c195270ba3ac1385d0509431549621d5ef5ef558ba9c4c1efa77e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.3 KB (992329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5548d8fc5c59a6fd473580a6b28b02ec1f638378bf3a473bf92331dc86e4db05`

```dockerfile
```

-	Layers:
	-	`sha256:90fad57a08e8809e193e2d976c2a6a59a19c5aaaba7933737ca575c34031f786`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 975.0 KB (975049 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:833e49bd915ced6aed85ab32c68fdbcc2809eac8f325ae4d6054353f2b8c1831`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 17.3 KB (17280 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine` - linux; 386

```console
$ docker pull irssi@sha256:a1f46da9d4d08c6ee70f056809a0b2ff79fae6cf722de2cfeb95261aa38bd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff78bbd9939209b5459ddead2d5e68cdea113746073e595135cace9e852ac2bc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afaf371c77ae0674d22138365f359b4ac14ab68be729fe05c7a79e10d726b117`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 8.9 MB (8904451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efe2cca0d709017c0c09011188dd71a937d9f8b4bebc918d2715769719a2f16b`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50bd6dc1d315e6329e05543858a9c8fe102bc166e11901747897745475fa8386`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 5.4 MB (5413019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:6b8364870daa037625c5a97cca22cfda0428edadd69cb3c8a1d00dcfbd6d361a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 KB (17160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b3895d731ba30f2fc6f8e5011be07f0b49d6a34b0cbc66d53c7b5b7b11a335`

```dockerfile
```

-	Layers:
	-	`sha256:c1ddea5c446d03568ddef362b94f90e3f0eef9a1d9953f26955878608f254c4c`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 17.2 KB (17160 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:9c9e58cecb2a60d8f94969085766c8889efbf766f96f59995d5c7b98d1098ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47be3724f03dc5882cc67a78b812dd6776c63edffaba6e670d48085ce1472f7a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d37696a9b7f09eb3052928fc0b0a2bf6b1a9d8a79f15198f00b8f3d7c6f2180e`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 9.7 MB (9736559 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d528e90d2e0d255c01bbbc4d2ead9da704d8bdd46c9941f6e25e61535c53d4e0`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6afb000755ce978e9c79e6e950a600241bef0c449da1370170c9ed808493a309`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 5.6 MB (5630879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:dc9c2d5721c50d04edfdd24dff32af69861be9998efaa742fe7a60cbb6910e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.8 KB (990779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e21d3be4a225b0dee4f04888c254c8da7545ae5d64238735a130e36cf0b3ca5`

```dockerfile
```

-	Layers:
	-	`sha256:a940fbde6476c7e256b3940a1c2571f77dc47966416e58880da03224a07fc411`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 973.5 KB (973452 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:83574fc30d526c7e54ab92e98efeac06578035a04067c1ff1e80c611f8171a86`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 17.3 KB (17327 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:5e2a23003f460cd14e9bc7690c38f6cf05f8a8b254aeae4eafe9164679748305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18707567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95225b5cd25d8f282a3244a872e6e4a783f373df46a5542928d2be3a9ff4bce4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bdf85127dd33246430604be8364aad59011ec1408e05f2760d4365bd707acf5`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 10.1 MB (10083022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3884e11e9a45bef8f46aa3a109d16b19156260a3446a960d36030cda38e2c32d`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97af07dc776076badee757665cb2b7671730020e1c388a5f061fd4314ea988ab`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 5.4 MB (5405800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:05c6dcc8971095fe5681ef8bed84db1a50569df548468626288a5fcc3d2ed038
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.7 KB (990660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152c5fd0322f65eabee1d5613d5f8d91bff738d7a560de9dd19de26507b21a88`

```dockerfile
```

-	Layers:
	-	`sha256:631809d2b169208a798334a1300be704693429072ad3e80adccdcd04bd0fd3c6`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 973.4 KB (973394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7a2cc8c102e1399aff2d9b99a53977edfb5ea139a7b3ef1f0faf71a24a879f`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 17.3 KB (17266 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1.4.5-alpine3.18`

```console
$ docker pull irssi@sha256:79451b25b3472ba9e2eaea3b2ac29fe6fe096d29e2c8906f5bc613d00d0aa5f5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1.4.5-alpine3.18` - linux; amd64

```console
$ docker pull irssi@sha256:105fa5e67e4e73efc68a46251ccc88bcdd20c1f00791c024d72049ec8c262192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90a1bb4955c1fa1c41936729e39aea9920194ea59a1c610b1a3403c3f0c6150`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e0489114318ebbbb358ac5d32aee84c3a4b5533810fa6706b0648de63eada38`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 9.6 MB (9645476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdf0d195e7f83acc9eedf0071d583bf6af6349889841e7635cf29c43c629c640`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d108ad9c820b6d6e8e249ebc6d8880815c65c45f26892e8a6ab3c9ae45685853`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 5.4 MB (5402203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:d20bcdc49a8bcf8dc91e15bca6c781ebcd7c4dc4198b20d4e313fc2c9c439bee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.5 KB (992458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb852ef521ea46c7682f4f7119f23851f36317e79cce4556e2e9e416fbde2cf`

```dockerfile
```

-	Layers:
	-	`sha256:4cd7f1f45cebca0db6e6b84a0d40d4291bd1884fe3a99cd8699e1f85cc855931`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 975.0 KB (975030 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc7b354d55ff368937c54932656d0c6e35d054544cd811ae952e5339e561af61`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 17.4 KB (17428 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:502678281e0a8fc11e5e60ab54cf7dd84c2ee569f3f870ef4adcaab298fb417b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17270398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899b60c73aa2cd976bff10c64aadf2960af1ce82aa7137f963033a1c8a9e01ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410e5270be4aa0f019d84c2b63359fe74822bbb5d0b839fe7016fc64dfbc7ae0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 8.9 MB (8880076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1571fb6473dae031bdc723dcc05df8bcedb8e7949fe43e60b88b84d28de6359`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c99573a422ea748e601e3fc5a3c7147a082b13fa4b63b41d7410e26fe7185d0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 5.2 MB (5242159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:464a826b2af15230d1a2d27c265fe0c4cdfa1911cc91aa09aea53ed9cfba65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 KB (17341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9858ff23fdfea20d8cc88ee6f6d49900d4a8b83f719dc1bbab498204aa70e95b`

```dockerfile
```

-	Layers:
	-	`sha256:c698656fcb6933453517855d73664fa233a7df879ad29c65c2c7e6c9bd6af2b1`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 17.3 KB (17341 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:781db50a278b2665670bc3112c5c0397014ab37ff3c9f3d9a515449d00407b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5613a41dc765b890dc98b0f1b3c5ff9a53edd2e1445eb87311c9fc626682efe9`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:831415ea41c64b7ebb180f4f1da27bcf8dff3a9c5857deefa938de6334bc05c8`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 8.7 MB (8721217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95002d0dfc5013bc236502c1d58e95122a36e7ced9325e458f87721e74424053`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfcc5163f111398aff0073ad800b7fe8d98fa110ae443c658242fe5979989243`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 5.0 MB (5006513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:80029ca5ee21b65a87e5bffcd0f6e982ab1939bd3a2fd22627ae42ed2677e9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **995.0 KB (994964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be9e8234e96256b98972c25f2a33d5b2f9af93030aa1c99e11688eec589a33`

```dockerfile
```

-	Layers:
	-	`sha256:647518d13f1ec703d0cc9f34b31e2b53de88cb2616b0cb39b44211edcd1de409`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 977.6 KB (977574 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:76183270a354928c61dc0a73762989852386c1f766eb7a8a6f5773870e87ad5f`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 17.4 KB (17390 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9231eee1fd711f485f49771ef585253227fe5803335d2301087e2cb083f099a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18315846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4729d538632dda020f3bcd9bae8a2249d9cad5ae76a8f02f431fc37137c71a14`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86f46af68b50326d6225714f933de969fae879fd66189bbd1edbda8e47ab9343`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 9.7 MB (9673040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183fe6397c74bb1e7159b0a06eebe92da8dbd1b6af699e543a7618777a0bf315`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e28fc2012c204a8e8b903e0d3b7a042e4d5c0867e2e9eeb2340b29cd64ee66f`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 5.3 MB (5308483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:1c785db37c195270ba3ac1385d0509431549621d5ef5ef558ba9c4c1efa77e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.3 KB (992329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5548d8fc5c59a6fd473580a6b28b02ec1f638378bf3a473bf92331dc86e4db05`

```dockerfile
```

-	Layers:
	-	`sha256:90fad57a08e8809e193e2d976c2a6a59a19c5aaaba7933737ca575c34031f786`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 975.0 KB (975049 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:833e49bd915ced6aed85ab32c68fdbcc2809eac8f325ae4d6054353f2b8c1831`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 17.3 KB (17280 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:a1f46da9d4d08c6ee70f056809a0b2ff79fae6cf722de2cfeb95261aa38bd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff78bbd9939209b5459ddead2d5e68cdea113746073e595135cace9e852ac2bc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afaf371c77ae0674d22138365f359b4ac14ab68be729fe05c7a79e10d726b117`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 8.9 MB (8904451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efe2cca0d709017c0c09011188dd71a937d9f8b4bebc918d2715769719a2f16b`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50bd6dc1d315e6329e05543858a9c8fe102bc166e11901747897745475fa8386`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 5.4 MB (5413019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:6b8364870daa037625c5a97cca22cfda0428edadd69cb3c8a1d00dcfbd6d361a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 KB (17160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b3895d731ba30f2fc6f8e5011be07f0b49d6a34b0cbc66d53c7b5b7b11a335`

```dockerfile
```

-	Layers:
	-	`sha256:c1ddea5c446d03568ddef362b94f90e3f0eef9a1d9953f26955878608f254c4c`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 17.2 KB (17160 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:9c9e58cecb2a60d8f94969085766c8889efbf766f96f59995d5c7b98d1098ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47be3724f03dc5882cc67a78b812dd6776c63edffaba6e670d48085ce1472f7a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d37696a9b7f09eb3052928fc0b0a2bf6b1a9d8a79f15198f00b8f3d7c6f2180e`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 9.7 MB (9736559 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d528e90d2e0d255c01bbbc4d2ead9da704d8bdd46c9941f6e25e61535c53d4e0`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6afb000755ce978e9c79e6e950a600241bef0c449da1370170c9ed808493a309`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 5.6 MB (5630879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:dc9c2d5721c50d04edfdd24dff32af69861be9998efaa742fe7a60cbb6910e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.8 KB (990779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e21d3be4a225b0dee4f04888c254c8da7545ae5d64238735a130e36cf0b3ca5`

```dockerfile
```

-	Layers:
	-	`sha256:a940fbde6476c7e256b3940a1c2571f77dc47966416e58880da03224a07fc411`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 973.5 KB (973452 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:83574fc30d526c7e54ab92e98efeac06578035a04067c1ff1e80c611f8171a86`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 17.3 KB (17327 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:5e2a23003f460cd14e9bc7690c38f6cf05f8a8b254aeae4eafe9164679748305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18707567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95225b5cd25d8f282a3244a872e6e4a783f373df46a5542928d2be3a9ff4bce4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bdf85127dd33246430604be8364aad59011ec1408e05f2760d4365bd707acf5`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 10.1 MB (10083022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3884e11e9a45bef8f46aa3a109d16b19156260a3446a960d36030cda38e2c32d`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97af07dc776076badee757665cb2b7671730020e1c388a5f061fd4314ea988ab`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 5.4 MB (5405800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:05c6dcc8971095fe5681ef8bed84db1a50569df548468626288a5fcc3d2ed038
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.7 KB (990660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152c5fd0322f65eabee1d5613d5f8d91bff738d7a560de9dd19de26507b21a88`

```dockerfile
```

-	Layers:
	-	`sha256:631809d2b169208a798334a1300be704693429072ad3e80adccdcd04bd0fd3c6`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 973.4 KB (973394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7a2cc8c102e1399aff2d9b99a53977edfb5ea139a7b3ef1f0faf71a24a879f`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 17.3 KB (17266 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:1.4.5-bookworm`

```console
$ docker pull irssi@sha256:9a77d1df6e590fef8eaae7ba475f2e5a9c43724bec98aff23d9b1631b9220d75
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:1.4.5-bookworm` - linux; amd64

```console
$ docker pull irssi@sha256:5d9147f3379e4b79b86271b8b280d77d7b23212e3a1877b71225a508538a41c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75862383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9176b56d5f8434c83bfe4ca38d64d1fd86b07a0fd49ffe1208f4b5efa59f9fd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1eea906c30d3d0487ae55380baa41c0f4d8b8e35308aac724e9ff9bcec124642`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 18.3 MB (18260013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f0ebb89009ec7651e1ddcb8eb0a59774e42c3bc06a4b223df4b200220914da4`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54234223781082d0352cc2ea4da765bdd0ac4e5c9cc00c8081a79eced99414b9`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 28.5 MB (28473044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:19511cb18b259e0e6c94ab3fce7c9be3ba16ef514db9f61cb7a30193f7fdec1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6634888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381d2efeff58df84e748ac3cbe9d2e46d374c1cd2291648e8a039a13c5393e0`

```dockerfile
```

-	Layers:
	-	`sha256:90cbaa48e8b08df31e60931aabf94fc30837256b3c5d3ca4c4972ce0e97b7d26`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 6.6 MB (6616285 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:448eaa4bf506a9b017f8a3d2fc48ee0633391d71aa6df73781d518620d86b965`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 18.6 KB (18603 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:4286526b50c80fffe45f3d033e3fdc13e3f5c04cd6ad1ec14790c2ee8d039a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70039481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf2812ad5e9e3913d5e6e2487a3c5f13f004f7e92d10c414267119db631dba3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd87cc8398be751321cd22ca920bc62183e34f8b4b4ac4a608f07888091da0ce`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 17.0 MB (17034983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a18da79d125b945cad0e400520adaca406e8180d56d64777eac37d6b3d3a97b`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1bcc51f403f8b1d911866ad57127a5c25094f2229c92b9fe5c866e89f4c3ec4`  
		Last Modified: Wed, 20 Dec 2023 20:20:22 GMT  
		Size: 26.1 MB (26115697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:57091b62d44164148afa83ea653c4e3ece0305c5481a3c9797e4c134c4bdc593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b36f2f3830b001060929f79c17d21c3bbcf8522ec030c4585413ef64492300`

```dockerfile
```

-	Layers:
	-	`sha256:be69a9e6f839e05382bfccafc02a33265cb58de10a9d4d54c62ca261eae2ceda`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 18.3 KB (18349 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:cb8f06b471dfaa3cd90e41f16b16b6dceaa08f113006002eb02a575759530ad3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66361909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9f07d2e179897cabf0bd0385a54c12835d517ff49a2acc7e2548f54f3c529c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9af19116d503c60c4477fb97778e4d00ec874702ca31ef19d4be65bd203ce75`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 16.6 MB (16627433 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b0e896ad984d1556dc3df25f1f24d17abd4bad05bd68f1ae582f687d457ae7b`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72a4105a0adfa8587dcd54b4600d7f905af063873577b5ff9b0fca192542e045`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 25.0 MB (25012958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:bf41c4ef33d0cc113632b1d9778922afd7d5091de5188addeb1066d5b441420e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6609143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e21deee85550008b9520c1299b0e2697ab56f7d45900ae612816b74feed26d`

```dockerfile
```

-	Layers:
	-	`sha256:789bc7a90003a2b096536fa12b6be4abbef105dc07fbdd85f0ab2e91ecc6c42f`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 6.6 MB (6590579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:37d0d4185472fed8e3e965d668e307726812a2cd1b7543b76085eef8c33e4318`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 18.6 KB (18564 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:4448d99fff66a402267a1326cf56befb11179adc9a588d74d9d232ac6896d13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74613777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6be87e358baeb4ebdb34e1b0bf058728b4c9b4791df705a97af2459aa4b112`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:560bf72e987fd6edd06c8b56f9b1566b5262ee2c254adf3863299dd47c78fa92`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 18.0 MB (18021745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:980da2332d71ffeb3fb18a84dbd721f5c4a52f7dee942f6e1d8e85713a3890cc`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d851282e78a89fab2fca7d86db4275a5e68bb52ea170ef151be24211ee1ea9f`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 27.4 MB (27431401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:51ef1e0b32d9b59ab96443e4f12015237b4289ae8365567cc267e8be313328b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6615458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae12ce93fbd3b325957885cb40c6582cd97d4d8fe0e69b96b92e469e333a84b`

```dockerfile
```

-	Layers:
	-	`sha256:e31580db9e488826eb1086346c8be3366de013ebbcd231d60ced6faca6d545ea`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 6.6 MB (6597004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1fdc10f0e5fa4cb00a3930219cf8bf8c5ea4d37cb721a83bc8eb8006e95dec45`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 18.5 KB (18454 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-bookworm` - linux; 386

```console
$ docker pull irssi@sha256:6a8475ff3c12f74fc70976a5161b3fe205b5de6af186234af5f1b589963f5412
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76291252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bd0be5ca51091c547885af81aa5f9ce44a235139086622e3a6cc4425f42abb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f7dc5be6fb0db696a5c82ed11d73cbf826f8b763876f18c25833f1ac9db5a9e`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 17.8 MB (17785994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb9836a268b33d7bfd41001911da5ce8ade91fd68ae9ad1ad4a1444f46d5c802`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc2f90db82b28b52fb5cc5805f4a587ece1c5d91add681edbab73eb99d5829c5`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 28.4 MB (28358032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:ca9217a9d59d109bd6ab0e81c9843708540d923c98f8f4089a0203337f0fb516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9feee74d3925e1773ca2cbdd6daa9468885e693129cf04d99d2b862d2ded7f`

```dockerfile
```

-	Layers:
	-	`sha256:f528901de35025479bc79bcbdceac123bb7b194efcd16d5831474114de792022`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 18.3 KB (18335 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:8cbeb7cfde7d32b8433e1c01c415fbd6ad8fa9cd259edd4313c1182a978eac09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74063255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b791cfba3e8bc5162ca9521ffdbb0820710918bc04a13a33e6f8be224f55438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:13:36 GMT
ADD file:dcd5696ac281b24df52a518e2402c7f7a4caedfcba0d82e195b7c06cd3a38fdd in / 
# Tue, 19 Dec 2023 02:13:40 GMT
CMD ["bash"]
# Wed, 20 Dec 2023 13:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Dec 2023 13:30:09 GMT
ENV HOME=/home/user
# Wed, 20 Dec 2023 13:30:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Dec 2023 13:30:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 13:30:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 20 Dec 2023 13:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Dec 2023 13:34:25 GMT
WORKDIR /home/user
# Wed, 20 Dec 2023 13:34:29 GMT
USER user
# Wed, 20 Dec 2023 13:34:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:12b1322ffb17b8e81ca1c6d9d7118e2fcee0b9d971aa3c90601e6345804a60d1`  
		Last Modified: Tue, 19 Dec 2023 02:24:36 GMT  
		Size: 29.1 MB (29121427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ad670e672d195ec763bd204f894d09cdc183c6ce311eba2ffc439612121ee`  
		Last Modified: Wed, 20 Dec 2023 13:35:14 GMT  
		Size: 16.9 MB (16929535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb1cb4c20719f053a8b365e7ae8908e7f3fc0b57887a9c01af2cff96600f8e7`  
		Last Modified: Wed, 20 Dec 2023 13:34:58 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fabfead7d49f06de8058ccfeab86b5aee8284be57ed979452324699df85abd1`  
		Last Modified: Wed, 20 Dec 2023 13:35:19 GMT  
		Size: 28.0 MB (28008995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.4.5-bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:575ef209f28f4f7ed0a9a7b1c99df2bb2f87cd950a7977188d8be9408323b055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81858507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e1e484a868196a76e57f555fecc46159723e455f87f03731192a645f49205e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c6980c5acfb61420bec3fecb79e92baf26848104c2f1a8cf0d1754bca2bac3e`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 18.8 MB (18757646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:765deb34181ae86766afbb92b8adb60ed2d09436f8b805be2169b2f85c496f0b`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:622166be7f78a644c3966afdbc21cd1d72d5b61221fc50ec222cc6ff1bef82aa`  
		Last Modified: Wed, 20 Dec 2023 21:08:23 GMT  
		Size: 30.0 MB (29976941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:1afc854d3abba98f2eb32986720d792629f71ee99d2d03d0f7c005f41125ae57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6627152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4510d937df9c77199f03f2ffc9c0d973e60235ae776b09cd1ddf79d983389`

```dockerfile
```

-	Layers:
	-	`sha256:8f0991cfc927c50f1f4496eb5371bc577a375f262aebd9f969e6fc90aa5b4f27`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 6.6 MB (6608650 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7204444fbb4c105206ab3f29c0589fc495706f2d07570acbc522140d7a09eb4d`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 18.5 KB (18502 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:1.4.5-bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:60a482b86f2db7fd10d491938f31901c7f6adbac8c2463cb2e2fa62c3c30cf5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72724499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1a2b7df92545b5f83cf7c3dc5f7a38e9573ef5035b06654c733958586e67e7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0caafde47a3e9a6dd324ed419bf5fbf3927b27845c745b95d9c37e1bb7d63a8`  
		Last Modified: Wed, 20 Dec 2023 21:18:34 GMT  
		Size: 18.2 MB (18207265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3d931210f84c8b8a6fbeae35b4a75acad3d2255b470db4a1a421d40c38e2abc`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a383a09d5e97936abef74784a8ef9413735c27dd1a73de75fd3fe595c5719fd`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 27.0 MB (27021999 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:1.4.5-bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:f49bf849702833ecb1a8740440767542d2c5b9980182fde5e48de04801a43a0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6623640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ed98bb6c8dc6a0f89cdc2d7b3d5386486f3daadbfdf2b7237d3bfe0fcbeb41`

```dockerfile
```

-	Layers:
	-	`sha256:65127003855e314eb1d3819c53d0fbe07edefc65c019685ffaaed55b5556af43`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 6.6 MB (6605204 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:055af2286d41963c455bd993dbb42a317414c6a8b4b231e164463af193d45837`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 18.4 KB (18436 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:alpine`

```console
$ docker pull irssi@sha256:79451b25b3472ba9e2eaea3b2ac29fe6fe096d29e2c8906f5bc613d00d0aa5f5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:alpine` - linux; amd64

```console
$ docker pull irssi@sha256:105fa5e67e4e73efc68a46251ccc88bcdd20c1f00791c024d72049ec8c262192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90a1bb4955c1fa1c41936729e39aea9920194ea59a1c610b1a3403c3f0c6150`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e0489114318ebbbb358ac5d32aee84c3a4b5533810fa6706b0648de63eada38`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 9.6 MB (9645476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdf0d195e7f83acc9eedf0071d583bf6af6349889841e7635cf29c43c629c640`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d108ad9c820b6d6e8e249ebc6d8880815c65c45f26892e8a6ab3c9ae45685853`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 5.4 MB (5402203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:d20bcdc49a8bcf8dc91e15bca6c781ebcd7c4dc4198b20d4e313fc2c9c439bee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.5 KB (992458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb852ef521ea46c7682f4f7119f23851f36317e79cce4556e2e9e416fbde2cf`

```dockerfile
```

-	Layers:
	-	`sha256:4cd7f1f45cebca0db6e6b84a0d40d4291bd1884fe3a99cd8699e1f85cc855931`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 975.0 KB (975030 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc7b354d55ff368937c54932656d0c6e35d054544cd811ae952e5339e561af61`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 17.4 KB (17428 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:502678281e0a8fc11e5e60ab54cf7dd84c2ee569f3f870ef4adcaab298fb417b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17270398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899b60c73aa2cd976bff10c64aadf2960af1ce82aa7137f963033a1c8a9e01ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410e5270be4aa0f019d84c2b63359fe74822bbb5d0b839fe7016fc64dfbc7ae0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 8.9 MB (8880076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1571fb6473dae031bdc723dcc05df8bcedb8e7949fe43e60b88b84d28de6359`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c99573a422ea748e601e3fc5a3c7147a082b13fa4b63b41d7410e26fe7185d0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 5.2 MB (5242159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:464a826b2af15230d1a2d27c265fe0c4cdfa1911cc91aa09aea53ed9cfba65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 KB (17341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9858ff23fdfea20d8cc88ee6f6d49900d4a8b83f719dc1bbab498204aa70e95b`

```dockerfile
```

-	Layers:
	-	`sha256:c698656fcb6933453517855d73664fa233a7df879ad29c65c2c7e6c9bd6af2b1`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 17.3 KB (17341 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:781db50a278b2665670bc3112c5c0397014ab37ff3c9f3d9a515449d00407b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5613a41dc765b890dc98b0f1b3c5ff9a53edd2e1445eb87311c9fc626682efe9`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:831415ea41c64b7ebb180f4f1da27bcf8dff3a9c5857deefa938de6334bc05c8`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 8.7 MB (8721217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95002d0dfc5013bc236502c1d58e95122a36e7ced9325e458f87721e74424053`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfcc5163f111398aff0073ad800b7fe8d98fa110ae443c658242fe5979989243`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 5.0 MB (5006513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:80029ca5ee21b65a87e5bffcd0f6e982ab1939bd3a2fd22627ae42ed2677e9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **995.0 KB (994964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be9e8234e96256b98972c25f2a33d5b2f9af93030aa1c99e11688eec589a33`

```dockerfile
```

-	Layers:
	-	`sha256:647518d13f1ec703d0cc9f34b31e2b53de88cb2616b0cb39b44211edcd1de409`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 977.6 KB (977574 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:76183270a354928c61dc0a73762989852386c1f766eb7a8a6f5773870e87ad5f`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 17.4 KB (17390 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9231eee1fd711f485f49771ef585253227fe5803335d2301087e2cb083f099a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18315846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4729d538632dda020f3bcd9bae8a2249d9cad5ae76a8f02f431fc37137c71a14`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86f46af68b50326d6225714f933de969fae879fd66189bbd1edbda8e47ab9343`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 9.7 MB (9673040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183fe6397c74bb1e7159b0a06eebe92da8dbd1b6af699e543a7618777a0bf315`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e28fc2012c204a8e8b903e0d3b7a042e4d5c0867e2e9eeb2340b29cd64ee66f`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 5.3 MB (5308483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:1c785db37c195270ba3ac1385d0509431549621d5ef5ef558ba9c4c1efa77e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.3 KB (992329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5548d8fc5c59a6fd473580a6b28b02ec1f638378bf3a473bf92331dc86e4db05`

```dockerfile
```

-	Layers:
	-	`sha256:90fad57a08e8809e193e2d976c2a6a59a19c5aaaba7933737ca575c34031f786`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 975.0 KB (975049 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:833e49bd915ced6aed85ab32c68fdbcc2809eac8f325ae4d6054353f2b8c1831`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 17.3 KB (17280 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:a1f46da9d4d08c6ee70f056809a0b2ff79fae6cf722de2cfeb95261aa38bd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff78bbd9939209b5459ddead2d5e68cdea113746073e595135cace9e852ac2bc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afaf371c77ae0674d22138365f359b4ac14ab68be729fe05c7a79e10d726b117`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 8.9 MB (8904451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efe2cca0d709017c0c09011188dd71a937d9f8b4bebc918d2715769719a2f16b`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50bd6dc1d315e6329e05543858a9c8fe102bc166e11901747897745475fa8386`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 5.4 MB (5413019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:6b8364870daa037625c5a97cca22cfda0428edadd69cb3c8a1d00dcfbd6d361a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 KB (17160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b3895d731ba30f2fc6f8e5011be07f0b49d6a34b0cbc66d53c7b5b7b11a335`

```dockerfile
```

-	Layers:
	-	`sha256:c1ddea5c446d03568ddef362b94f90e3f0eef9a1d9953f26955878608f254c4c`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 17.2 KB (17160 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:9c9e58cecb2a60d8f94969085766c8889efbf766f96f59995d5c7b98d1098ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47be3724f03dc5882cc67a78b812dd6776c63edffaba6e670d48085ce1472f7a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d37696a9b7f09eb3052928fc0b0a2bf6b1a9d8a79f15198f00b8f3d7c6f2180e`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 9.7 MB (9736559 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d528e90d2e0d255c01bbbc4d2ead9da704d8bdd46c9941f6e25e61535c53d4e0`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6afb000755ce978e9c79e6e950a600241bef0c449da1370170c9ed808493a309`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 5.6 MB (5630879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:dc9c2d5721c50d04edfdd24dff32af69861be9998efaa742fe7a60cbb6910e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.8 KB (990779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e21d3be4a225b0dee4f04888c254c8da7545ae5d64238735a130e36cf0b3ca5`

```dockerfile
```

-	Layers:
	-	`sha256:a940fbde6476c7e256b3940a1c2571f77dc47966416e58880da03224a07fc411`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 973.5 KB (973452 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:83574fc30d526c7e54ab92e98efeac06578035a04067c1ff1e80c611f8171a86`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 17.3 KB (17327 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:5e2a23003f460cd14e9bc7690c38f6cf05f8a8b254aeae4eafe9164679748305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18707567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95225b5cd25d8f282a3244a872e6e4a783f373df46a5542928d2be3a9ff4bce4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bdf85127dd33246430604be8364aad59011ec1408e05f2760d4365bd707acf5`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 10.1 MB (10083022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3884e11e9a45bef8f46aa3a109d16b19156260a3446a960d36030cda38e2c32d`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97af07dc776076badee757665cb2b7671730020e1c388a5f061fd4314ea988ab`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 5.4 MB (5405800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine` - unknown; unknown

```console
$ docker pull irssi@sha256:05c6dcc8971095fe5681ef8bed84db1a50569df548468626288a5fcc3d2ed038
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.7 KB (990660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152c5fd0322f65eabee1d5613d5f8d91bff738d7a560de9dd19de26507b21a88`

```dockerfile
```

-	Layers:
	-	`sha256:631809d2b169208a798334a1300be704693429072ad3e80adccdcd04bd0fd3c6`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 973.4 KB (973394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7a2cc8c102e1399aff2d9b99a53977edfb5ea139a7b3ef1f0faf71a24a879f`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 17.3 KB (17266 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:alpine3.18`

```console
$ docker pull irssi@sha256:79451b25b3472ba9e2eaea3b2ac29fe6fe096d29e2c8906f5bc613d00d0aa5f5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:alpine3.18` - linux; amd64

```console
$ docker pull irssi@sha256:105fa5e67e4e73efc68a46251ccc88bcdd20c1f00791c024d72049ec8c262192
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18451394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90a1bb4955c1fa1c41936729e39aea9920194ea59a1c610b1a3403c3f0c6150`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e0489114318ebbbb358ac5d32aee84c3a4b5533810fa6706b0648de63eada38`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 9.6 MB (9645476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdf0d195e7f83acc9eedf0071d583bf6af6349889841e7635cf29c43c629c640`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d108ad9c820b6d6e8e249ebc6d8880815c65c45f26892e8a6ab3c9ae45685853`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 5.4 MB (5402203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:d20bcdc49a8bcf8dc91e15bca6c781ebcd7c4dc4198b20d4e313fc2c9c439bee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.5 KB (992458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb852ef521ea46c7682f4f7119f23851f36317e79cce4556e2e9e416fbde2cf`

```dockerfile
```

-	Layers:
	-	`sha256:4cd7f1f45cebca0db6e6b84a0d40d4291bd1884fe3a99cd8699e1f85cc855931`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 975.0 KB (975030 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc7b354d55ff368937c54932656d0c6e35d054544cd811ae952e5339e561af61`  
		Last Modified: Wed, 20 Dec 2023 20:13:04 GMT  
		Size: 17.4 KB (17428 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine3.18` - linux; arm variant v6

```console
$ docker pull irssi@sha256:502678281e0a8fc11e5e60ab54cf7dd84c2ee569f3f870ef4adcaab298fb417b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 MB (17270398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899b60c73aa2cd976bff10c64aadf2960af1ce82aa7137f963033a1c8a9e01ea`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410e5270be4aa0f019d84c2b63359fe74822bbb5d0b839fe7016fc64dfbc7ae0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 8.9 MB (8880076 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1571fb6473dae031bdc723dcc05df8bcedb8e7949fe43e60b88b84d28de6359`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c99573a422ea748e601e3fc5a3c7147a082b13fa4b63b41d7410e26fe7185d0`  
		Last Modified: Wed, 20 Dec 2023 21:58:15 GMT  
		Size: 5.2 MB (5242159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:464a826b2af15230d1a2d27c265fe0c4cdfa1911cc91aa09aea53ed9cfba65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.3 KB (17341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9858ff23fdfea20d8cc88ee6f6d49900d4a8b83f719dc1bbab498204aa70e95b`

```dockerfile
```

-	Layers:
	-	`sha256:c698656fcb6933453517855d73664fa233a7df879ad29c65c2c7e6c9bd6af2b1`  
		Last Modified: Wed, 20 Dec 2023 21:58:14 GMT  
		Size: 17.3 KB (17341 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine3.18` - linux; arm variant v7

```console
$ docker pull irssi@sha256:781db50a278b2665670bc3112c5c0397014ab37ff3c9f3d9a515449d00407b8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16630028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5613a41dc765b890dc98b0f1b3c5ff9a53edd2e1445eb87311c9fc626682efe9`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:831415ea41c64b7ebb180f4f1da27bcf8dff3a9c5857deefa938de6334bc05c8`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 8.7 MB (8721217 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95002d0dfc5013bc236502c1d58e95122a36e7ced9325e458f87721e74424053`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfcc5163f111398aff0073ad800b7fe8d98fa110ae443c658242fe5979989243`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 5.0 MB (5006513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:80029ca5ee21b65a87e5bffcd0f6e982ab1939bd3a2fd22627ae42ed2677e9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **995.0 KB (994964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be9e8234e96256b98972c25f2a33d5b2f9af93030aa1c99e11688eec589a33`

```dockerfile
```

-	Layers:
	-	`sha256:647518d13f1ec703d0cc9f34b31e2b53de88cb2616b0cb39b44211edcd1de409`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 977.6 KB (977574 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:76183270a354928c61dc0a73762989852386c1f766eb7a8a6f5773870e87ad5f`  
		Last Modified: Wed, 20 Dec 2023 22:50:52 GMT  
		Size: 17.4 KB (17390 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:9231eee1fd711f485f49771ef585253227fe5803335d2301087e2cb083f099a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18315846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4729d538632dda020f3bcd9bae8a2249d9cad5ae76a8f02f431fc37137c71a14`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86f46af68b50326d6225714f933de969fae879fd66189bbd1edbda8e47ab9343`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 9.7 MB (9673040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183fe6397c74bb1e7159b0a06eebe92da8dbd1b6af699e543a7618777a0bf315`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e28fc2012c204a8e8b903e0d3b7a042e4d5c0867e2e9eeb2340b29cd64ee66f`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 5.3 MB (5308483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:1c785db37c195270ba3ac1385d0509431549621d5ef5ef558ba9c4c1efa77e32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **992.3 KB (992329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5548d8fc5c59a6fd473580a6b28b02ec1f638378bf3a473bf92331dc86e4db05`

```dockerfile
```

-	Layers:
	-	`sha256:90fad57a08e8809e193e2d976c2a6a59a19c5aaaba7933737ca575c34031f786`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 975.0 KB (975049 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:833e49bd915ced6aed85ab32c68fdbcc2809eac8f325ae4d6054353f2b8c1831`  
		Last Modified: Wed, 20 Dec 2023 22:06:10 GMT  
		Size: 17.3 KB (17280 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine3.18` - linux; 386

```console
$ docker pull irssi@sha256:a1f46da9d4d08c6ee70f056809a0b2ff79fae6cf722de2cfeb95261aa38bd42a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 MB (17557591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff78bbd9939209b5459ddead2d5e68cdea113746073e595135cace9e852ac2bc`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afaf371c77ae0674d22138365f359b4ac14ab68be729fe05c7a79e10d726b117`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 8.9 MB (8904451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efe2cca0d709017c0c09011188dd71a937d9f8b4bebc918d2715769719a2f16b`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50bd6dc1d315e6329e05543858a9c8fe102bc166e11901747897745475fa8386`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 5.4 MB (5413019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:6b8364870daa037625c5a97cca22cfda0428edadd69cb3c8a1d00dcfbd6d361a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.2 KB (17160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b3895d731ba30f2fc6f8e5011be07f0b49d6a34b0cbc66d53c7b5b7b11a335`

```dockerfile
```

-	Layers:
	-	`sha256:c1ddea5c446d03568ddef362b94f90e3f0eef9a1d9953f26955878608f254c4c`  
		Last Modified: Wed, 20 Dec 2023 20:13:12 GMT  
		Size: 17.2 KB (17160 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine3.18` - linux; ppc64le

```console
$ docker pull irssi@sha256:9c9e58cecb2a60d8f94969085766c8889efbf766f96f59995d5c7b98d1098ad2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18717052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47be3724f03dc5882cc67a78b812dd6776c63edffaba6e670d48085ce1472f7a`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d37696a9b7f09eb3052928fc0b0a2bf6b1a9d8a79f15198f00b8f3d7c6f2180e`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 9.7 MB (9736559 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d528e90d2e0d255c01bbbc4d2ead9da704d8bdd46c9941f6e25e61535c53d4e0`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6afb000755ce978e9c79e6e950a600241bef0c449da1370170c9ed808493a309`  
		Last Modified: Wed, 20 Dec 2023 21:09:16 GMT  
		Size: 5.6 MB (5630879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:dc9c2d5721c50d04edfdd24dff32af69861be9998efaa742fe7a60cbb6910e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.8 KB (990779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e21d3be4a225b0dee4f04888c254c8da7545ae5d64238735a130e36cf0b3ca5`

```dockerfile
```

-	Layers:
	-	`sha256:a940fbde6476c7e256b3940a1c2571f77dc47966416e58880da03224a07fc411`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 973.5 KB (973452 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:83574fc30d526c7e54ab92e98efeac06578035a04067c1ff1e80c611f8171a86`  
		Last Modified: Wed, 20 Dec 2023 21:09:15 GMT  
		Size: 17.3 KB (17327 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:alpine3.18` - linux; s390x

```console
$ docker pull irssi@sha256:5e2a23003f460cd14e9bc7690c38f6cf05f8a8b254aeae4eafe9164679748305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 MB (18707567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95225b5cd25d8f282a3244a872e6e4a783f373df46a5542928d2be3a9ff4bce4`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["/bin/sh"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		meson 		ncurses-dev 		ninja 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 		xz 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bdf85127dd33246430604be8364aad59011ec1408e05f2760d4365bd707acf5`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 10.1 MB (10083022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3884e11e9a45bef8f46aa3a109d16b19156260a3446a960d36030cda38e2c32d`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97af07dc776076badee757665cb2b7671730020e1c388a5f061fd4314ea988ab`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 5.4 MB (5405800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:alpine3.18` - unknown; unknown

```console
$ docker pull irssi@sha256:05c6dcc8971095fe5681ef8bed84db1a50569df548468626288a5fcc3d2ed038
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **990.7 KB (990660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152c5fd0322f65eabee1d5613d5f8d91bff738d7a560de9dd19de26507b21a88`

```dockerfile
```

-	Layers:
	-	`sha256:631809d2b169208a798334a1300be704693429072ad3e80adccdcd04bd0fd3c6`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 973.4 KB (973394 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7a2cc8c102e1399aff2d9b99a53977edfb5ea139a7b3ef1f0faf71a24a879f`  
		Last Modified: Wed, 20 Dec 2023 21:19:20 GMT  
		Size: 17.3 KB (17266 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:bookworm`

```console
$ docker pull irssi@sha256:9a77d1df6e590fef8eaae7ba475f2e5a9c43724bec98aff23d9b1631b9220d75
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:bookworm` - linux; amd64

```console
$ docker pull irssi@sha256:5d9147f3379e4b79b86271b8b280d77d7b23212e3a1877b71225a508538a41c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75862383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9176b56d5f8434c83bfe4ca38d64d1fd86b07a0fd49ffe1208f4b5efa59f9fd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1eea906c30d3d0487ae55380baa41c0f4d8b8e35308aac724e9ff9bcec124642`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 18.3 MB (18260013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f0ebb89009ec7651e1ddcb8eb0a59774e42c3bc06a4b223df4b200220914da4`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54234223781082d0352cc2ea4da765bdd0ac4e5c9cc00c8081a79eced99414b9`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 28.5 MB (28473044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:19511cb18b259e0e6c94ab3fce7c9be3ba16ef514db9f61cb7a30193f7fdec1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6634888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381d2efeff58df84e748ac3cbe9d2e46d374c1cd2291648e8a039a13c5393e0`

```dockerfile
```

-	Layers:
	-	`sha256:90cbaa48e8b08df31e60931aabf94fc30837256b3c5d3ca4c4972ce0e97b7d26`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 6.6 MB (6616285 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:448eaa4bf506a9b017f8a3d2fc48ee0633391d71aa6df73781d518620d86b965`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 18.6 KB (18603 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:bookworm` - linux; arm variant v5

```console
$ docker pull irssi@sha256:4286526b50c80fffe45f3d033e3fdc13e3f5c04cd6ad1ec14790c2ee8d039a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70039481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf2812ad5e9e3913d5e6e2487a3c5f13f004f7e92d10c414267119db631dba3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd87cc8398be751321cd22ca920bc62183e34f8b4b4ac4a608f07888091da0ce`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 17.0 MB (17034983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a18da79d125b945cad0e400520adaca406e8180d56d64777eac37d6b3d3a97b`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1bcc51f403f8b1d911866ad57127a5c25094f2229c92b9fe5c866e89f4c3ec4`  
		Last Modified: Wed, 20 Dec 2023 20:20:22 GMT  
		Size: 26.1 MB (26115697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:57091b62d44164148afa83ea653c4e3ece0305c5481a3c9797e4c134c4bdc593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b36f2f3830b001060929f79c17d21c3bbcf8522ec030c4585413ef64492300`

```dockerfile
```

-	Layers:
	-	`sha256:be69a9e6f839e05382bfccafc02a33265cb58de10a9d4d54c62ca261eae2ceda`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 18.3 KB (18349 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:bookworm` - linux; arm variant v7

```console
$ docker pull irssi@sha256:cb8f06b471dfaa3cd90e41f16b16b6dceaa08f113006002eb02a575759530ad3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66361909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9f07d2e179897cabf0bd0385a54c12835d517ff49a2acc7e2548f54f3c529c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9af19116d503c60c4477fb97778e4d00ec874702ca31ef19d4be65bd203ce75`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 16.6 MB (16627433 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b0e896ad984d1556dc3df25f1f24d17abd4bad05bd68f1ae582f687d457ae7b`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72a4105a0adfa8587dcd54b4600d7f905af063873577b5ff9b0fca192542e045`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 25.0 MB (25012958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:bf41c4ef33d0cc113632b1d9778922afd7d5091de5188addeb1066d5b441420e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6609143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e21deee85550008b9520c1299b0e2697ab56f7d45900ae612816b74feed26d`

```dockerfile
```

-	Layers:
	-	`sha256:789bc7a90003a2b096536fa12b6be4abbef105dc07fbdd85f0ab2e91ecc6c42f`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 6.6 MB (6590579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:37d0d4185472fed8e3e965d668e307726812a2cd1b7543b76085eef8c33e4318`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 18.6 KB (18564 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:bookworm` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:4448d99fff66a402267a1326cf56befb11179adc9a588d74d9d232ac6896d13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74613777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6be87e358baeb4ebdb34e1b0bf058728b4c9b4791df705a97af2459aa4b112`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:560bf72e987fd6edd06c8b56f9b1566b5262ee2c254adf3863299dd47c78fa92`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 18.0 MB (18021745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:980da2332d71ffeb3fb18a84dbd721f5c4a52f7dee942f6e1d8e85713a3890cc`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d851282e78a89fab2fca7d86db4275a5e68bb52ea170ef151be24211ee1ea9f`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 27.4 MB (27431401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:51ef1e0b32d9b59ab96443e4f12015237b4289ae8365567cc267e8be313328b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6615458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae12ce93fbd3b325957885cb40c6582cd97d4d8fe0e69b96b92e469e333a84b`

```dockerfile
```

-	Layers:
	-	`sha256:e31580db9e488826eb1086346c8be3366de013ebbcd231d60ced6faca6d545ea`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 6.6 MB (6597004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1fdc10f0e5fa4cb00a3930219cf8bf8c5ea4d37cb721a83bc8eb8006e95dec45`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 18.5 KB (18454 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:bookworm` - linux; 386

```console
$ docker pull irssi@sha256:6a8475ff3c12f74fc70976a5161b3fe205b5de6af186234af5f1b589963f5412
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76291252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bd0be5ca51091c547885af81aa5f9ce44a235139086622e3a6cc4425f42abb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f7dc5be6fb0db696a5c82ed11d73cbf826f8b763876f18c25833f1ac9db5a9e`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 17.8 MB (17785994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb9836a268b33d7bfd41001911da5ce8ade91fd68ae9ad1ad4a1444f46d5c802`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc2f90db82b28b52fb5cc5805f4a587ece1c5d91add681edbab73eb99d5829c5`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 28.4 MB (28358032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:ca9217a9d59d109bd6ab0e81c9843708540d923c98f8f4089a0203337f0fb516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9feee74d3925e1773ca2cbdd6daa9468885e693129cf04d99d2b862d2ded7f`

```dockerfile
```

-	Layers:
	-	`sha256:f528901de35025479bc79bcbdceac123bb7b194efcd16d5831474114de792022`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 18.3 KB (18335 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:bookworm` - linux; mips64le

```console
$ docker pull irssi@sha256:8cbeb7cfde7d32b8433e1c01c415fbd6ad8fa9cd259edd4313c1182a978eac09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74063255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b791cfba3e8bc5162ca9521ffdbb0820710918bc04a13a33e6f8be224f55438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:13:36 GMT
ADD file:dcd5696ac281b24df52a518e2402c7f7a4caedfcba0d82e195b7c06cd3a38fdd in / 
# Tue, 19 Dec 2023 02:13:40 GMT
CMD ["bash"]
# Wed, 20 Dec 2023 13:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Dec 2023 13:30:09 GMT
ENV HOME=/home/user
# Wed, 20 Dec 2023 13:30:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Dec 2023 13:30:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 13:30:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 20 Dec 2023 13:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Dec 2023 13:34:25 GMT
WORKDIR /home/user
# Wed, 20 Dec 2023 13:34:29 GMT
USER user
# Wed, 20 Dec 2023 13:34:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:12b1322ffb17b8e81ca1c6d9d7118e2fcee0b9d971aa3c90601e6345804a60d1`  
		Last Modified: Tue, 19 Dec 2023 02:24:36 GMT  
		Size: 29.1 MB (29121427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ad670e672d195ec763bd204f894d09cdc183c6ce311eba2ffc439612121ee`  
		Last Modified: Wed, 20 Dec 2023 13:35:14 GMT  
		Size: 16.9 MB (16929535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb1cb4c20719f053a8b365e7ae8908e7f3fc0b57887a9c01af2cff96600f8e7`  
		Last Modified: Wed, 20 Dec 2023 13:34:58 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fabfead7d49f06de8058ccfeab86b5aee8284be57ed979452324699df85abd1`  
		Last Modified: Wed, 20 Dec 2023 13:35:19 GMT  
		Size: 28.0 MB (28008995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:bookworm` - linux; ppc64le

```console
$ docker pull irssi@sha256:575ef209f28f4f7ed0a9a7b1c99df2bb2f87cd950a7977188d8be9408323b055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81858507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e1e484a868196a76e57f555fecc46159723e455f87f03731192a645f49205e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c6980c5acfb61420bec3fecb79e92baf26848104c2f1a8cf0d1754bca2bac3e`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 18.8 MB (18757646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:765deb34181ae86766afbb92b8adb60ed2d09436f8b805be2169b2f85c496f0b`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:622166be7f78a644c3966afdbc21cd1d72d5b61221fc50ec222cc6ff1bef82aa`  
		Last Modified: Wed, 20 Dec 2023 21:08:23 GMT  
		Size: 30.0 MB (29976941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:1afc854d3abba98f2eb32986720d792629f71ee99d2d03d0f7c005f41125ae57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6627152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4510d937df9c77199f03f2ffc9c0d973e60235ae776b09cd1ddf79d983389`

```dockerfile
```

-	Layers:
	-	`sha256:8f0991cfc927c50f1f4496eb5371bc577a375f262aebd9f969e6fc90aa5b4f27`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 6.6 MB (6608650 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7204444fbb4c105206ab3f29c0589fc495706f2d07570acbc522140d7a09eb4d`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 18.5 KB (18502 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:bookworm` - linux; s390x

```console
$ docker pull irssi@sha256:60a482b86f2db7fd10d491938f31901c7f6adbac8c2463cb2e2fa62c3c30cf5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72724499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1a2b7df92545b5f83cf7c3dc5f7a38e9573ef5035b06654c733958586e67e7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0caafde47a3e9a6dd324ed419bf5fbf3927b27845c745b95d9c37e1bb7d63a8`  
		Last Modified: Wed, 20 Dec 2023 21:18:34 GMT  
		Size: 18.2 MB (18207265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3d931210f84c8b8a6fbeae35b4a75acad3d2255b470db4a1a421d40c38e2abc`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a383a09d5e97936abef74784a8ef9413735c27dd1a73de75fd3fe595c5719fd`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 27.0 MB (27021999 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:bookworm` - unknown; unknown

```console
$ docker pull irssi@sha256:f49bf849702833ecb1a8740440767542d2c5b9980182fde5e48de04801a43a0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6623640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ed98bb6c8dc6a0f89cdc2d7b3d5386486f3daadbfdf2b7237d3bfe0fcbeb41`

```dockerfile
```

-	Layers:
	-	`sha256:65127003855e314eb1d3819c53d0fbe07edefc65c019685ffaaed55b5556af43`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 6.6 MB (6605204 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:055af2286d41963c455bd993dbb42a317414c6a8b4b231e164463af193d45837`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 18.4 KB (18436 bytes)  
		MIME: application/vnd.in-toto+json

## `irssi:latest`

```console
$ docker pull irssi@sha256:9a77d1df6e590fef8eaae7ba475f2e5a9c43724bec98aff23d9b1631b9220d75
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `irssi:latest` - linux; amd64

```console
$ docker pull irssi@sha256:5d9147f3379e4b79b86271b8b280d77d7b23212e3a1877b71225a508538a41c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75862383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9176b56d5f8434c83bfe4ca38d64d1fd86b07a0fd49ffe1208f4b5efa59f9fd`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1eea906c30d3d0487ae55380baa41c0f4d8b8e35308aac724e9ff9bcec124642`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 18.3 MB (18260013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f0ebb89009ec7651e1ddcb8eb0a59774e42c3bc06a4b223df4b200220914da4`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54234223781082d0352cc2ea4da765bdd0ac4e5c9cc00c8081a79eced99414b9`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 28.5 MB (28473044 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:latest` - unknown; unknown

```console
$ docker pull irssi@sha256:19511cb18b259e0e6c94ab3fce7c9be3ba16ef514db9f61cb7a30193f7fdec1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6634888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381d2efeff58df84e748ac3cbe9d2e46d374c1cd2291648e8a039a13c5393e0`

```dockerfile
```

-	Layers:
	-	`sha256:90cbaa48e8b08df31e60931aabf94fc30837256b3c5d3ca4c4972ce0e97b7d26`  
		Last Modified: Wed, 20 Dec 2023 20:12:58 GMT  
		Size: 6.6 MB (6616285 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:448eaa4bf506a9b017f8a3d2fc48ee0633391d71aa6df73781d518620d86b965`  
		Last Modified: Wed, 20 Dec 2023 20:12:57 GMT  
		Size: 18.6 KB (18603 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:4286526b50c80fffe45f3d033e3fdc13e3f5c04cd6ad1ec14790c2ee8d039a43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (70039481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf2812ad5e9e3913d5e6e2487a3c5f13f004f7e92d10c414267119db631dba3`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd87cc8398be751321cd22ca920bc62183e34f8b4b4ac4a608f07888091da0ce`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 17.0 MB (17034983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a18da79d125b945cad0e400520adaca406e8180d56d64777eac37d6b3d3a97b`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1bcc51f403f8b1d911866ad57127a5c25094f2229c92b9fe5c866e89f4c3ec4`  
		Last Modified: Wed, 20 Dec 2023 20:20:22 GMT  
		Size: 26.1 MB (26115697 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:latest` - unknown; unknown

```console
$ docker pull irssi@sha256:57091b62d44164148afa83ea653c4e3ece0305c5481a3c9797e4c134c4bdc593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8b36f2f3830b001060929f79c17d21c3bbcf8522ec030c4585413ef64492300`

```dockerfile
```

-	Layers:
	-	`sha256:be69a9e6f839e05382bfccafc02a33265cb58de10a9d4d54c62ca261eae2ceda`  
		Last Modified: Wed, 20 Dec 2023 20:20:21 GMT  
		Size: 18.3 KB (18349 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:cb8f06b471dfaa3cd90e41f16b16b6dceaa08f113006002eb02a575759530ad3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66361909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9f07d2e179897cabf0bd0385a54c12835d517ff49a2acc7e2548f54f3c529c`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9af19116d503c60c4477fb97778e4d00ec874702ca31ef19d4be65bd203ce75`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 16.6 MB (16627433 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b0e896ad984d1556dc3df25f1f24d17abd4bad05bd68f1ae582f687d457ae7b`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72a4105a0adfa8587dcd54b4600d7f905af063873577b5ff9b0fca192542e045`  
		Last Modified: Wed, 20 Dec 2023 22:50:07 GMT  
		Size: 25.0 MB (25012958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:latest` - unknown; unknown

```console
$ docker pull irssi@sha256:bf41c4ef33d0cc113632b1d9778922afd7d5091de5188addeb1066d5b441420e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6609143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e21deee85550008b9520c1299b0e2697ab56f7d45900ae612816b74feed26d`

```dockerfile
```

-	Layers:
	-	`sha256:789bc7a90003a2b096536fa12b6be4abbef105dc07fbdd85f0ab2e91ecc6c42f`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 6.6 MB (6590579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:37d0d4185472fed8e3e965d668e307726812a2cd1b7543b76085eef8c33e4318`  
		Last Modified: Wed, 20 Dec 2023 22:50:06 GMT  
		Size: 18.6 KB (18564 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:4448d99fff66a402267a1326cf56befb11179adc9a588d74d9d232ac6896d13e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74613777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6be87e358baeb4ebdb34e1b0bf058728b4c9b4791df705a97af2459aa4b112`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:560bf72e987fd6edd06c8b56f9b1566b5262ee2c254adf3863299dd47c78fa92`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 18.0 MB (18021745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:980da2332d71ffeb3fb18a84dbd721f5c4a52f7dee942f6e1d8e85713a3890cc`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d851282e78a89fab2fca7d86db4275a5e68bb52ea170ef151be24211ee1ea9f`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 27.4 MB (27431401 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:latest` - unknown; unknown

```console
$ docker pull irssi@sha256:51ef1e0b32d9b59ab96443e4f12015237b4289ae8365567cc267e8be313328b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6615458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae12ce93fbd3b325957885cb40c6582cd97d4d8fe0e69b96b92e469e333a84b`

```dockerfile
```

-	Layers:
	-	`sha256:e31580db9e488826eb1086346c8be3366de013ebbcd231d60ced6faca6d545ea`  
		Last Modified: Wed, 20 Dec 2023 22:05:37 GMT  
		Size: 6.6 MB (6597004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1fdc10f0e5fa4cb00a3930219cf8bf8c5ea4d37cb721a83bc8eb8006e95dec45`  
		Last Modified: Wed, 20 Dec 2023 22:05:36 GMT  
		Size: 18.5 KB (18454 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:6a8475ff3c12f74fc70976a5161b3fe205b5de6af186234af5f1b589963f5412
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76291252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bd0be5ca51091c547885af81aa5f9ce44a235139086622e3a6cc4425f42abb`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f7dc5be6fb0db696a5c82ed11d73cbf826f8b763876f18c25833f1ac9db5a9e`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 17.8 MB (17785994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb9836a268b33d7bfd41001911da5ce8ade91fd68ae9ad1ad4a1444f46d5c802`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 3.3 KB (3331 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc2f90db82b28b52fb5cc5805f4a587ece1c5d91add681edbab73eb99d5829c5`  
		Last Modified: Wed, 20 Dec 2023 20:14:05 GMT  
		Size: 28.4 MB (28358032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:latest` - unknown; unknown

```console
$ docker pull irssi@sha256:ca9217a9d59d109bd6ab0e81c9843708540d923c98f8f4089a0203337f0fb516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 KB (18335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9feee74d3925e1773ca2cbdd6daa9468885e693129cf04d99d2b862d2ded7f`

```dockerfile
```

-	Layers:
	-	`sha256:f528901de35025479bc79bcbdceac123bb7b194efcd16d5831474114de792022`  
		Last Modified: Wed, 20 Dec 2023 20:14:04 GMT  
		Size: 18.3 KB (18335 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:8cbeb7cfde7d32b8433e1c01c415fbd6ad8fa9cd259edd4313c1182a978eac09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74063255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b791cfba3e8bc5162ca9521ffdbb0820710918bc04a13a33e6f8be224f55438`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 19 Dec 2023 02:13:36 GMT
ADD file:dcd5696ac281b24df52a518e2402c7f7a4caedfcba0d82e195b7c06cd3a38fdd in / 
# Tue, 19 Dec 2023 02:13:40 GMT
CMD ["bash"]
# Wed, 20 Dec 2023 13:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Dec 2023 13:30:09 GMT
ENV HOME=/home/user
# Wed, 20 Dec 2023 13:30:17 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 20 Dec 2023 13:30:20 GMT
ENV LANG=C.UTF-8
# Wed, 20 Dec 2023 13:30:23 GMT
ENV IRSSI_VERSION=1.4.5
# Wed, 20 Dec 2023 13:34:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 20 Dec 2023 13:34:25 GMT
WORKDIR /home/user
# Wed, 20 Dec 2023 13:34:29 GMT
USER user
# Wed, 20 Dec 2023 13:34:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:12b1322ffb17b8e81ca1c6d9d7118e2fcee0b9d971aa3c90601e6345804a60d1`  
		Last Modified: Tue, 19 Dec 2023 02:24:36 GMT  
		Size: 29.1 MB (29121427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ad670e672d195ec763bd204f894d09cdc183c6ce311eba2ffc439612121ee`  
		Last Modified: Wed, 20 Dec 2023 13:35:14 GMT  
		Size: 16.9 MB (16929535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb1cb4c20719f053a8b365e7ae8908e7f3fc0b57887a9c01af2cff96600f8e7`  
		Last Modified: Wed, 20 Dec 2023 13:34:58 GMT  
		Size: 3.3 KB (3298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fabfead7d49f06de8058ccfeab86b5aee8284be57ed979452324699df85abd1`  
		Last Modified: Wed, 20 Dec 2023 13:35:19 GMT  
		Size: 28.0 MB (28008995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:575ef209f28f4f7ed0a9a7b1c99df2bb2f87cd950a7977188d8be9408323b055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81858507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e1e484a868196a76e57f555fecc46159723e455f87f03731192a645f49205e`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c6980c5acfb61420bec3fecb79e92baf26848104c2f1a8cf0d1754bca2bac3e`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 18.8 MB (18757646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:765deb34181ae86766afbb92b8adb60ed2d09436f8b805be2169b2f85c496f0b`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 3.3 KB (3330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:622166be7f78a644c3966afdbc21cd1d72d5b61221fc50ec222cc6ff1bef82aa`  
		Last Modified: Wed, 20 Dec 2023 21:08:23 GMT  
		Size: 30.0 MB (29976941 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:latest` - unknown; unknown

```console
$ docker pull irssi@sha256:1afc854d3abba98f2eb32986720d792629f71ee99d2d03d0f7c005f41125ae57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6627152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3af4510d937df9c77199f03f2ffc9c0d973e60235ae776b09cd1ddf79d983389`

```dockerfile
```

-	Layers:
	-	`sha256:8f0991cfc927c50f1f4496eb5371bc577a375f262aebd9f969e6fc90aa5b4f27`  
		Last Modified: Wed, 20 Dec 2023 21:08:22 GMT  
		Size: 6.6 MB (6608650 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7204444fbb4c105206ab3f29c0589fc495706f2d07570acbc522140d7a09eb4d`  
		Last Modified: Wed, 20 Dec 2023 21:08:21 GMT  
		Size: 18.5 KB (18502 bytes)  
		MIME: application/vnd.in-toto+json

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:60a482b86f2db7fd10d491938f31901c7f6adbac8c2463cb2e2fa62c3c30cf5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72724499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1a2b7df92545b5f83cf7c3dc5f7a38e9573ef5035b06654c733958586e67e7`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 03 Oct 2023 09:06:10 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV HOME=/home/user
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME" # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:06:10 GMT
ENV IRSSI_VERSION=1.4.5
# Tue, 03 Oct 2023 09:06:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		meson 		ninja-build 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	meson 		-Denable-true-color=yes 		-Dwith-bot=yes 		-Dwith-perl=yes 		-Dwith-proxy=yes 		Build 	; 	ninja -C Build -j "$(nproc)"; 	ninja -C Build install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version # buildkit
# Tue, 03 Oct 2023 09:06:10 GMT
WORKDIR /home/user
# Tue, 03 Oct 2023 09:06:10 GMT
USER user
# Tue, 03 Oct 2023 09:06:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0caafde47a3e9a6dd324ed419bf5fbf3927b27845c745b95d9c37e1bb7d63a8`  
		Last Modified: Wed, 20 Dec 2023 21:18:34 GMT  
		Size: 18.2 MB (18207265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3d931210f84c8b8a6fbeae35b4a75acad3d2255b470db4a1a421d40c38e2abc`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 3.3 KB (3329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a383a09d5e97936abef74784a8ef9413735c27dd1a73de75fd3fe595c5719fd`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 27.0 MB (27021999 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `irssi:latest` - unknown; unknown

```console
$ docker pull irssi@sha256:f49bf849702833ecb1a8740440767542d2c5b9980182fde5e48de04801a43a0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6623640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ed98bb6c8dc6a0f89cdc2d7b3d5386486f3daadbfdf2b7237d3bfe0fcbeb41`

```dockerfile
```

-	Layers:
	-	`sha256:65127003855e314eb1d3819c53d0fbe07edefc65c019685ffaaed55b5556af43`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 6.6 MB (6605204 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:055af2286d41963c455bd993dbb42a317414c6a8b4b231e164463af193d45837`  
		Last Modified: Wed, 20 Dec 2023 21:18:33 GMT  
		Size: 18.4 KB (18436 bytes)  
		MIME: application/vnd.in-toto+json
