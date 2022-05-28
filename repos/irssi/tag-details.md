<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `irssi`

-	[`irssi:1`](#irssi1)
-	[`irssi:1-alpine`](#irssi1-alpine)
-	[`irssi:1.2`](#irssi12)
-	[`irssi:1.2-alpine`](#irssi12-alpine)
-	[`irssi:1.2.3`](#irssi123)
-	[`irssi:1.2.3-alpine`](#irssi123-alpine)
-	[`irssi:alpine`](#irssialpine)
-	[`irssi:latest`](#irssilatest)

## `irssi:1`

```console
$ docker pull irssi@sha256:9e19096cc30c331015cc1e4ebb3a4f11967adb7c2ae52aa11dc775f90441605f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1` - linux; amd64

```console
$ docker pull irssi@sha256:9b8e794c52606ddb03386ca63e00b8822bb0422ba8d1bbc1f6a91b1169badcf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50616256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d9bf5187a352d791a3be64008fab00c63e5153e65db45b19b848fafffa65e7`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:20:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:20:24 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 05:20:25 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 05:20:25 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 05:20:25 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 05:21:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 05:21:09 GMT
WORKDIR /home/user
# Sat, 28 May 2022 05:21:09 GMT
USER user
# Sat, 28 May 2022 05:21:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1afda879f82264f53bd7206d0529f22e6289f5c266669663f9a1dbcb2377086`  
		Last Modified: Sat, 28 May 2022 05:21:37 GMT  
		Size: 17.0 MB (17038480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b893d548ee02faada4ffcfce881ee9a9d8e144b1d052d85e14338a10a584f73f`  
		Last Modified: Sat, 28 May 2022 05:21:33 GMT  
		Size: 4.2 KB (4213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78daf0e1ebbead3bdba065457c48d6a82da6191e098a16e5b228c56e2079d10`  
		Last Modified: Sat, 28 May 2022 05:21:35 GMT  
		Size: 6.4 MB (6433419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v5

```console
$ docker pull irssi@sha256:319e7359b22812fedb09a44d23cd11e0da8e2764a1f58117d086cb28b1efbfae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46896517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece64e4b9eb38841094e52414e2eb69af1f67124e41ae31ab7f4eb05e168e822`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 02:04:06 GMT
ADD file:26e9ed6c41ec12bf5fd602b7f86b924d34537bbc82442f630763f9f6c48bf3b3 in / 
# Sat, 28 May 2022 02:04:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:51:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:51:33 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 03:51:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 03:51:35 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 03:51:35 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 03:53:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 03:53:30 GMT
WORKDIR /home/user
# Sat, 28 May 2022 03:53:30 GMT
USER user
# Sat, 28 May 2022 03:53:31 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:19389fd1100abdedaa775b43242838cdd2d5c8c3388643a7e52da2b7b4399c15`  
		Last Modified: Sat, 28 May 2022 02:20:06 GMT  
		Size: 24.9 MB (24890069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc97e5088dad5dd24e65c10e4ea9e411d109a92d2e5ea0ea963e08e311ad796`  
		Last Modified: Sat, 28 May 2022 03:54:27 GMT  
		Size: 15.9 MB (15937730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4a37ba27a89a967fe9c2d2f15f8e694a897f7ce14473c47467a7d1fee1f5eb`  
		Last Modified: Sat, 28 May 2022 03:54:12 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a75a4f2bb09f772d8125095f28993565ba0cedf1ea7e623d06819383b74dd`  
		Last Modified: Sat, 28 May 2022 03:54:16 GMT  
		Size: 6.1 MB (6064521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4cf05cf78af130b124c2677cfc8a08fb5b49ee61ef19ee43cf5aa7d668ea8609
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44283091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bde88159cecf11997b4d861c8ce640cc9e4dc449048d1436268d80152d736f`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:00:54 GMT
ADD file:c89d47099a38749a424760d9c7d3a6e982089455ba9d04140db15ba9eb4cdda1 in / 
# Sat, 28 May 2022 01:00:55 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:32:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:33:00 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 07:33:02 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 07:33:02 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 07:33:02 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 07:34:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 07:34:50 GMT
WORKDIR /home/user
# Sat, 28 May 2022 07:34:50 GMT
USER user
# Sat, 28 May 2022 07:34:51 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e41117292dc8c199b63ae1ec4485358841dbcba68dcbd13f379b66182efe832e`  
		Last Modified: Sat, 28 May 2022 01:16:58 GMT  
		Size: 22.7 MB (22748097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3818c0c31072687a62a285a3582a6ac59a7e9c1c0d84423739dafb09cd2f397`  
		Last Modified: Sat, 28 May 2022 07:36:12 GMT  
		Size: 15.6 MB (15598239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c30d93b9a282c1f30a84b17541b5cb2b05cdbced870f4f1f7097d1c79985ee`  
		Last Modified: Sat, 28 May 2022 07:35:57 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22736721f72dfd763c95b664b3afb4327c73190f4bf5230c40283d02328701eb`  
		Last Modified: Sat, 28 May 2022 07:36:00 GMT  
		Size: 5.9 MB (5932564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:93331fad416045665e2b6bfb19606ccc3e2da9ab35ac8e4f3e359d9d8564efa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48908753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d67ac80f549afca6223607f6df4382b1f3caefa46171f8129e47175a13833c`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 00:41:05 GMT
ADD file:d0e42d603f275c040783ec7b6c051200815492fc35b73110234dfcd584e6cdec in / 
# Sat, 28 May 2022 00:41:05 GMT
CMD ["bash"]
# Sat, 28 May 2022 13:07:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 13:07:23 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 13:07:24 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 13:07:25 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 13:07:26 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 13:08:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 13:08:08 GMT
WORKDIR /home/user
# Sat, 28 May 2022 13:08:09 GMT
USER user
# Sat, 28 May 2022 13:08:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4931fb8ba4223cb35034141162105ee5482122692b2931eb69eec912ce64606d`  
		Last Modified: Sat, 28 May 2022 00:48:26 GMT  
		Size: 25.9 MB (25914033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578f8e8c703cdf2c34f2aacd16e83af9040d1c923427dc5fe10fff3969b17983`  
		Last Modified: Sat, 28 May 2022 13:08:49 GMT  
		Size: 16.8 MB (16814580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dba055597f3b5e93280156ec02d53a40d9604ae8e34f7b120795b251f0adab`  
		Last Modified: Sat, 28 May 2022 13:08:46 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1655e15c8cad9556df1295427409be5707ebc949b480830c26e363b0b146534c`  
		Last Modified: Sat, 28 May 2022 13:08:47 GMT  
		Size: 6.2 MB (6176068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; 386

```console
$ docker pull irssi@sha256:f87197bcb070dc6091ab19977c431f3e95e762098396a327d292f019ddb5dc0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50263361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c22d8c0a1d40fa9e5af5c700fc4e768e9277eb28e82bad9f5bbafd0fb48def2e`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 00:40:01 GMT
ADD file:9aea7a35c215cdd778adec1dd5213973ef9b4830110e4550f2ead85679551ee5 in / 
# Sat, 28 May 2022 00:40:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 12:36:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 12:36:40 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 12:36:41 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 12:36:42 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 12:36:43 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 12:37:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 12:37:28 GMT
WORKDIR /home/user
# Sat, 28 May 2022 12:37:29 GMT
USER user
# Sat, 28 May 2022 12:37:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:40837b3d848885c0b0c031d6d950b38e6a26962a5ee49704cb3ca2d2db535617`  
		Last Modified: Sat, 28 May 2022 00:47:36 GMT  
		Size: 27.8 MB (27799572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd85652cb7aee11a1ee235bfe214f30f2eed4280ecc94c7721326d13bbaeaf`  
		Last Modified: Sat, 28 May 2022 12:38:05 GMT  
		Size: 16.6 MB (16566304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c056bbb0e1c559600ab3a62c0b4cb4e41e2277f340915f3e120c990c97bafa84`  
		Last Modified: Sat, 28 May 2022 12:38:02 GMT  
		Size: 4.1 KB (4058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9f8088df3ca5683e0a6dfe2a6aaf868428ecfcbef01b067549522f8b11e93`  
		Last Modified: Sat, 28 May 2022 12:38:03 GMT  
		Size: 5.9 MB (5893427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; mips64le

```console
$ docker pull irssi@sha256:4bf810ff969b5912a5e687a4c44aa741870b792ff2ec4a48afa82cf959023d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47631105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b4d731d65f3d51d2dfe09f12efe86b3963cdc36b44461ec2373fa54942db31`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:12:21 GMT
ADD file:12eb3f58e1c47ef1af98f481c1f5f33832f45144bf66f3a01065f8c939f1eaa9 in / 
# Sat, 28 May 2022 01:12:25 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:15:46 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 03:15:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 03:15:57 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 03:16:00 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 03:20:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 03:20:30 GMT
WORKDIR /home/user
# Sat, 28 May 2022 03:20:33 GMT
USER user
# Sat, 28 May 2022 03:20:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:79a954ba282b6c17b5d2fdc4563e0fbc4bf4e3c673bada0b2f656937656557eb`  
		Last Modified: Sat, 28 May 2022 01:22:56 GMT  
		Size: 25.8 MB (25814580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad211fee54c5f12de817e949479da0f9fa7e5923811567b7286c6050032245fc`  
		Last Modified: Sat, 28 May 2022 03:21:16 GMT  
		Size: 15.7 MB (15732112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805cb834a6e653d97de303cfc43b9da9082614eb08397f22b596a004b9532474`  
		Last Modified: Sat, 28 May 2022 03:21:02 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edb471e3b1d4a83905a6a5c109848bbdf1f68055b04cc7a6763006a14dfc474`  
		Last Modified: Sat, 28 May 2022 03:21:06 GMT  
		Size: 6.1 MB (6080339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; ppc64le

```console
$ docker pull irssi@sha256:e39d45ef70272a2e6cf18c9dd66d12ee70a3645f2046b11496743d0cd865deca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54787987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baff97fede43b1fb6e3ca8de715b96fc263414eedea56bd2b0051990c5ed73d9`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:23:57 GMT
ADD file:a8c6c897bc64da424049ad04a354d123b0622abda1a56b2725f72de5e4569df8 in / 
# Sat, 28 May 2022 01:24:04 GMT
CMD ["bash"]
# Sat, 28 May 2022 06:52:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 06:52:32 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 06:52:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 06:52:38 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 06:52:41 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 06:57:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 06:57:14 GMT
WORKDIR /home/user
# Sat, 28 May 2022 06:57:16 GMT
USER user
# Sat, 28 May 2022 06:57:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:087d40850259bdcd3bee3d5d30d5a2070216727f72c1c9731b514ac3dbf7573e`  
		Last Modified: Sat, 28 May 2022 01:33:30 GMT  
		Size: 30.6 MB (30560238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e180ca0caaecd96894d59df3140df02564c778c40d46b6d03f0fda10eefa6d35`  
		Last Modified: Sat, 28 May 2022 06:58:03 GMT  
		Size: 17.4 MB (17440702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932bc69b6c04fbdc83f98628214743c0e6645a14a5adb34acc1d5590c38d360`  
		Last Modified: Sat, 28 May 2022 06:57:58 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf716870602840820cee5bb11e395b8197b4435e92d9213dba7ad4456818e16`  
		Last Modified: Sat, 28 May 2022 06:58:00 GMT  
		Size: 6.8 MB (6782838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1` - linux; s390x

```console
$ docker pull irssi@sha256:6babbc57189870e9c78763f97de83c067a89b24ddac49f302b21504254e0da1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49061887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b289242502c712e59b5bc78e77d30bad09363d5bdbf1da235ab944c5f4a4393`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 May 2022 00:44:47 GMT
ADD file:28b1e60f65391906bebd81248a4da766172138fab99b8b9e6b18bce76afea02d in / 
# Wed, 11 May 2022 00:44:49 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:29:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:29:57 GMT
ENV HOME=/home/user
# Wed, 11 May 2022 02:29:58 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 May 2022 02:29:58 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 02:29:58 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 11 May 2022 02:30:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 May 2022 02:30:37 GMT
WORKDIR /home/user
# Wed, 11 May 2022 02:30:37 GMT
USER user
# Wed, 11 May 2022 02:30:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bf64474a39a67000556a4502abd4584010a062b942cf8e2545d0502d38ffa150`  
		Last Modified: Wed, 11 May 2022 00:50:43 GMT  
		Size: 25.8 MB (25758738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bab2a510dcd371ba308d88b7a421f4392242a1145a5e2032557bff64f1f3096`  
		Last Modified: Wed, 11 May 2022 02:31:19 GMT  
		Size: 16.9 MB (16914219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114f12ef452583e1b53623df64e6ed1ef5fe101a2bd32bcb5670547708d201b1`  
		Last Modified: Wed, 11 May 2022 02:31:16 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3872a1d35d40ae59cc2e54813e37c9cd0c725b5df75a8e79c674d79cfed86c`  
		Last Modified: Wed, 11 May 2022 02:31:17 GMT  
		Size: 6.4 MB (6384718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1-alpine`

```console
$ docker pull irssi@sha256:bfbb6e415dbf4cd1ea2d6bd42bdcc5fcc054d6b053c6d07b983c9b390dac8f9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:c38f2415219abd42abe51fa4eaf222d8d7c7bdebb86910500d59bb7d0c21b231
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c0676773ef4ea9992d62133ac02ba861fde6dd9ba437e8fb36eaf4aae78852`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:16 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 11:18:17 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 11:18:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 11:18:17 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:18:17 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 11:19:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 11:19:01 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 11:19:01 GMT
USER user
# Tue, 05 Apr 2022 11:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa1dbdb27d63340f8b8fa494a282aeded5f878185e2847d6dfb481b353b8c11`  
		Last Modified: Tue, 05 Apr 2022 11:19:27 GMT  
		Size: 9.5 MB (9540662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd245485e0307925fa298d8f511fe481b6600ce336c8ff0a0b5c13ce1435d9`  
		Last Modified: Tue, 05 Apr 2022 11:19:24 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4513426f1a6993290c7fa1e95a9f0bd0309456d69e3c04c0a7e8b17b66c9a079`  
		Last Modified: Tue, 05 Apr 2022 11:19:25 GMT  
		Size: 6.3 MB (6287259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:5262462a3f32457835863ac8b11823de2d926d672219bdff8c5c67bc5e116e2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab49acd659041f4c479472bb7ed35e0fc93656b968625544d96599e44c57c01`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:01:19 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:01:20 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:01:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:01:22 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:01:22 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:02:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:02:32 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:02:32 GMT
USER user
# Tue, 05 Apr 2022 04:02:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b589ee3c7baf4a3043d5c498c04269109c4a45e58c44ab98b5a969b7ba2f8a`  
		Last Modified: Tue, 05 Apr 2022 04:03:13 GMT  
		Size: 8.8 MB (8771955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82acf7c178275d848adf6769cd6193b1f701750ef2bf058c507c10c4af90080d`  
		Last Modified: Tue, 05 Apr 2022 04:03:05 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391da21a1ce4611cc08325dc363346ea9ae04e1724386ad9b1a8801e1843e835`  
		Last Modified: Tue, 05 Apr 2022 04:03:09 GMT  
		Size: 6.0 MB (5987042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:85b6871234efe5afa8aee356cecfc27abb04e6a99f43a969eedce41a3230299b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f387771b9c45b2879b4d36faf8f6326c4b27afacac146e4d774c52b2d0f103cb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:58:06 GMT
ADD file:0834e20e80add8b1c6bd545ebe0729239e00a4dff08b025cb5555cd3ce58e4c6 in / 
# Mon, 04 Apr 2022 23:58:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:02:01 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 16:02:01 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 16:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 16:02:03 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:02:04 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 16:03:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 16:03:10 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 16:03:10 GMT
USER user
# Tue, 05 Apr 2022 16:03:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a8b8a1c7a552f6893757dd6327a5a430981d78aa06a59298076603526186829e`  
		Last Modified: Mon, 04 Apr 2022 23:59:56 GMT  
		Size: 2.4 MB (2427836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0c71a12aa1dc1147bd41cf6458906772bf77be69de2e8fc3d9242f641fc445`  
		Last Modified: Tue, 05 Apr 2022 16:04:19 GMT  
		Size: 8.6 MB (8626381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf67fa3e83093b4230c7f24388cfb9f6f9aa8bd3c5d76434f7b058a66d7ab80`  
		Last Modified: Tue, 05 Apr 2022 16:04:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a6a97274960e7695eb8d37b680b0fe6bc45a12b2b550e310504260e923285`  
		Last Modified: Tue, 05 Apr 2022 16:04:15 GMT  
		Size: 5.8 MB (5783964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:d49fa5e7d3a8cd10c7bfad3e9bec2fa37e6a44c2911c1958c7014a121f4eef59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98cf9f811eb592e3b8c251eb41f7f7dfdadc8c7b6dc2e9fae2c2d835173d8ac`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:14:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:14:16 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:14:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:14:18 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:14:19 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:14:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:14:54 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:14:55 GMT
USER user
# Tue, 05 Apr 2022 04:14:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f125d0f2f3de8f4307e1218e71620016554b5120c8ce30e8786904dc74366d0b`  
		Last Modified: Tue, 05 Apr 2022 04:15:25 GMT  
		Size: 9.5 MB (9536419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c48a8193426a12a478ffa39f46aa61977b41d48a60d252930c3c2a4708fd0b7`  
		Last Modified: Tue, 05 Apr 2022 04:15:23 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7a5707b30c726d92bca84220a2cb23b4ff000e7119f0a696975a866269d135`  
		Last Modified: Tue, 05 Apr 2022 04:15:24 GMT  
		Size: 6.2 MB (6247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; 386

```console
$ docker pull irssi@sha256:f4044a89fe2a5119671314da6e8cbfed9929c215d20d677e6b84a7e5b713611f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17704054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aea095e2938971334ab2464fcf39c254bd75a69e3b56999f7fab374fb813c92`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:47:49 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 06:47:49 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 06:47:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 06:47:51 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 06:47:52 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 06:48:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 06:48:28 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 06:48:29 GMT
USER user
# Tue, 05 Apr 2022 06:48:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d17b6eaf713c06aeabfe2feac029d7c880865cf49ab0c148c784791c31779`  
		Last Modified: Tue, 05 Apr 2022 06:49:01 GMT  
		Size: 8.9 MB (8904271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831ba5a4f1fc534f7dec6b2cf96d9935df1d6b00524538974d10799fd6f4c53`  
		Last Modified: Tue, 05 Apr 2022 06:48:59 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3dd29c50ebba7606220a2a714a5fdb3059694e3f39c9b707f4c43086cf958`  
		Last Modified: Tue, 05 Apr 2022 06:49:00 GMT  
		Size: 6.0 MB (5978011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:beba11d08d6df10a4fe4518b49c2e3d8b54f2cb9f15feb8bce4bfba5d97c6674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37da7ed44ea84c9ebfb079e981447b44fccab806fd3be499c492a079908bf21d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:10:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 19:10:11 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 19:10:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 19:10:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 19:10:29 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 19:11:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 19:11:33 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 19:11:36 GMT
USER user
# Tue, 05 Apr 2022 19:11:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73fa56481e3f5fd84b721b288e4628ef18d832025ab22c2cb0601f85d9025b`  
		Last Modified: Tue, 05 Apr 2022 19:12:17 GMT  
		Size: 9.6 MB (9632765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2998f1c0df5727d61352cf5bbb86f17a2b07e8d0feef2892ad0c1a13693ed8`  
		Last Modified: Tue, 05 Apr 2022 19:12:15 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0ce73fb7b2975452460737c989e296843d87ad3f26c26f5c7df696df51a1ea`  
		Last Modified: Tue, 05 Apr 2022 19:12:16 GMT  
		Size: 6.5 MB (6492183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:07e9626c05472af1fce5448f4310a04d7bc5e3a7e6a4384227d5aaec02d65705
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18855197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5ea35b9201821c8168c1b19f5a926438127784e392a0465b5a49bc2b7f98e1`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:58:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 03:58:35 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 03:58:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 03:58:36 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:58:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 03:59:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 03:59:07 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 03:59:07 GMT
USER user
# Tue, 05 Apr 2022 03:59:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2a655edb7398e76b909cbb12baf208d875c598793a42546c8f2b906ab8e2c7`  
		Last Modified: Tue, 05 Apr 2022 03:59:36 GMT  
		Size: 10.0 MB (9972200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16218c4743041a59790e9a6b9388344940cd9dbf0e8c3cff8ea17486b32b553`  
		Last Modified: Tue, 05 Apr 2022 03:59:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e5f35e6bfccd90acff05f4db673effe1dce4f736f0d128d6e878f5524767`  
		Last Modified: Tue, 05 Apr 2022 03:59:35 GMT  
		Size: 6.3 MB (6276668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2`

```console
$ docker pull irssi@sha256:9e19096cc30c331015cc1e4ebb3a4f11967adb7c2ae52aa11dc775f90441605f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.2` - linux; amd64

```console
$ docker pull irssi@sha256:9b8e794c52606ddb03386ca63e00b8822bb0422ba8d1bbc1f6a91b1169badcf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50616256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d9bf5187a352d791a3be64008fab00c63e5153e65db45b19b848fafffa65e7`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:20:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:20:24 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 05:20:25 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 05:20:25 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 05:20:25 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 05:21:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 05:21:09 GMT
WORKDIR /home/user
# Sat, 28 May 2022 05:21:09 GMT
USER user
# Sat, 28 May 2022 05:21:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1afda879f82264f53bd7206d0529f22e6289f5c266669663f9a1dbcb2377086`  
		Last Modified: Sat, 28 May 2022 05:21:37 GMT  
		Size: 17.0 MB (17038480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b893d548ee02faada4ffcfce881ee9a9d8e144b1d052d85e14338a10a584f73f`  
		Last Modified: Sat, 28 May 2022 05:21:33 GMT  
		Size: 4.2 KB (4213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78daf0e1ebbead3bdba065457c48d6a82da6191e098a16e5b228c56e2079d10`  
		Last Modified: Sat, 28 May 2022 05:21:35 GMT  
		Size: 6.4 MB (6433419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v5

```console
$ docker pull irssi@sha256:319e7359b22812fedb09a44d23cd11e0da8e2764a1f58117d086cb28b1efbfae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46896517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece64e4b9eb38841094e52414e2eb69af1f67124e41ae31ab7f4eb05e168e822`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 02:04:06 GMT
ADD file:26e9ed6c41ec12bf5fd602b7f86b924d34537bbc82442f630763f9f6c48bf3b3 in / 
# Sat, 28 May 2022 02:04:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:51:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:51:33 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 03:51:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 03:51:35 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 03:51:35 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 03:53:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 03:53:30 GMT
WORKDIR /home/user
# Sat, 28 May 2022 03:53:30 GMT
USER user
# Sat, 28 May 2022 03:53:31 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:19389fd1100abdedaa775b43242838cdd2d5c8c3388643a7e52da2b7b4399c15`  
		Last Modified: Sat, 28 May 2022 02:20:06 GMT  
		Size: 24.9 MB (24890069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc97e5088dad5dd24e65c10e4ea9e411d109a92d2e5ea0ea963e08e311ad796`  
		Last Modified: Sat, 28 May 2022 03:54:27 GMT  
		Size: 15.9 MB (15937730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4a37ba27a89a967fe9c2d2f15f8e694a897f7ce14473c47467a7d1fee1f5eb`  
		Last Modified: Sat, 28 May 2022 03:54:12 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a75a4f2bb09f772d8125095f28993565ba0cedf1ea7e623d06819383b74dd`  
		Last Modified: Sat, 28 May 2022 03:54:16 GMT  
		Size: 6.1 MB (6064521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4cf05cf78af130b124c2677cfc8a08fb5b49ee61ef19ee43cf5aa7d668ea8609
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44283091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bde88159cecf11997b4d861c8ce640cc9e4dc449048d1436268d80152d736f`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:00:54 GMT
ADD file:c89d47099a38749a424760d9c7d3a6e982089455ba9d04140db15ba9eb4cdda1 in / 
# Sat, 28 May 2022 01:00:55 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:32:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:33:00 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 07:33:02 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 07:33:02 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 07:33:02 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 07:34:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 07:34:50 GMT
WORKDIR /home/user
# Sat, 28 May 2022 07:34:50 GMT
USER user
# Sat, 28 May 2022 07:34:51 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e41117292dc8c199b63ae1ec4485358841dbcba68dcbd13f379b66182efe832e`  
		Last Modified: Sat, 28 May 2022 01:16:58 GMT  
		Size: 22.7 MB (22748097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3818c0c31072687a62a285a3582a6ac59a7e9c1c0d84423739dafb09cd2f397`  
		Last Modified: Sat, 28 May 2022 07:36:12 GMT  
		Size: 15.6 MB (15598239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c30d93b9a282c1f30a84b17541b5cb2b05cdbced870f4f1f7097d1c79985ee`  
		Last Modified: Sat, 28 May 2022 07:35:57 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22736721f72dfd763c95b664b3afb4327c73190f4bf5230c40283d02328701eb`  
		Last Modified: Sat, 28 May 2022 07:36:00 GMT  
		Size: 5.9 MB (5932564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:93331fad416045665e2b6bfb19606ccc3e2da9ab35ac8e4f3e359d9d8564efa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48908753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d67ac80f549afca6223607f6df4382b1f3caefa46171f8129e47175a13833c`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 00:41:05 GMT
ADD file:d0e42d603f275c040783ec7b6c051200815492fc35b73110234dfcd584e6cdec in / 
# Sat, 28 May 2022 00:41:05 GMT
CMD ["bash"]
# Sat, 28 May 2022 13:07:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 13:07:23 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 13:07:24 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 13:07:25 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 13:07:26 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 13:08:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 13:08:08 GMT
WORKDIR /home/user
# Sat, 28 May 2022 13:08:09 GMT
USER user
# Sat, 28 May 2022 13:08:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4931fb8ba4223cb35034141162105ee5482122692b2931eb69eec912ce64606d`  
		Last Modified: Sat, 28 May 2022 00:48:26 GMT  
		Size: 25.9 MB (25914033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578f8e8c703cdf2c34f2aacd16e83af9040d1c923427dc5fe10fff3969b17983`  
		Last Modified: Sat, 28 May 2022 13:08:49 GMT  
		Size: 16.8 MB (16814580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dba055597f3b5e93280156ec02d53a40d9604ae8e34f7b120795b251f0adab`  
		Last Modified: Sat, 28 May 2022 13:08:46 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1655e15c8cad9556df1295427409be5707ebc949b480830c26e363b0b146534c`  
		Last Modified: Sat, 28 May 2022 13:08:47 GMT  
		Size: 6.2 MB (6176068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; 386

```console
$ docker pull irssi@sha256:f87197bcb070dc6091ab19977c431f3e95e762098396a327d292f019ddb5dc0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50263361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c22d8c0a1d40fa9e5af5c700fc4e768e9277eb28e82bad9f5bbafd0fb48def2e`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 00:40:01 GMT
ADD file:9aea7a35c215cdd778adec1dd5213973ef9b4830110e4550f2ead85679551ee5 in / 
# Sat, 28 May 2022 00:40:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 12:36:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 12:36:40 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 12:36:41 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 12:36:42 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 12:36:43 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 12:37:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 12:37:28 GMT
WORKDIR /home/user
# Sat, 28 May 2022 12:37:29 GMT
USER user
# Sat, 28 May 2022 12:37:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:40837b3d848885c0b0c031d6d950b38e6a26962a5ee49704cb3ca2d2db535617`  
		Last Modified: Sat, 28 May 2022 00:47:36 GMT  
		Size: 27.8 MB (27799572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd85652cb7aee11a1ee235bfe214f30f2eed4280ecc94c7721326d13bbaeaf`  
		Last Modified: Sat, 28 May 2022 12:38:05 GMT  
		Size: 16.6 MB (16566304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c056bbb0e1c559600ab3a62c0b4cb4e41e2277f340915f3e120c990c97bafa84`  
		Last Modified: Sat, 28 May 2022 12:38:02 GMT  
		Size: 4.1 KB (4058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9f8088df3ca5683e0a6dfe2a6aaf868428ecfcbef01b067549522f8b11e93`  
		Last Modified: Sat, 28 May 2022 12:38:03 GMT  
		Size: 5.9 MB (5893427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; mips64le

```console
$ docker pull irssi@sha256:4bf810ff969b5912a5e687a4c44aa741870b792ff2ec4a48afa82cf959023d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47631105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b4d731d65f3d51d2dfe09f12efe86b3963cdc36b44461ec2373fa54942db31`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:12:21 GMT
ADD file:12eb3f58e1c47ef1af98f481c1f5f33832f45144bf66f3a01065f8c939f1eaa9 in / 
# Sat, 28 May 2022 01:12:25 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:15:46 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 03:15:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 03:15:57 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 03:16:00 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 03:20:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 03:20:30 GMT
WORKDIR /home/user
# Sat, 28 May 2022 03:20:33 GMT
USER user
# Sat, 28 May 2022 03:20:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:79a954ba282b6c17b5d2fdc4563e0fbc4bf4e3c673bada0b2f656937656557eb`  
		Last Modified: Sat, 28 May 2022 01:22:56 GMT  
		Size: 25.8 MB (25814580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad211fee54c5f12de817e949479da0f9fa7e5923811567b7286c6050032245fc`  
		Last Modified: Sat, 28 May 2022 03:21:16 GMT  
		Size: 15.7 MB (15732112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805cb834a6e653d97de303cfc43b9da9082614eb08397f22b596a004b9532474`  
		Last Modified: Sat, 28 May 2022 03:21:02 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edb471e3b1d4a83905a6a5c109848bbdf1f68055b04cc7a6763006a14dfc474`  
		Last Modified: Sat, 28 May 2022 03:21:06 GMT  
		Size: 6.1 MB (6080339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; ppc64le

```console
$ docker pull irssi@sha256:e39d45ef70272a2e6cf18c9dd66d12ee70a3645f2046b11496743d0cd865deca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54787987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baff97fede43b1fb6e3ca8de715b96fc263414eedea56bd2b0051990c5ed73d9`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:23:57 GMT
ADD file:a8c6c897bc64da424049ad04a354d123b0622abda1a56b2725f72de5e4569df8 in / 
# Sat, 28 May 2022 01:24:04 GMT
CMD ["bash"]
# Sat, 28 May 2022 06:52:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 06:52:32 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 06:52:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 06:52:38 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 06:52:41 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 06:57:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 06:57:14 GMT
WORKDIR /home/user
# Sat, 28 May 2022 06:57:16 GMT
USER user
# Sat, 28 May 2022 06:57:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:087d40850259bdcd3bee3d5d30d5a2070216727f72c1c9731b514ac3dbf7573e`  
		Last Modified: Sat, 28 May 2022 01:33:30 GMT  
		Size: 30.6 MB (30560238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e180ca0caaecd96894d59df3140df02564c778c40d46b6d03f0fda10eefa6d35`  
		Last Modified: Sat, 28 May 2022 06:58:03 GMT  
		Size: 17.4 MB (17440702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932bc69b6c04fbdc83f98628214743c0e6645a14a5adb34acc1d5590c38d360`  
		Last Modified: Sat, 28 May 2022 06:57:58 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf716870602840820cee5bb11e395b8197b4435e92d9213dba7ad4456818e16`  
		Last Modified: Sat, 28 May 2022 06:58:00 GMT  
		Size: 6.8 MB (6782838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2` - linux; s390x

```console
$ docker pull irssi@sha256:6babbc57189870e9c78763f97de83c067a89b24ddac49f302b21504254e0da1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49061887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b289242502c712e59b5bc78e77d30bad09363d5bdbf1da235ab944c5f4a4393`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 May 2022 00:44:47 GMT
ADD file:28b1e60f65391906bebd81248a4da766172138fab99b8b9e6b18bce76afea02d in / 
# Wed, 11 May 2022 00:44:49 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:29:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:29:57 GMT
ENV HOME=/home/user
# Wed, 11 May 2022 02:29:58 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 May 2022 02:29:58 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 02:29:58 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 11 May 2022 02:30:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 May 2022 02:30:37 GMT
WORKDIR /home/user
# Wed, 11 May 2022 02:30:37 GMT
USER user
# Wed, 11 May 2022 02:30:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bf64474a39a67000556a4502abd4584010a062b942cf8e2545d0502d38ffa150`  
		Last Modified: Wed, 11 May 2022 00:50:43 GMT  
		Size: 25.8 MB (25758738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bab2a510dcd371ba308d88b7a421f4392242a1145a5e2032557bff64f1f3096`  
		Last Modified: Wed, 11 May 2022 02:31:19 GMT  
		Size: 16.9 MB (16914219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114f12ef452583e1b53623df64e6ed1ef5fe101a2bd32bcb5670547708d201b1`  
		Last Modified: Wed, 11 May 2022 02:31:16 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3872a1d35d40ae59cc2e54813e37c9cd0c725b5df75a8e79c674d79cfed86c`  
		Last Modified: Wed, 11 May 2022 02:31:17 GMT  
		Size: 6.4 MB (6384718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2-alpine`

```console
$ docker pull irssi@sha256:bfbb6e415dbf4cd1ea2d6bd42bdcc5fcc054d6b053c6d07b983c9b390dac8f9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.2-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:c38f2415219abd42abe51fa4eaf222d8d7c7bdebb86910500d59bb7d0c21b231
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c0676773ef4ea9992d62133ac02ba861fde6dd9ba437e8fb36eaf4aae78852`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:16 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 11:18:17 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 11:18:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 11:18:17 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:18:17 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 11:19:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 11:19:01 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 11:19:01 GMT
USER user
# Tue, 05 Apr 2022 11:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa1dbdb27d63340f8b8fa494a282aeded5f878185e2847d6dfb481b353b8c11`  
		Last Modified: Tue, 05 Apr 2022 11:19:27 GMT  
		Size: 9.5 MB (9540662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd245485e0307925fa298d8f511fe481b6600ce336c8ff0a0b5c13ce1435d9`  
		Last Modified: Tue, 05 Apr 2022 11:19:24 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4513426f1a6993290c7fa1e95a9f0bd0309456d69e3c04c0a7e8b17b66c9a079`  
		Last Modified: Tue, 05 Apr 2022 11:19:25 GMT  
		Size: 6.3 MB (6287259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:5262462a3f32457835863ac8b11823de2d926d672219bdff8c5c67bc5e116e2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab49acd659041f4c479472bb7ed35e0fc93656b968625544d96599e44c57c01`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:01:19 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:01:20 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:01:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:01:22 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:01:22 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:02:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:02:32 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:02:32 GMT
USER user
# Tue, 05 Apr 2022 04:02:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b589ee3c7baf4a3043d5c498c04269109c4a45e58c44ab98b5a969b7ba2f8a`  
		Last Modified: Tue, 05 Apr 2022 04:03:13 GMT  
		Size: 8.8 MB (8771955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82acf7c178275d848adf6769cd6193b1f701750ef2bf058c507c10c4af90080d`  
		Last Modified: Tue, 05 Apr 2022 04:03:05 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391da21a1ce4611cc08325dc363346ea9ae04e1724386ad9b1a8801e1843e835`  
		Last Modified: Tue, 05 Apr 2022 04:03:09 GMT  
		Size: 6.0 MB (5987042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:85b6871234efe5afa8aee356cecfc27abb04e6a99f43a969eedce41a3230299b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f387771b9c45b2879b4d36faf8f6326c4b27afacac146e4d774c52b2d0f103cb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:58:06 GMT
ADD file:0834e20e80add8b1c6bd545ebe0729239e00a4dff08b025cb5555cd3ce58e4c6 in / 
# Mon, 04 Apr 2022 23:58:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:02:01 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 16:02:01 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 16:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 16:02:03 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:02:04 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 16:03:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 16:03:10 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 16:03:10 GMT
USER user
# Tue, 05 Apr 2022 16:03:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a8b8a1c7a552f6893757dd6327a5a430981d78aa06a59298076603526186829e`  
		Last Modified: Mon, 04 Apr 2022 23:59:56 GMT  
		Size: 2.4 MB (2427836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0c71a12aa1dc1147bd41cf6458906772bf77be69de2e8fc3d9242f641fc445`  
		Last Modified: Tue, 05 Apr 2022 16:04:19 GMT  
		Size: 8.6 MB (8626381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf67fa3e83093b4230c7f24388cfb9f6f9aa8bd3c5d76434f7b058a66d7ab80`  
		Last Modified: Tue, 05 Apr 2022 16:04:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a6a97274960e7695eb8d37b680b0fe6bc45a12b2b550e310504260e923285`  
		Last Modified: Tue, 05 Apr 2022 16:04:15 GMT  
		Size: 5.8 MB (5783964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:d49fa5e7d3a8cd10c7bfad3e9bec2fa37e6a44c2911c1958c7014a121f4eef59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98cf9f811eb592e3b8c251eb41f7f7dfdadc8c7b6dc2e9fae2c2d835173d8ac`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:14:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:14:16 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:14:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:14:18 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:14:19 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:14:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:14:54 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:14:55 GMT
USER user
# Tue, 05 Apr 2022 04:14:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f125d0f2f3de8f4307e1218e71620016554b5120c8ce30e8786904dc74366d0b`  
		Last Modified: Tue, 05 Apr 2022 04:15:25 GMT  
		Size: 9.5 MB (9536419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c48a8193426a12a478ffa39f46aa61977b41d48a60d252930c3c2a4708fd0b7`  
		Last Modified: Tue, 05 Apr 2022 04:15:23 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7a5707b30c726d92bca84220a2cb23b4ff000e7119f0a696975a866269d135`  
		Last Modified: Tue, 05 Apr 2022 04:15:24 GMT  
		Size: 6.2 MB (6247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; 386

```console
$ docker pull irssi@sha256:f4044a89fe2a5119671314da6e8cbfed9929c215d20d677e6b84a7e5b713611f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17704054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aea095e2938971334ab2464fcf39c254bd75a69e3b56999f7fab374fb813c92`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:47:49 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 06:47:49 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 06:47:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 06:47:51 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 06:47:52 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 06:48:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 06:48:28 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 06:48:29 GMT
USER user
# Tue, 05 Apr 2022 06:48:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d17b6eaf713c06aeabfe2feac029d7c880865cf49ab0c148c784791c31779`  
		Last Modified: Tue, 05 Apr 2022 06:49:01 GMT  
		Size: 8.9 MB (8904271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831ba5a4f1fc534f7dec6b2cf96d9935df1d6b00524538974d10799fd6f4c53`  
		Last Modified: Tue, 05 Apr 2022 06:48:59 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3dd29c50ebba7606220a2a714a5fdb3059694e3f39c9b707f4c43086cf958`  
		Last Modified: Tue, 05 Apr 2022 06:49:00 GMT  
		Size: 6.0 MB (5978011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:beba11d08d6df10a4fe4518b49c2e3d8b54f2cb9f15feb8bce4bfba5d97c6674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37da7ed44ea84c9ebfb079e981447b44fccab806fd3be499c492a079908bf21d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:10:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 19:10:11 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 19:10:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 19:10:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 19:10:29 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 19:11:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 19:11:33 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 19:11:36 GMT
USER user
# Tue, 05 Apr 2022 19:11:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73fa56481e3f5fd84b721b288e4628ef18d832025ab22c2cb0601f85d9025b`  
		Last Modified: Tue, 05 Apr 2022 19:12:17 GMT  
		Size: 9.6 MB (9632765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2998f1c0df5727d61352cf5bbb86f17a2b07e8d0feef2892ad0c1a13693ed8`  
		Last Modified: Tue, 05 Apr 2022 19:12:15 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0ce73fb7b2975452460737c989e296843d87ad3f26c26f5c7df696df51a1ea`  
		Last Modified: Tue, 05 Apr 2022 19:12:16 GMT  
		Size: 6.5 MB (6492183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:07e9626c05472af1fce5448f4310a04d7bc5e3a7e6a4384227d5aaec02d65705
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18855197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5ea35b9201821c8168c1b19f5a926438127784e392a0465b5a49bc2b7f98e1`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:58:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 03:58:35 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 03:58:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 03:58:36 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:58:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 03:59:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 03:59:07 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 03:59:07 GMT
USER user
# Tue, 05 Apr 2022 03:59:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2a655edb7398e76b909cbb12baf208d875c598793a42546c8f2b906ab8e2c7`  
		Last Modified: Tue, 05 Apr 2022 03:59:36 GMT  
		Size: 10.0 MB (9972200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16218c4743041a59790e9a6b9388344940cd9dbf0e8c3cff8ea17486b32b553`  
		Last Modified: Tue, 05 Apr 2022 03:59:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e5f35e6bfccd90acff05f4db673effe1dce4f736f0d128d6e878f5524767`  
		Last Modified: Tue, 05 Apr 2022 03:59:35 GMT  
		Size: 6.3 MB (6276668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3`

```console
$ docker pull irssi@sha256:9e19096cc30c331015cc1e4ebb3a4f11967adb7c2ae52aa11dc775f90441605f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.2.3` - linux; amd64

```console
$ docker pull irssi@sha256:9b8e794c52606ddb03386ca63e00b8822bb0422ba8d1bbc1f6a91b1169badcf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50616256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d9bf5187a352d791a3be64008fab00c63e5153e65db45b19b848fafffa65e7`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:20:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:20:24 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 05:20:25 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 05:20:25 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 05:20:25 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 05:21:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 05:21:09 GMT
WORKDIR /home/user
# Sat, 28 May 2022 05:21:09 GMT
USER user
# Sat, 28 May 2022 05:21:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1afda879f82264f53bd7206d0529f22e6289f5c266669663f9a1dbcb2377086`  
		Last Modified: Sat, 28 May 2022 05:21:37 GMT  
		Size: 17.0 MB (17038480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b893d548ee02faada4ffcfce881ee9a9d8e144b1d052d85e14338a10a584f73f`  
		Last Modified: Sat, 28 May 2022 05:21:33 GMT  
		Size: 4.2 KB (4213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78daf0e1ebbead3bdba065457c48d6a82da6191e098a16e5b228c56e2079d10`  
		Last Modified: Sat, 28 May 2022 05:21:35 GMT  
		Size: 6.4 MB (6433419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm variant v5

```console
$ docker pull irssi@sha256:319e7359b22812fedb09a44d23cd11e0da8e2764a1f58117d086cb28b1efbfae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46896517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece64e4b9eb38841094e52414e2eb69af1f67124e41ae31ab7f4eb05e168e822`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 02:04:06 GMT
ADD file:26e9ed6c41ec12bf5fd602b7f86b924d34537bbc82442f630763f9f6c48bf3b3 in / 
# Sat, 28 May 2022 02:04:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:51:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:51:33 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 03:51:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 03:51:35 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 03:51:35 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 03:53:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 03:53:30 GMT
WORKDIR /home/user
# Sat, 28 May 2022 03:53:30 GMT
USER user
# Sat, 28 May 2022 03:53:31 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:19389fd1100abdedaa775b43242838cdd2d5c8c3388643a7e52da2b7b4399c15`  
		Last Modified: Sat, 28 May 2022 02:20:06 GMT  
		Size: 24.9 MB (24890069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc97e5088dad5dd24e65c10e4ea9e411d109a92d2e5ea0ea963e08e311ad796`  
		Last Modified: Sat, 28 May 2022 03:54:27 GMT  
		Size: 15.9 MB (15937730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4a37ba27a89a967fe9c2d2f15f8e694a897f7ce14473c47467a7d1fee1f5eb`  
		Last Modified: Sat, 28 May 2022 03:54:12 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a75a4f2bb09f772d8125095f28993565ba0cedf1ea7e623d06819383b74dd`  
		Last Modified: Sat, 28 May 2022 03:54:16 GMT  
		Size: 6.1 MB (6064521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4cf05cf78af130b124c2677cfc8a08fb5b49ee61ef19ee43cf5aa7d668ea8609
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44283091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bde88159cecf11997b4d861c8ce640cc9e4dc449048d1436268d80152d736f`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:00:54 GMT
ADD file:c89d47099a38749a424760d9c7d3a6e982089455ba9d04140db15ba9eb4cdda1 in / 
# Sat, 28 May 2022 01:00:55 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:32:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:33:00 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 07:33:02 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 07:33:02 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 07:33:02 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 07:34:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 07:34:50 GMT
WORKDIR /home/user
# Sat, 28 May 2022 07:34:50 GMT
USER user
# Sat, 28 May 2022 07:34:51 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e41117292dc8c199b63ae1ec4485358841dbcba68dcbd13f379b66182efe832e`  
		Last Modified: Sat, 28 May 2022 01:16:58 GMT  
		Size: 22.7 MB (22748097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3818c0c31072687a62a285a3582a6ac59a7e9c1c0d84423739dafb09cd2f397`  
		Last Modified: Sat, 28 May 2022 07:36:12 GMT  
		Size: 15.6 MB (15598239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c30d93b9a282c1f30a84b17541b5cb2b05cdbced870f4f1f7097d1c79985ee`  
		Last Modified: Sat, 28 May 2022 07:35:57 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22736721f72dfd763c95b664b3afb4327c73190f4bf5230c40283d02328701eb`  
		Last Modified: Sat, 28 May 2022 07:36:00 GMT  
		Size: 5.9 MB (5932564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:93331fad416045665e2b6bfb19606ccc3e2da9ab35ac8e4f3e359d9d8564efa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48908753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d67ac80f549afca6223607f6df4382b1f3caefa46171f8129e47175a13833c`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 00:41:05 GMT
ADD file:d0e42d603f275c040783ec7b6c051200815492fc35b73110234dfcd584e6cdec in / 
# Sat, 28 May 2022 00:41:05 GMT
CMD ["bash"]
# Sat, 28 May 2022 13:07:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 13:07:23 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 13:07:24 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 13:07:25 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 13:07:26 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 13:08:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 13:08:08 GMT
WORKDIR /home/user
# Sat, 28 May 2022 13:08:09 GMT
USER user
# Sat, 28 May 2022 13:08:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4931fb8ba4223cb35034141162105ee5482122692b2931eb69eec912ce64606d`  
		Last Modified: Sat, 28 May 2022 00:48:26 GMT  
		Size: 25.9 MB (25914033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578f8e8c703cdf2c34f2aacd16e83af9040d1c923427dc5fe10fff3969b17983`  
		Last Modified: Sat, 28 May 2022 13:08:49 GMT  
		Size: 16.8 MB (16814580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dba055597f3b5e93280156ec02d53a40d9604ae8e34f7b120795b251f0adab`  
		Last Modified: Sat, 28 May 2022 13:08:46 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1655e15c8cad9556df1295427409be5707ebc949b480830c26e363b0b146534c`  
		Last Modified: Sat, 28 May 2022 13:08:47 GMT  
		Size: 6.2 MB (6176068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; 386

```console
$ docker pull irssi@sha256:f87197bcb070dc6091ab19977c431f3e95e762098396a327d292f019ddb5dc0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50263361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c22d8c0a1d40fa9e5af5c700fc4e768e9277eb28e82bad9f5bbafd0fb48def2e`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 00:40:01 GMT
ADD file:9aea7a35c215cdd778adec1dd5213973ef9b4830110e4550f2ead85679551ee5 in / 
# Sat, 28 May 2022 00:40:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 12:36:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 12:36:40 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 12:36:41 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 12:36:42 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 12:36:43 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 12:37:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 12:37:28 GMT
WORKDIR /home/user
# Sat, 28 May 2022 12:37:29 GMT
USER user
# Sat, 28 May 2022 12:37:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:40837b3d848885c0b0c031d6d950b38e6a26962a5ee49704cb3ca2d2db535617`  
		Last Modified: Sat, 28 May 2022 00:47:36 GMT  
		Size: 27.8 MB (27799572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd85652cb7aee11a1ee235bfe214f30f2eed4280ecc94c7721326d13bbaeaf`  
		Last Modified: Sat, 28 May 2022 12:38:05 GMT  
		Size: 16.6 MB (16566304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c056bbb0e1c559600ab3a62c0b4cb4e41e2277f340915f3e120c990c97bafa84`  
		Last Modified: Sat, 28 May 2022 12:38:02 GMT  
		Size: 4.1 KB (4058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9f8088df3ca5683e0a6dfe2a6aaf868428ecfcbef01b067549522f8b11e93`  
		Last Modified: Sat, 28 May 2022 12:38:03 GMT  
		Size: 5.9 MB (5893427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; mips64le

```console
$ docker pull irssi@sha256:4bf810ff969b5912a5e687a4c44aa741870b792ff2ec4a48afa82cf959023d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47631105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b4d731d65f3d51d2dfe09f12efe86b3963cdc36b44461ec2373fa54942db31`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:12:21 GMT
ADD file:12eb3f58e1c47ef1af98f481c1f5f33832f45144bf66f3a01065f8c939f1eaa9 in / 
# Sat, 28 May 2022 01:12:25 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:15:46 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 03:15:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 03:15:57 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 03:16:00 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 03:20:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 03:20:30 GMT
WORKDIR /home/user
# Sat, 28 May 2022 03:20:33 GMT
USER user
# Sat, 28 May 2022 03:20:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:79a954ba282b6c17b5d2fdc4563e0fbc4bf4e3c673bada0b2f656937656557eb`  
		Last Modified: Sat, 28 May 2022 01:22:56 GMT  
		Size: 25.8 MB (25814580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad211fee54c5f12de817e949479da0f9fa7e5923811567b7286c6050032245fc`  
		Last Modified: Sat, 28 May 2022 03:21:16 GMT  
		Size: 15.7 MB (15732112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805cb834a6e653d97de303cfc43b9da9082614eb08397f22b596a004b9532474`  
		Last Modified: Sat, 28 May 2022 03:21:02 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edb471e3b1d4a83905a6a5c109848bbdf1f68055b04cc7a6763006a14dfc474`  
		Last Modified: Sat, 28 May 2022 03:21:06 GMT  
		Size: 6.1 MB (6080339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; ppc64le

```console
$ docker pull irssi@sha256:e39d45ef70272a2e6cf18c9dd66d12ee70a3645f2046b11496743d0cd865deca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54787987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baff97fede43b1fb6e3ca8de715b96fc263414eedea56bd2b0051990c5ed73d9`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:23:57 GMT
ADD file:a8c6c897bc64da424049ad04a354d123b0622abda1a56b2725f72de5e4569df8 in / 
# Sat, 28 May 2022 01:24:04 GMT
CMD ["bash"]
# Sat, 28 May 2022 06:52:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 06:52:32 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 06:52:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 06:52:38 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 06:52:41 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 06:57:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 06:57:14 GMT
WORKDIR /home/user
# Sat, 28 May 2022 06:57:16 GMT
USER user
# Sat, 28 May 2022 06:57:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:087d40850259bdcd3bee3d5d30d5a2070216727f72c1c9731b514ac3dbf7573e`  
		Last Modified: Sat, 28 May 2022 01:33:30 GMT  
		Size: 30.6 MB (30560238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e180ca0caaecd96894d59df3140df02564c778c40d46b6d03f0fda10eefa6d35`  
		Last Modified: Sat, 28 May 2022 06:58:03 GMT  
		Size: 17.4 MB (17440702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932bc69b6c04fbdc83f98628214743c0e6645a14a5adb34acc1d5590c38d360`  
		Last Modified: Sat, 28 May 2022 06:57:58 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf716870602840820cee5bb11e395b8197b4435e92d9213dba7ad4456818e16`  
		Last Modified: Sat, 28 May 2022 06:58:00 GMT  
		Size: 6.8 MB (6782838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3` - linux; s390x

```console
$ docker pull irssi@sha256:6babbc57189870e9c78763f97de83c067a89b24ddac49f302b21504254e0da1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49061887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b289242502c712e59b5bc78e77d30bad09363d5bdbf1da235ab944c5f4a4393`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 May 2022 00:44:47 GMT
ADD file:28b1e60f65391906bebd81248a4da766172138fab99b8b9e6b18bce76afea02d in / 
# Wed, 11 May 2022 00:44:49 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:29:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:29:57 GMT
ENV HOME=/home/user
# Wed, 11 May 2022 02:29:58 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 May 2022 02:29:58 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 02:29:58 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 11 May 2022 02:30:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 May 2022 02:30:37 GMT
WORKDIR /home/user
# Wed, 11 May 2022 02:30:37 GMT
USER user
# Wed, 11 May 2022 02:30:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bf64474a39a67000556a4502abd4584010a062b942cf8e2545d0502d38ffa150`  
		Last Modified: Wed, 11 May 2022 00:50:43 GMT  
		Size: 25.8 MB (25758738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bab2a510dcd371ba308d88b7a421f4392242a1145a5e2032557bff64f1f3096`  
		Last Modified: Wed, 11 May 2022 02:31:19 GMT  
		Size: 16.9 MB (16914219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114f12ef452583e1b53623df64e6ed1ef5fe101a2bd32bcb5670547708d201b1`  
		Last Modified: Wed, 11 May 2022 02:31:16 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3872a1d35d40ae59cc2e54813e37c9cd0c725b5df75a8e79c674d79cfed86c`  
		Last Modified: Wed, 11 May 2022 02:31:17 GMT  
		Size: 6.4 MB (6384718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:1.2.3-alpine`

```console
$ docker pull irssi@sha256:bfbb6e415dbf4cd1ea2d6bd42bdcc5fcc054d6b053c6d07b983c9b390dac8f9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:1.2.3-alpine` - linux; amd64

```console
$ docker pull irssi@sha256:c38f2415219abd42abe51fa4eaf222d8d7c7bdebb86910500d59bb7d0c21b231
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c0676773ef4ea9992d62133ac02ba861fde6dd9ba437e8fb36eaf4aae78852`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:16 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 11:18:17 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 11:18:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 11:18:17 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:18:17 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 11:19:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 11:19:01 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 11:19:01 GMT
USER user
# Tue, 05 Apr 2022 11:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa1dbdb27d63340f8b8fa494a282aeded5f878185e2847d6dfb481b353b8c11`  
		Last Modified: Tue, 05 Apr 2022 11:19:27 GMT  
		Size: 9.5 MB (9540662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd245485e0307925fa298d8f511fe481b6600ce336c8ff0a0b5c13ce1435d9`  
		Last Modified: Tue, 05 Apr 2022 11:19:24 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4513426f1a6993290c7fa1e95a9f0bd0309456d69e3c04c0a7e8b17b66c9a079`  
		Last Modified: Tue, 05 Apr 2022 11:19:25 GMT  
		Size: 6.3 MB (6287259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:5262462a3f32457835863ac8b11823de2d926d672219bdff8c5c67bc5e116e2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab49acd659041f4c479472bb7ed35e0fc93656b968625544d96599e44c57c01`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:01:19 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:01:20 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:01:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:01:22 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:01:22 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:02:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:02:32 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:02:32 GMT
USER user
# Tue, 05 Apr 2022 04:02:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b589ee3c7baf4a3043d5c498c04269109c4a45e58c44ab98b5a969b7ba2f8a`  
		Last Modified: Tue, 05 Apr 2022 04:03:13 GMT  
		Size: 8.8 MB (8771955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82acf7c178275d848adf6769cd6193b1f701750ef2bf058c507c10c4af90080d`  
		Last Modified: Tue, 05 Apr 2022 04:03:05 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391da21a1ce4611cc08325dc363346ea9ae04e1724386ad9b1a8801e1843e835`  
		Last Modified: Tue, 05 Apr 2022 04:03:09 GMT  
		Size: 6.0 MB (5987042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:85b6871234efe5afa8aee356cecfc27abb04e6a99f43a969eedce41a3230299b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f387771b9c45b2879b4d36faf8f6326c4b27afacac146e4d774c52b2d0f103cb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:58:06 GMT
ADD file:0834e20e80add8b1c6bd545ebe0729239e00a4dff08b025cb5555cd3ce58e4c6 in / 
# Mon, 04 Apr 2022 23:58:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:02:01 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 16:02:01 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 16:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 16:02:03 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:02:04 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 16:03:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 16:03:10 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 16:03:10 GMT
USER user
# Tue, 05 Apr 2022 16:03:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a8b8a1c7a552f6893757dd6327a5a430981d78aa06a59298076603526186829e`  
		Last Modified: Mon, 04 Apr 2022 23:59:56 GMT  
		Size: 2.4 MB (2427836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0c71a12aa1dc1147bd41cf6458906772bf77be69de2e8fc3d9242f641fc445`  
		Last Modified: Tue, 05 Apr 2022 16:04:19 GMT  
		Size: 8.6 MB (8626381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf67fa3e83093b4230c7f24388cfb9f6f9aa8bd3c5d76434f7b058a66d7ab80`  
		Last Modified: Tue, 05 Apr 2022 16:04:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a6a97274960e7695eb8d37b680b0fe6bc45a12b2b550e310504260e923285`  
		Last Modified: Tue, 05 Apr 2022 16:04:15 GMT  
		Size: 5.8 MB (5783964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:d49fa5e7d3a8cd10c7bfad3e9bec2fa37e6a44c2911c1958c7014a121f4eef59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98cf9f811eb592e3b8c251eb41f7f7dfdadc8c7b6dc2e9fae2c2d835173d8ac`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:14:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:14:16 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:14:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:14:18 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:14:19 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:14:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:14:54 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:14:55 GMT
USER user
# Tue, 05 Apr 2022 04:14:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f125d0f2f3de8f4307e1218e71620016554b5120c8ce30e8786904dc74366d0b`  
		Last Modified: Tue, 05 Apr 2022 04:15:25 GMT  
		Size: 9.5 MB (9536419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c48a8193426a12a478ffa39f46aa61977b41d48a60d252930c3c2a4708fd0b7`  
		Last Modified: Tue, 05 Apr 2022 04:15:23 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7a5707b30c726d92bca84220a2cb23b4ff000e7119f0a696975a866269d135`  
		Last Modified: Tue, 05 Apr 2022 04:15:24 GMT  
		Size: 6.2 MB (6247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; 386

```console
$ docker pull irssi@sha256:f4044a89fe2a5119671314da6e8cbfed9929c215d20d677e6b84a7e5b713611f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17704054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aea095e2938971334ab2464fcf39c254bd75a69e3b56999f7fab374fb813c92`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:47:49 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 06:47:49 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 06:47:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 06:47:51 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 06:47:52 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 06:48:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 06:48:28 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 06:48:29 GMT
USER user
# Tue, 05 Apr 2022 06:48:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d17b6eaf713c06aeabfe2feac029d7c880865cf49ab0c148c784791c31779`  
		Last Modified: Tue, 05 Apr 2022 06:49:01 GMT  
		Size: 8.9 MB (8904271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831ba5a4f1fc534f7dec6b2cf96d9935df1d6b00524538974d10799fd6f4c53`  
		Last Modified: Tue, 05 Apr 2022 06:48:59 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3dd29c50ebba7606220a2a714a5fdb3059694e3f39c9b707f4c43086cf958`  
		Last Modified: Tue, 05 Apr 2022 06:49:00 GMT  
		Size: 6.0 MB (5978011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:beba11d08d6df10a4fe4518b49c2e3d8b54f2cb9f15feb8bce4bfba5d97c6674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37da7ed44ea84c9ebfb079e981447b44fccab806fd3be499c492a079908bf21d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:10:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 19:10:11 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 19:10:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 19:10:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 19:10:29 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 19:11:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 19:11:33 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 19:11:36 GMT
USER user
# Tue, 05 Apr 2022 19:11:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73fa56481e3f5fd84b721b288e4628ef18d832025ab22c2cb0601f85d9025b`  
		Last Modified: Tue, 05 Apr 2022 19:12:17 GMT  
		Size: 9.6 MB (9632765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2998f1c0df5727d61352cf5bbb86f17a2b07e8d0feef2892ad0c1a13693ed8`  
		Last Modified: Tue, 05 Apr 2022 19:12:15 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0ce73fb7b2975452460737c989e296843d87ad3f26c26f5c7df696df51a1ea`  
		Last Modified: Tue, 05 Apr 2022 19:12:16 GMT  
		Size: 6.5 MB (6492183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:1.2.3-alpine` - linux; s390x

```console
$ docker pull irssi@sha256:07e9626c05472af1fce5448f4310a04d7bc5e3a7e6a4384227d5aaec02d65705
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18855197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5ea35b9201821c8168c1b19f5a926438127784e392a0465b5a49bc2b7f98e1`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:58:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 03:58:35 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 03:58:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 03:58:36 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:58:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 03:59:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 03:59:07 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 03:59:07 GMT
USER user
# Tue, 05 Apr 2022 03:59:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2a655edb7398e76b909cbb12baf208d875c598793a42546c8f2b906ab8e2c7`  
		Last Modified: Tue, 05 Apr 2022 03:59:36 GMT  
		Size: 10.0 MB (9972200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16218c4743041a59790e9a6b9388344940cd9dbf0e8c3cff8ea17486b32b553`  
		Last Modified: Tue, 05 Apr 2022 03:59:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e5f35e6bfccd90acff05f4db673effe1dce4f736f0d128d6e878f5524767`  
		Last Modified: Tue, 05 Apr 2022 03:59:35 GMT  
		Size: 6.3 MB (6276668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:alpine`

```console
$ docker pull irssi@sha256:bfbb6e415dbf4cd1ea2d6bd42bdcc5fcc054d6b053c6d07b983c9b390dac8f9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `irssi:alpine` - linux; amd64

```console
$ docker pull irssi@sha256:c38f2415219abd42abe51fa4eaf222d8d7c7bdebb86910500d59bb7d0c21b231
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18648499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c0676773ef4ea9992d62133ac02ba861fde6dd9ba437e8fb36eaf4aae78852`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:16 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 11:18:17 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 11:18:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 11:18:17 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 11:18:17 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 11:19:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 11:19:01 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 11:19:01 GMT
USER user
# Tue, 05 Apr 2022 11:19:01 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa1dbdb27d63340f8b8fa494a282aeded5f878185e2847d6dfb481b353b8c11`  
		Last Modified: Tue, 05 Apr 2022 11:19:27 GMT  
		Size: 9.5 MB (9540662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd245485e0307925fa298d8f511fe481b6600ce336c8ff0a0b5c13ce1435d9`  
		Last Modified: Tue, 05 Apr 2022 11:19:24 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4513426f1a6993290c7fa1e95a9f0bd0309456d69e3c04c0a7e8b17b66c9a079`  
		Last Modified: Tue, 05 Apr 2022 11:19:25 GMT  
		Size: 6.3 MB (6287259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v6

```console
$ docker pull irssi@sha256:5262462a3f32457835863ac8b11823de2d926d672219bdff8c5c67bc5e116e2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17385410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab49acd659041f4c479472bb7ed35e0fc93656b968625544d96599e44c57c01`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:01:19 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:01:20 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:01:21 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:01:22 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:01:22 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:02:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:02:32 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:02:32 GMT
USER user
# Tue, 05 Apr 2022 04:02:33 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b589ee3c7baf4a3043d5c498c04269109c4a45e58c44ab98b5a969b7ba2f8a`  
		Last Modified: Tue, 05 Apr 2022 04:03:13 GMT  
		Size: 8.8 MB (8771955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82acf7c178275d848adf6769cd6193b1f701750ef2bf058c507c10c4af90080d`  
		Last Modified: Tue, 05 Apr 2022 04:03:05 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391da21a1ce4611cc08325dc363346ea9ae04e1724386ad9b1a8801e1843e835`  
		Last Modified: Tue, 05 Apr 2022 04:03:09 GMT  
		Size: 6.0 MB (5987042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm variant v7

```console
$ docker pull irssi@sha256:85b6871234efe5afa8aee356cecfc27abb04e6a99f43a969eedce41a3230299b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16839452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f387771b9c45b2879b4d36faf8f6326c4b27afacac146e4d774c52b2d0f103cb`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:58:06 GMT
ADD file:0834e20e80add8b1c6bd545ebe0729239e00a4dff08b025cb5555cd3ce58e4c6 in / 
# Mon, 04 Apr 2022 23:58:07 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:02:01 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 16:02:01 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 16:02:03 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 16:02:03 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 16:02:04 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 16:03:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 16:03:10 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 16:03:10 GMT
USER user
# Tue, 05 Apr 2022 16:03:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:a8b8a1c7a552f6893757dd6327a5a430981d78aa06a59298076603526186829e`  
		Last Modified: Mon, 04 Apr 2022 23:59:56 GMT  
		Size: 2.4 MB (2427836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0c71a12aa1dc1147bd41cf6458906772bf77be69de2e8fc3d9242f641fc445`  
		Last Modified: Tue, 05 Apr 2022 16:04:19 GMT  
		Size: 8.6 MB (8626381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf67fa3e83093b4230c7f24388cfb9f6f9aa8bd3c5d76434f7b058a66d7ab80`  
		Last Modified: Tue, 05 Apr 2022 16:04:11 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95a6a97274960e7695eb8d37b680b0fe6bc45a12b2b550e310504260e923285`  
		Last Modified: Tue, 05 Apr 2022 16:04:15 GMT  
		Size: 5.8 MB (5783964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:d49fa5e7d3a8cd10c7bfad3e9bec2fa37e6a44c2911c1958c7014a121f4eef59
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.5 MB (18505792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98cf9f811eb592e3b8c251eb41f7f7dfdadc8c7b6dc2e9fae2c2d835173d8ac`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:14:15 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 04:14:16 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 04:14:17 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 04:14:18 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 04:14:19 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 04:14:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 04:14:54 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 04:14:55 GMT
USER user
# Tue, 05 Apr 2022 04:14:56 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f125d0f2f3de8f4307e1218e71620016554b5120c8ce30e8786904dc74366d0b`  
		Last Modified: Tue, 05 Apr 2022 04:15:25 GMT  
		Size: 9.5 MB (9536419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c48a8193426a12a478ffa39f46aa61977b41d48a60d252930c3c2a4708fd0b7`  
		Last Modified: Tue, 05 Apr 2022 04:15:23 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7a5707b30c726d92bca84220a2cb23b4ff000e7119f0a696975a866269d135`  
		Last Modified: Tue, 05 Apr 2022 04:15:24 GMT  
		Size: 6.2 MB (6247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; 386

```console
$ docker pull irssi@sha256:f4044a89fe2a5119671314da6e8cbfed9929c215d20d677e6b84a7e5b713611f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17704054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aea095e2938971334ab2464fcf39c254bd75a69e3b56999f7fab374fb813c92`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:47:49 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 06:47:49 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 06:47:50 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 06:47:51 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 06:47:52 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 06:48:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 06:48:28 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 06:48:29 GMT
USER user
# Tue, 05 Apr 2022 06:48:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d17b6eaf713c06aeabfe2feac029d7c880865cf49ab0c148c784791c31779`  
		Last Modified: Tue, 05 Apr 2022 06:49:01 GMT  
		Size: 8.9 MB (8904271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831ba5a4f1fc534f7dec6b2cf96d9935df1d6b00524538974d10799fd6f4c53`  
		Last Modified: Tue, 05 Apr 2022 06:48:59 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3dd29c50ebba7606220a2a714a5fdb3059694e3f39c9b707f4c43086cf958`  
		Last Modified: Tue, 05 Apr 2022 06:49:00 GMT  
		Size: 6.0 MB (5978011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; ppc64le

```console
$ docker pull irssi@sha256:beba11d08d6df10a4fe4518b49c2e3d8b54f2cb9f15feb8bce4bfba5d97c6674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18941010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37da7ed44ea84c9ebfb079e981447b44fccab806fd3be499c492a079908bf21d`
-	Default Command: `["irssi"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:56 GMT
ADD file:a9d5347a58c095f620406d9afc12b5ae4fd6c3994ea7e88e6415db7b09725289 in / 
# Tue, 05 Apr 2022 00:24:00 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:10:05 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 19:10:11 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 19:10:20 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 19:10:25 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 19:10:29 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 19:11:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 19:11:33 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 19:11:36 GMT
USER user
# Tue, 05 Apr 2022 19:11:39 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:afbded953e7f469508815262f0ff60fc06823cc1701e4b7aa211eb10bca545bd`  
		Last Modified: Tue, 05 Apr 2022 00:25:18 GMT  
		Size: 2.8 MB (2814791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73fa56481e3f5fd84b721b288e4628ef18d832025ab22c2cb0601f85d9025b`  
		Last Modified: Tue, 05 Apr 2022 19:12:17 GMT  
		Size: 9.6 MB (9632765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2998f1c0df5727d61352cf5bbb86f17a2b07e8d0feef2892ad0c1a13693ed8`  
		Last Modified: Tue, 05 Apr 2022 19:12:15 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0ce73fb7b2975452460737c989e296843d87ad3f26c26f5c7df696df51a1ea`  
		Last Modified: Tue, 05 Apr 2022 19:12:16 GMT  
		Size: 6.5 MB (6492183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:alpine` - linux; s390x

```console
$ docker pull irssi@sha256:07e9626c05472af1fce5448f4310a04d7bc5e3a7e6a4384227d5aaec02d65705
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.9 MB (18855197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5ea35b9201821c8168c1b19f5a926438127784e392a0465b5a49bc2b7f98e1`
-	Default Command: `["irssi"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:55 GMT
ADD file:0f7653032bb9c65a5643cc31ad93fca7bd018ca0466a2d1c4ccadc5db00ad0f0 in / 
# Mon, 04 Apr 2022 23:41:55 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:58:34 GMT
RUN apk add --no-cache 		ca-certificates 		perl-libwww
# Tue, 05 Apr 2022 03:58:35 GMT
ENV HOME=/home/user
# Tue, 05 Apr 2022 03:58:36 GMT
RUN set -eux; 	adduser -u 1001 -D -h "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Tue, 05 Apr 2022 03:58:36 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:58:36 GMT
ENV IRSSI_VERSION=1.2.3
# Tue, 05 Apr 2022 03:59:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		autoconf 		automake 		coreutils 		dpkg-dev dpkg 		gcc 		glib-dev 		gnupg 		libc-dev 		libtool 		lynx 		make 		ncurses-dev 		openssl 		openssl-dev 		perl-dev 		pkgconf 		tar 	; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .irssi-rundeps $runDeps; 	apk del --no-network .build-deps; 		irssi --version
# Tue, 05 Apr 2022 03:59:07 GMT
WORKDIR /home/user
# Tue, 05 Apr 2022 03:59:07 GMT
USER user
# Tue, 05 Apr 2022 03:59:07 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:22b3eb8fdd3cabd13718400a1a4d1e75330e6e512d556cdd902359adeb0b014a`  
		Last Modified: Mon, 04 Apr 2022 23:42:54 GMT  
		Size: 2.6 MB (2605058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2a655edb7398e76b909cbb12baf208d875c598793a42546c8f2b906ab8e2c7`  
		Last Modified: Tue, 05 Apr 2022 03:59:36 GMT  
		Size: 10.0 MB (9972200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16218c4743041a59790e9a6b9388344940cd9dbf0e8c3cff8ea17486b32b553`  
		Last Modified: Tue, 05 Apr 2022 03:59:34 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92e5f35e6bfccd90acff05f4db673effe1dce4f736f0d128d6e878f5524767`  
		Last Modified: Tue, 05 Apr 2022 03:59:35 GMT  
		Size: 6.3 MB (6276668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `irssi:latest`

```console
$ docker pull irssi@sha256:9e19096cc30c331015cc1e4ebb3a4f11967adb7c2ae52aa11dc775f90441605f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `irssi:latest` - linux; amd64

```console
$ docker pull irssi@sha256:9b8e794c52606ddb03386ca63e00b8822bb0422ba8d1bbc1f6a91b1169badcf6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50616256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d9bf5187a352d791a3be64008fab00c63e5153e65db45b19b848fafffa65e7`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 05:20:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 05:20:24 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 05:20:25 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 05:20:25 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 05:20:25 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 05:21:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 05:21:09 GMT
WORKDIR /home/user
# Sat, 28 May 2022 05:21:09 GMT
USER user
# Sat, 28 May 2022 05:21:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1afda879f82264f53bd7206d0529f22e6289f5c266669663f9a1dbcb2377086`  
		Last Modified: Sat, 28 May 2022 05:21:37 GMT  
		Size: 17.0 MB (17038480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b893d548ee02faada4ffcfce881ee9a9d8e144b1d052d85e14338a10a584f73f`  
		Last Modified: Sat, 28 May 2022 05:21:33 GMT  
		Size: 4.2 KB (4213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78daf0e1ebbead3bdba065457c48d6a82da6191e098a16e5b228c56e2079d10`  
		Last Modified: Sat, 28 May 2022 05:21:35 GMT  
		Size: 6.4 MB (6433419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v5

```console
$ docker pull irssi@sha256:319e7359b22812fedb09a44d23cd11e0da8e2764a1f58117d086cb28b1efbfae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46896517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece64e4b9eb38841094e52414e2eb69af1f67124e41ae31ab7f4eb05e168e822`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 02:04:06 GMT
ADD file:26e9ed6c41ec12bf5fd602b7f86b924d34537bbc82442f630763f9f6c48bf3b3 in / 
# Sat, 28 May 2022 02:04:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:51:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:51:33 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 03:51:34 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 03:51:35 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 03:51:35 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 03:53:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 03:53:30 GMT
WORKDIR /home/user
# Sat, 28 May 2022 03:53:30 GMT
USER user
# Sat, 28 May 2022 03:53:31 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:19389fd1100abdedaa775b43242838cdd2d5c8c3388643a7e52da2b7b4399c15`  
		Last Modified: Sat, 28 May 2022 02:20:06 GMT  
		Size: 24.9 MB (24890069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc97e5088dad5dd24e65c10e4ea9e411d109a92d2e5ea0ea963e08e311ad796`  
		Last Modified: Sat, 28 May 2022 03:54:27 GMT  
		Size: 15.9 MB (15937730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4a37ba27a89a967fe9c2d2f15f8e694a897f7ce14473c47467a7d1fee1f5eb`  
		Last Modified: Sat, 28 May 2022 03:54:12 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a75a4f2bb09f772d8125095f28993565ba0cedf1ea7e623d06819383b74dd`  
		Last Modified: Sat, 28 May 2022 03:54:16 GMT  
		Size: 6.1 MB (6064521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm variant v7

```console
$ docker pull irssi@sha256:4cf05cf78af130b124c2677cfc8a08fb5b49ee61ef19ee43cf5aa7d668ea8609
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44283091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9bde88159cecf11997b4d861c8ce640cc9e4dc449048d1436268d80152d736f`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:00:54 GMT
ADD file:c89d47099a38749a424760d9c7d3a6e982089455ba9d04140db15ba9eb4cdda1 in / 
# Sat, 28 May 2022 01:00:55 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:32:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:33:00 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 07:33:02 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 07:33:02 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 07:33:02 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 07:34:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 07:34:50 GMT
WORKDIR /home/user
# Sat, 28 May 2022 07:34:50 GMT
USER user
# Sat, 28 May 2022 07:34:51 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:e41117292dc8c199b63ae1ec4485358841dbcba68dcbd13f379b66182efe832e`  
		Last Modified: Sat, 28 May 2022 01:16:58 GMT  
		Size: 22.7 MB (22748097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3818c0c31072687a62a285a3582a6ac59a7e9c1c0d84423739dafb09cd2f397`  
		Last Modified: Sat, 28 May 2022 07:36:12 GMT  
		Size: 15.6 MB (15598239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c30d93b9a282c1f30a84b17541b5cb2b05cdbced870f4f1f7097d1c79985ee`  
		Last Modified: Sat, 28 May 2022 07:35:57 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22736721f72dfd763c95b664b3afb4327c73190f4bf5230c40283d02328701eb`  
		Last Modified: Sat, 28 May 2022 07:36:00 GMT  
		Size: 5.9 MB (5932564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; arm64 variant v8

```console
$ docker pull irssi@sha256:93331fad416045665e2b6bfb19606ccc3e2da9ab35ac8e4f3e359d9d8564efa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48908753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d67ac80f549afca6223607f6df4382b1f3caefa46171f8129e47175a13833c`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 00:41:05 GMT
ADD file:d0e42d603f275c040783ec7b6c051200815492fc35b73110234dfcd584e6cdec in / 
# Sat, 28 May 2022 00:41:05 GMT
CMD ["bash"]
# Sat, 28 May 2022 13:07:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 13:07:23 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 13:07:24 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 13:07:25 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 13:07:26 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 13:08:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 13:08:08 GMT
WORKDIR /home/user
# Sat, 28 May 2022 13:08:09 GMT
USER user
# Sat, 28 May 2022 13:08:10 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:4931fb8ba4223cb35034141162105ee5482122692b2931eb69eec912ce64606d`  
		Last Modified: Sat, 28 May 2022 00:48:26 GMT  
		Size: 25.9 MB (25914033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578f8e8c703cdf2c34f2aacd16e83af9040d1c923427dc5fe10fff3969b17983`  
		Last Modified: Sat, 28 May 2022 13:08:49 GMT  
		Size: 16.8 MB (16814580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dba055597f3b5e93280156ec02d53a40d9604ae8e34f7b120795b251f0adab`  
		Last Modified: Sat, 28 May 2022 13:08:46 GMT  
		Size: 4.1 KB (4072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1655e15c8cad9556df1295427409be5707ebc949b480830c26e363b0b146534c`  
		Last Modified: Sat, 28 May 2022 13:08:47 GMT  
		Size: 6.2 MB (6176068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; 386

```console
$ docker pull irssi@sha256:f87197bcb070dc6091ab19977c431f3e95e762098396a327d292f019ddb5dc0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50263361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c22d8c0a1d40fa9e5af5c700fc4e768e9277eb28e82bad9f5bbafd0fb48def2e`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 00:40:01 GMT
ADD file:9aea7a35c215cdd778adec1dd5213973ef9b4830110e4550f2ead85679551ee5 in / 
# Sat, 28 May 2022 00:40:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 12:36:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 12:36:40 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 12:36:41 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 12:36:42 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 12:36:43 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 12:37:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 12:37:28 GMT
WORKDIR /home/user
# Sat, 28 May 2022 12:37:29 GMT
USER user
# Sat, 28 May 2022 12:37:30 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:40837b3d848885c0b0c031d6d950b38e6a26962a5ee49704cb3ca2d2db535617`  
		Last Modified: Sat, 28 May 2022 00:47:36 GMT  
		Size: 27.8 MB (27799572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bd85652cb7aee11a1ee235bfe214f30f2eed4280ecc94c7721326d13bbaeaf`  
		Last Modified: Sat, 28 May 2022 12:38:05 GMT  
		Size: 16.6 MB (16566304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c056bbb0e1c559600ab3a62c0b4cb4e41e2277f340915f3e120c990c97bafa84`  
		Last Modified: Sat, 28 May 2022 12:38:02 GMT  
		Size: 4.1 KB (4058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c9f8088df3ca5683e0a6dfe2a6aaf868428ecfcbef01b067549522f8b11e93`  
		Last Modified: Sat, 28 May 2022 12:38:03 GMT  
		Size: 5.9 MB (5893427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; mips64le

```console
$ docker pull irssi@sha256:4bf810ff969b5912a5e687a4c44aa741870b792ff2ec4a48afa82cf959023d49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47631105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b4d731d65f3d51d2dfe09f12efe86b3963cdc36b44461ec2373fa54942db31`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:12:21 GMT
ADD file:12eb3f58e1c47ef1af98f481c1f5f33832f45144bf66f3a01065f8c939f1eaa9 in / 
# Sat, 28 May 2022 01:12:25 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:15:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:15:46 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 03:15:54 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 03:15:57 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 03:16:00 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 03:20:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 03:20:30 GMT
WORKDIR /home/user
# Sat, 28 May 2022 03:20:33 GMT
USER user
# Sat, 28 May 2022 03:20:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:79a954ba282b6c17b5d2fdc4563e0fbc4bf4e3c673bada0b2f656937656557eb`  
		Last Modified: Sat, 28 May 2022 01:22:56 GMT  
		Size: 25.8 MB (25814580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad211fee54c5f12de817e949479da0f9fa7e5923811567b7286c6050032245fc`  
		Last Modified: Sat, 28 May 2022 03:21:16 GMT  
		Size: 15.7 MB (15732112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805cb834a6e653d97de303cfc43b9da9082614eb08397f22b596a004b9532474`  
		Last Modified: Sat, 28 May 2022 03:21:02 GMT  
		Size: 4.1 KB (4074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edb471e3b1d4a83905a6a5c109848bbdf1f68055b04cc7a6763006a14dfc474`  
		Last Modified: Sat, 28 May 2022 03:21:06 GMT  
		Size: 6.1 MB (6080339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; ppc64le

```console
$ docker pull irssi@sha256:e39d45ef70272a2e6cf18c9dd66d12ee70a3645f2046b11496743d0cd865deca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54787987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baff97fede43b1fb6e3ca8de715b96fc263414eedea56bd2b0051990c5ed73d9`
-	Default Command: `["irssi"]`

```dockerfile
# Sat, 28 May 2022 01:23:57 GMT
ADD file:a8c6c897bc64da424049ad04a354d123b0622abda1a56b2725f72de5e4569df8 in / 
# Sat, 28 May 2022 01:24:04 GMT
CMD ["bash"]
# Sat, 28 May 2022 06:52:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 06:52:32 GMT
ENV HOME=/home/user
# Sat, 28 May 2022 06:52:36 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Sat, 28 May 2022 06:52:38 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 06:52:41 GMT
ENV IRSSI_VERSION=1.2.3
# Sat, 28 May 2022 06:57:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Sat, 28 May 2022 06:57:14 GMT
WORKDIR /home/user
# Sat, 28 May 2022 06:57:16 GMT
USER user
# Sat, 28 May 2022 06:57:21 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:087d40850259bdcd3bee3d5d30d5a2070216727f72c1c9731b514ac3dbf7573e`  
		Last Modified: Sat, 28 May 2022 01:33:30 GMT  
		Size: 30.6 MB (30560238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e180ca0caaecd96894d59df3140df02564c778c40d46b6d03f0fda10eefa6d35`  
		Last Modified: Sat, 28 May 2022 06:58:03 GMT  
		Size: 17.4 MB (17440702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932bc69b6c04fbdc83f98628214743c0e6645a14a5adb34acc1d5590c38d360`  
		Last Modified: Sat, 28 May 2022 06:57:58 GMT  
		Size: 4.2 KB (4209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf716870602840820cee5bb11e395b8197b4435e92d9213dba7ad4456818e16`  
		Last Modified: Sat, 28 May 2022 06:58:00 GMT  
		Size: 6.8 MB (6782838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `irssi:latest` - linux; s390x

```console
$ docker pull irssi@sha256:6babbc57189870e9c78763f97de83c067a89b24ddac49f302b21504254e0da1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49061887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b289242502c712e59b5bc78e77d30bad09363d5bdbf1da235ab944c5f4a4393`
-	Default Command: `["irssi"]`

```dockerfile
# Wed, 11 May 2022 00:44:47 GMT
ADD file:28b1e60f65391906bebd81248a4da766172138fab99b8b9e6b18bce76afea02d in / 
# Wed, 11 May 2022 00:44:49 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:29:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		libdatetime-perl 		libwww-perl 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:29:57 GMT
ENV HOME=/home/user
# Wed, 11 May 2022 02:29:58 GMT
RUN set -eux; 	useradd --create-home --home-dir "$HOME" user; 	mkdir "$HOME/.irssi"; 	chown -R user:user "$HOME"
# Wed, 11 May 2022 02:29:58 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 02:29:58 GMT
ENV IRSSI_VERSION=1.2.3
# Wed, 11 May 2022 02:30:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dirmngr 		dpkg-dev 		gnupg 		libglib2.0-dev 		libncurses-dev 		libperl-dev 		libssl-dev 		libtool 		lynx 		make 		pkg-config 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz" -O /tmp/irssi.tar.xz; 	wget "https://github.com/irssi/irssi/releases/download/${IRSSI_VERSION}/irssi-${IRSSI_VERSION}.tar.xz.asc" -O /tmp/irssi.tar.xz.asc; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 7EE65E3082A5FB06AC7C368D00CCB587DDBEF0E1; 	gpg --batch --verify /tmp/irssi.tar.xz.asc /tmp/irssi.tar.xz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /tmp/irssi.tar.xz.asc; 		mkdir -p /usr/src/irssi; 	tar -xf /tmp/irssi.tar.xz -C /usr/src/irssi --strip-components 1; 	rm /tmp/irssi.tar.xz; 		cd /usr/src/irssi; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-true-color 		--with-bot 		--with-proxy 		--with-socks 	; 	make -j "$(nproc)"; 	make install; 		cd /; 	rm -rf /usr/src/irssi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		irssi --version
# Wed, 11 May 2022 02:30:37 GMT
WORKDIR /home/user
# Wed, 11 May 2022 02:30:37 GMT
USER user
# Wed, 11 May 2022 02:30:37 GMT
CMD ["irssi"]
```

-	Layers:
	-	`sha256:bf64474a39a67000556a4502abd4584010a062b942cf8e2545d0502d38ffa150`  
		Last Modified: Wed, 11 May 2022 00:50:43 GMT  
		Size: 25.8 MB (25758738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bab2a510dcd371ba308d88b7a421f4392242a1145a5e2032557bff64f1f3096`  
		Last Modified: Wed, 11 May 2022 02:31:19 GMT  
		Size: 16.9 MB (16914219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114f12ef452583e1b53623df64e6ed1ef5fe101a2bd32bcb5670547708d201b1`  
		Last Modified: Wed, 11 May 2022 02:31:16 GMT  
		Size: 4.2 KB (4212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3872a1d35d40ae59cc2e54813e37c9cd0c725b5df75a8e79c674d79cfed86c`  
		Last Modified: Wed, 11 May 2022 02:31:17 GMT  
		Size: 6.4 MB (6384718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
