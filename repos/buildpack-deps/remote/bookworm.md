## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:914dabfd8e27e0ff0d78ed451513d8529f0239ab92be537bf8b368c0b312c75e
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

### `buildpack-deps:bookworm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e3ceaa559f55d3ef7143e6f5e2c7deb45373a14f66d78337c98275cf7e3dd43e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.0 MB (338982342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f655195eb67b40fd8f6edcdb2ef14478a4b6045bcb64aa54c10803217e372c0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:19:54 GMT
ADD file:7e968e6ae38ede120a52f1d2e734b4fee4fd4ffd6e5f747edc8190d2a8bc6a52 in / 
# Thu, 23 Jun 2022 00:19:56 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:48:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 00:49:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:49:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8849e73adf621df4a443e9ac4eec9b698476e4f14f8ed894806f302d5b33156b`  
		Last Modified: Thu, 23 Jun 2022 00:24:12 GMT  
		Size: 53.0 MB (52993983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a3004561e732519f3aa704178d4bc2d97eae3c1cc556af0ea0d3e66e28ba24`  
		Last Modified: Thu, 23 Jun 2022 00:57:33 GMT  
		Size: 9.3 MB (9291497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0f93f12fe636ab6b9beed73979390ba6a1aa6fdcf7bbc5cb403f683142a0e3`  
		Last Modified: Thu, 23 Jun 2022 00:57:33 GMT  
		Size: 11.3 MB (11264030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c85c343cd3e553d90219aa415a28525986ebdcf4ed151ad763eea350150fd70`  
		Last Modified: Thu, 23 Jun 2022 00:57:52 GMT  
		Size: 57.7 MB (57719551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d4709f8d9bb7ab97a241ea8a07159919e2c1d3dfab03b8cb8f554c6c1e690e`  
		Last Modified: Thu, 23 Jun 2022 00:58:26 GMT  
		Size: 207.7 MB (207713281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a11d1efb1f84172d9c04b0ee4c0ac1bc9105aec26b2fcbb0268f9bbcf1998f08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.5 MB (309542429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f16b434cdd0de5160a0c8cfa396a33ad959bc9f9619b3aef0e69678232434c0e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:49:07 GMT
ADD file:d8a58d5f4d1c34aefbf2ca6b2eeab0bbf20b8cb6400548926c6a16cce570dc9d in / 
# Thu, 23 Jun 2022 00:49:08 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:32:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:32:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:34:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:36:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5248fb4f18035bd1257a3136675241430095c1cdf250910c001999b7f421381c`  
		Last Modified: Thu, 23 Jun 2022 01:03:30 GMT  
		Size: 50.8 MB (50767843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b7a64f309184d3ebc17e9dbe6bed869037215ff9f9748c7dffa9ffd3e631ee`  
		Last Modified: Thu, 23 Jun 2022 01:58:12 GMT  
		Size: 8.7 MB (8726860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a0203b6e2645c48e6d7e1a1ec99807f7da08cea315ce1d19d9ca8ae62d6246`  
		Last Modified: Thu, 23 Jun 2022 01:58:12 GMT  
		Size: 10.9 MB (10927730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f066702837fa4198900a9738fb6fce0276868d06d1e1cd19d0dda62c8bc1161`  
		Last Modified: Thu, 23 Jun 2022 01:59:03 GMT  
		Size: 55.4 MB (55387224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b3c207706998bc07b60b9b927e1f93c5b5e53b7508f83b82bb40c3d50e879`  
		Last Modified: Thu, 23 Jun 2022 02:01:07 GMT  
		Size: 183.7 MB (183732772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7d657db2082a4bfda8d9131f08ec63c45f1d0e541e885d41b5124e4fdf6eb11b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.4 MB (296444733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5acebd892f2b8f818fb9534daf32472b1345b8b2a6ed3848ffe6899ee35cc71`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:58:08 GMT
ADD file:485670bbc3d21c74d06e079229d1c74d05970c4bdf8c5d25692ab1464f0acfce in / 
# Thu, 23 Jun 2022 00:58:09 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:42:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:42:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:43:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:45:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:da5c76d2fa54760a1e859c83968ea6d7dfee1c43064fb6f34c27f8d639859b07`  
		Last Modified: Thu, 23 Jun 2022 01:13:19 GMT  
		Size: 48.5 MB (48506514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231adce49f6a983a4cfa3f3683a6c276af5ef432ea37e705272135b3a56084b1`  
		Last Modified: Thu, 23 Jun 2022 02:10:23 GMT  
		Size: 8.4 MB (8397133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8487327d153dbcbea96feb013bca9efcd1fa6319396003a967515da5f4ab1d6a`  
		Last Modified: Thu, 23 Jun 2022 02:10:23 GMT  
		Size: 10.6 MB (10572720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2c56a82b9fbf3bde9d03894c5080a67cf22d4eb43fb32978cc465e44267d81`  
		Last Modified: Thu, 23 Jun 2022 02:11:11 GMT  
		Size: 53.3 MB (53313376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb9aafaf1a57b0edb3b93746d80ff4e9c59e726137f63775d11785fe99aa297`  
		Last Modified: Thu, 23 Jun 2022 02:13:00 GMT  
		Size: 175.7 MB (175654990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:39537ff6fa2874d82dd2303e1bb631bde9ac3f92d705b1b72ac90ed6953dcb5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331545818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0653b279d5c793b8369b188bf37d263d691e39e0ab86fa035d3cc78f9d8a30d6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:05 GMT
ADD file:149d923f098f33a347aa57ca673aae5cc103628b202337e4ff2ea5ac278e5c18 in / 
# Thu, 23 Jun 2022 00:40:05 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:09:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:09:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:09:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:11:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e34000263ac838bb9254930c5e34d9fa4b486f544707ae0aa508bb7ded624d59`  
		Last Modified: Thu, 23 Jun 2022 00:46:09 GMT  
		Size: 52.1 MB (52074605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d844fe46570aeb3a40b42c67a4714c432ac2d6ccc31125f7eeb076c05e919ff`  
		Last Modified: Thu, 23 Jun 2022 01:20:40 GMT  
		Size: 9.1 MB (9126954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f39d92840e0fe1b4aa70af7e37d1e6c48b3c61da85b2b3d9e13efb83c990d2d`  
		Last Modified: Thu, 23 Jun 2022 01:20:40 GMT  
		Size: 11.0 MB (11041433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbe8b6171db521e3284e73fee8669036467cffe10b2030372d262cb498caaf1`  
		Last Modified: Thu, 23 Jun 2022 01:21:01 GMT  
		Size: 57.7 MB (57713059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304a54a06ddf5360088c970ab81c345cb257f2c4fb82f6e9c48f7e7671864610`  
		Last Modified: Thu, 23 Jun 2022 01:21:38 GMT  
		Size: 201.6 MB (201589767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:24ce11a00391b071a67ed11662e55dc14db3fb6473b4729d64e34ed282a3173c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.1 MB (342084069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54baeb2366e78baa032405ff8dbb9557cfff15249944d2ba36e2a88af853468a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:38:52 GMT
ADD file:d8108af9af2f3fb7f3dd905a9b4dd8391d568ba8dd590a9ca2bbeecd44354e03 in / 
# Thu, 23 Jun 2022 00:38:54 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:08:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:08:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:09:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:11:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0120d80f9ec3d96114e34087bd467cf9989c9c723cf7622bb16fb3675443565c`  
		Last Modified: Thu, 23 Jun 2022 00:45:18 GMT  
		Size: 54.0 MB (53963635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a0c1f242a443b42292f09b23bf00a038a40230b125f2d832ff706e0b0fd009`  
		Last Modified: Thu, 23 Jun 2022 01:21:05 GMT  
		Size: 9.5 MB (9464738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2c7e9a858ffdd4f52faf3fc1e4e080485c9024f299858237d4b3961f4e27d`  
		Last Modified: Thu, 23 Jun 2022 01:21:05 GMT  
		Size: 11.5 MB (11464163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000d7279af4a42e39fe0892505db82f28dc4127c5b4ff59701217c5f3921c339`  
		Last Modified: Thu, 23 Jun 2022 01:21:26 GMT  
		Size: 59.2 MB (59192570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e247eb958bba36f25d3fbec4ead564df58e2dc5cc7e06e7b32f7e73f839a3d`  
		Last Modified: Thu, 23 Jun 2022 01:22:02 GMT  
		Size: 208.0 MB (207998963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2c556d878f8bba91c100c075b10c01bbccf928d8d74bc064b64de3e3379a6c1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.2 MB (319218709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b303a555dec9e7582838a9009ea93f853041d8a0f5590b190534633eb1a22e30`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:08:42 GMT
ADD file:8bc6b496d7debb22306bce782f6b34ee75efae7151dc19314b45a9751b8fbdb4 in / 
# Thu, 23 Jun 2022 01:08:47 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:44:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:44:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:51:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25ef8061366d5e6abd7ca324b8c1f08ba96be6bd0e55fd310e046a1e4becfdb6`  
		Last Modified: Thu, 23 Jun 2022 01:18:17 GMT  
		Size: 52.1 MB (52089294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8d0efe31fb7f6ccd1d5334126a57a6651ed1009e9a6eb93f4fb51019078cf1`  
		Last Modified: Thu, 23 Jun 2022 02:16:45 GMT  
		Size: 8.7 MB (8657797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d342e8e78e8778dab632125fd70a05b026d9c29cfed07832f8527747409a8a67`  
		Last Modified: Thu, 23 Jun 2022 02:16:45 GMT  
		Size: 11.0 MB (11019371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93153ce1ff5d2f9dd76da70875ccf9835543f0261f518018d8d826434056dd06`  
		Last Modified: Thu, 23 Jun 2022 02:17:34 GMT  
		Size: 56.4 MB (56361059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ef1942cd54d67bac3636a1272b66f84ecddbffab074cb4a4a948efd0abc30f`  
		Last Modified: Thu, 23 Jun 2022 02:19:45 GMT  
		Size: 191.1 MB (191091188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:89a3c27b023746b78465e06a5259ad98842a1bc0f28e7790637b6ce4388ee967
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.5 MB (349538058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e0fadfc9f932a7b23e286aad9006320195f0d70b1ae1fcae3307ab46b5af0a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 02:00:58 GMT
ADD file:d857864fffea40faaeec8c9492ef1805e6c891ebf06f1427f02398a3824debce in / 
# Thu, 23 Jun 2022 02:01:01 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 03:43:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:43:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 03:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 03:52:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8afb6214160c68cb540431e94c7bfe898f1a094dc45a834aa07634d34b1505a3`  
		Last Modified: Thu, 23 Jun 2022 02:12:13 GMT  
		Size: 57.2 MB (57198049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a70dd21016ae34b7615f4f27bc039c2c609a2ac123e43b625424da683ee24b3`  
		Last Modified: Thu, 23 Jun 2022 04:54:13 GMT  
		Size: 9.9 MB (9883483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb14a4d02ea4ebe3ab1ddfc7a7bfdc8945f0478c8c9592495931e4a0a21b69d`  
		Last Modified: Thu, 23 Jun 2022 04:54:12 GMT  
		Size: 12.1 MB (12065040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1582dcac09eb1694cd819ab79fa690166d66caa532597c54cb2899dc67c2f55`  
		Last Modified: Thu, 23 Jun 2022 04:55:06 GMT  
		Size: 62.4 MB (62429235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5355ca87e53f29fa6918c79d3833d8a62dfdb18807fa0cfca5cf81431fdd226d`  
		Last Modified: Thu, 23 Jun 2022 04:55:53 GMT  
		Size: 208.0 MB (207962251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:16ec60917538e8e2b1debdbdc160dfcf2a8648bc05b2dd1230618707c929b552
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.5 MB (310505144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b0ef30301ba4c9f2e2593fcaa132249c8a37e6b350cfe7c13c629c0384010f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:41:51 GMT
ADD file:b7c920f3965a4e47e7a0f42e020e195f493babee2f175c563676dd0d45c0b27b in / 
# Thu, 23 Jun 2022 00:41:58 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:11:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:11:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:12:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:15:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bb926b744d748e9437f2a0a451eea25192350981dae9cf0d8effd239dd22e761`  
		Last Modified: Thu, 23 Jun 2022 00:51:01 GMT  
		Size: 51.5 MB (51530571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7ecccdf5c546fed3b800725dd538dd6145ccb9ae337d876c51b657ce9b04f1`  
		Last Modified: Thu, 23 Jun 2022 01:34:04 GMT  
		Size: 8.9 MB (8938768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98bfe7c167f54ada5e3d22060e56ad9ef2d8269fb0c0bbd4e5683afaf21b548`  
		Last Modified: Thu, 23 Jun 2022 01:34:03 GMT  
		Size: 11.2 MB (11157453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2649e5b4208cd3e4644788449131d6ce6bcdfd648d98111724b67c0429e1f0bc`  
		Last Modified: Thu, 23 Jun 2022 01:34:20 GMT  
		Size: 57.0 MB (57028211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c287c55c8d127a3c227a19bff4089f9753edd211b5312b78428fcb703bdaf0fe`  
		Last Modified: Thu, 23 Jun 2022 01:34:48 GMT  
		Size: 181.9 MB (181850141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
