## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:ec54c90000724dd20416132f1562d4b0df1435552c2d78459a8be15a5e78cff3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bullseye` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:18ffeadb213e77ecc83d883b471b385a8e08be64d5fecfa5028872d6a70bc00c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.3 MB (329274045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06d716de316b00290d127c19c465ea87f6534f82a6a09864fd7474007a5c7b6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:09 GMT
ADD file:730ef8e3327df644cd47994a561a489bfcce5da8103cc8eb34e67321a36df2ba in / 
# Tue, 12 Jan 2021 00:32:09 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:55:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:56:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b802c2c29a7757c7475a0b343a18a46b6b27dde9e3fb6b4db61c68ea197b51d2`  
		Last Modified: Tue, 12 Jan 2021 00:38:04 GMT  
		Size: 53.6 MB (53566443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd06bfac0a19b28c6511794acccc260657d53a299701a82ec9fcafe465089350`  
		Last Modified: Tue, 12 Jan 2021 04:04:36 GMT  
		Size: 8.0 MB (7974792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d97704dcad5e05944cbac93df8fdf452cb71e698fd44004184391a44e8787c`  
		Last Modified: Tue, 12 Jan 2021 04:04:36 GMT  
		Size: 10.6 MB (10649126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782396cc8dbffc61d005f86b48ba6f88b4dbeb6e71f98f909b15d1e290bc9273`  
		Last Modified: Tue, 12 Jan 2021 04:04:59 GMT  
		Size: 53.9 MB (53853868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6675c99b996119a82a24c8129eb1800246924afe764c3b117cbcb338810f70`  
		Last Modified: Tue, 12 Jan 2021 04:05:47 GMT  
		Size: 203.2 MB (203229816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7c1b4f5adcc0a6a06b80c182cb1098f6f8198d3a762d7d9bc96ca71a699bb540
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302384589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfcc33cc62602e4c18e75fa0f531ebffb3ced2ab94410974540d2c95e3f63f9c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:50:29 GMT
ADD file:d4da31b3c934d9b6c8328e7951f06cec1babe1f9674a7a3ee2e87670575ff01c in / 
# Tue, 12 Jan 2021 00:50:30 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:24:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:27:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f9810833d48e3d19cbfbfb8871ba282d104d5bcfae1b19c0c003f9811dbe7c4c`  
		Last Modified: Tue, 12 Jan 2021 00:58:53 GMT  
		Size: 51.5 MB (51487444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257fe5697f52f59aa0dbdede36db8adf4c0796905b3388832de43ac1e4ab97d`  
		Last Modified: Tue, 12 Jan 2021 01:41:45 GMT  
		Size: 7.5 MB (7527914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c59bb7c72bcd7ff3df84ab37209a928574816146c37f0808619c4b5a6dde4a1`  
		Last Modified: Tue, 12 Jan 2021 01:41:45 GMT  
		Size: 10.3 MB (10335674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2064b7463d16bbcc2e8bc6d085c083e4e8d5bf88ac7a254843dc12449eaec623`  
		Last Modified: Tue, 12 Jan 2021 01:42:15 GMT  
		Size: 51.5 MB (51549893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b96292ec002aa2f69335d7a934c50886b11e8eb437c505481d1998923ea7c74`  
		Last Modified: Tue, 12 Jan 2021 01:43:14 GMT  
		Size: 181.5 MB (181483664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:351a5c6c0582ba30067abe0d39793326686b8dd7b1c068f8b30138b9820e6b09
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.7 MB (289712622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74eb074d50a54cda9cf29fdf1b2d4f12ca7cc8dcb8796c62a60105c1246ed89e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 11 Jan 2021 23:59:52 GMT
ADD file:ad9ce4dd05291eba636daae5f0b9de510927734ac26dcca6940d93e88b5c5330 in / 
# Mon, 11 Jan 2021 23:59:54 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:11:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:11:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:12:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:14:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4ecb0a075e68a9a1a4b7394123b05b2811afa9bc0a23170e2e6c42d5ee19a7ac`  
		Last Modified: Tue, 12 Jan 2021 00:09:56 GMT  
		Size: 49.2 MB (49159573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dea32ec53c55b5a19d9fb093241be9ba6e2fe2fd55963111e57d39b0973f01c`  
		Last Modified: Tue, 12 Jan 2021 01:27:54 GMT  
		Size: 7.3 MB (7265094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4b285ad78deb9119d75d41a2decc62fd9676078225d860eec32d20835fa7fb`  
		Last Modified: Tue, 12 Jan 2021 01:27:54 GMT  
		Size: 10.0 MB (9975049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e47a7484b9800c33e8812962a70ed0114c8572b070a16230fbfcd1c09b7a60`  
		Last Modified: Tue, 12 Jan 2021 01:28:31 GMT  
		Size: 49.6 MB (49587245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ef31ae7211e144bec0e79d33cfcb609d9bac6a1f0368146ce60b1ccee3bcf4`  
		Last Modified: Tue, 12 Jan 2021 01:29:36 GMT  
		Size: 173.7 MB (173725661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e6758e27ebe539eebfdb1e7af27b00380dbb1dfd1e73f29b46053e0901feadd0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.0 MB (321037802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14d55ce6157b804eafe2dc59cb7c43de411e9837f0e00c349f8af4ce6e77bb6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:49 GMT
ADD file:0700c58361c6ae34d399d7ca2a5a6f509980a496c07d319f7455d86b483e7f25 in / 
# Tue, 12 Jan 2021 00:39:56 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:19:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:20:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:20:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:22:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1e62204d5e176f9e5ef453b346203f7bda9e22ed810a0a4e2c14548d7cc3afe`  
		Last Modified: Tue, 12 Jan 2021 00:50:17 GMT  
		Size: 52.4 MB (52428437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f37b86a934fe39fb5aebaff30977af7d0075b2eeb06b1b794582ae2566dff1`  
		Last Modified: Tue, 12 Jan 2021 01:36:53 GMT  
		Size: 7.8 MB (7840062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0908ecaa573834d3855dd61a0aabaf6565245ab200624d87774802a93f1b2dea`  
		Last Modified: Tue, 12 Jan 2021 01:36:54 GMT  
		Size: 10.7 MB (10654799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8b5a3d04882a1f9723afda0d32fb1325ffa21fe435e1088c0b1736b2ba28cc`  
		Last Modified: Tue, 12 Jan 2021 01:37:17 GMT  
		Size: 54.0 MB (53962123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5592b7d4b54a1ed855e77b1f5d140002a31dde11ef835179bd01efe8dac5ae`  
		Last Modified: Tue, 12 Jan 2021 01:38:14 GMT  
		Size: 196.2 MB (196152381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c573a1e0c75a2a79348dac86ff38843612214ef1f9dda8efa438175a5b935e67
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.2 MB (335220401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3beabd4bcbbf1a6cbfe335a6040ebd8b902491bde75f978cc2f6768eba6f561d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:38:50 GMT
ADD file:5bf2c8336f63e88ae7e3d1d6804439d7f6a54937823f8e72b84f8bc95c97391e in / 
# Tue, 12 Jan 2021 00:38:50 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:15:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:15:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:16:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:18:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a8d8d38d6122a88724bab503447c48e782190ba13d75634b2b651e6dbe0a0225`  
		Last Modified: Tue, 12 Jan 2021 00:45:03 GMT  
		Size: 54.6 MB (54617930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c3a2f57bfbcccfb355c377855cb08176af609e0a121945636c2af1f19b110`  
		Last Modified: Tue, 12 Jan 2021 03:29:40 GMT  
		Size: 8.2 MB (8157573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e0211a7714f69b0754581dbc4d3b367733f5113d0b6a49c72623b3327621b4`  
		Last Modified: Tue, 12 Jan 2021 03:29:40 GMT  
		Size: 11.0 MB (11032217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e630fdae63dfc10347058d61bc56b367781b3c5d80f350c52f780f10c94a1d3`  
		Last Modified: Tue, 12 Jan 2021 03:30:07 GMT  
		Size: 55.2 MB (55156746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed133c183a9f5641f71ef7bdd7f454e3e83299e4a51aab262984118564e19f6b`  
		Last Modified: Tue, 12 Jan 2021 03:31:05 GMT  
		Size: 206.3 MB (206255935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b063004b1efd19a5038d2d567b1840356deb2c1155c8abcf31ee753211bdf35c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.2 MB (308195143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e6a906b1b929635c1387f58cf4c1c2b20bbbad9efe2319acffadfe33dd15cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 01:15:12 GMT
ADD file:171276d9060030f06df201450c4356d6449f4c6a905d02db7f2371f7ed26b34d in / 
# Tue, 12 Jan 2021 01:15:13 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:45:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:45:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:46:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:49:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cdc62d8dca2f8e7c324fa9f4efc40193ada4c98be9ca6b3f1388ad903e4bd5d9`  
		Last Modified: Tue, 12 Jan 2021 01:20:56 GMT  
		Size: 52.3 MB (52264790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60b87fc90acd9bd7359cfb81de768ce7f4cdc0821db3ed523142fe855433832`  
		Last Modified: Tue, 12 Jan 2021 01:58:49 GMT  
		Size: 7.5 MB (7492735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6084ef3498948096f602b4aac1a0fb7a2dbaa7d5d751897ddec139d2cebb08f`  
		Last Modified: Tue, 12 Jan 2021 01:58:51 GMT  
		Size: 10.7 MB (10657326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d002bf71507be6bd90480c0b53df54edfde519a712016ceb3e562397e7259f42`  
		Last Modified: Tue, 12 Jan 2021 01:59:44 GMT  
		Size: 52.6 MB (52588286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c881ad6b44a52f076da88203cb158447a4f1cfe756338cf1be55d7cb50552b1a`  
		Last Modified: Tue, 12 Jan 2021 02:01:56 GMT  
		Size: 185.2 MB (185192006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0549af4dbd8b7be8c2dfec161e8fe9c99ac33566c2959ce7a0ae7f249004db3b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.1 MB (338109806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01b9b6f26e528c702ea931c7de96a9003bb9fe19ca2dd1dcae5083bec129ccc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:23:03 GMT
ADD file:840490bff9a0b2cb1e20599d893c1160f6884327f51294479567e5d43f91b885 in / 
# Tue, 12 Jan 2021 00:23:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:39:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:42:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:58:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d21ce86f5496c36ba2ba289acb977a3b160c6c56fb257c10e3adb8b55164a16`  
		Last Modified: Tue, 12 Jan 2021 00:32:24 GMT  
		Size: 57.6 MB (57562164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d42b61558772eb59064c0ebad8029e0e7524bf865c29218b048871cd3e43fe7`  
		Last Modified: Tue, 12 Jan 2021 02:37:14 GMT  
		Size: 8.4 MB (8431230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663cfe2e2cfc28477e509f0e7aaffd4159d2f37157b32a7327bb6f43a7508ac4`  
		Last Modified: Tue, 12 Jan 2021 02:37:17 GMT  
		Size: 11.4 MB (11421868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe449d18af822c075f40a6ecd99422667906a91875941e650eb90b9743412ec4`  
		Last Modified: Tue, 12 Jan 2021 02:37:47 GMT  
		Size: 58.1 MB (58136248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210b3449c8291088f7275f584257b0d05753e64c6666b2b09ff58782b600765c`  
		Last Modified: Tue, 12 Jan 2021 02:38:43 GMT  
		Size: 202.6 MB (202558296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:443d285bc1ffb143cdb4b1f698b51a2ab9f6dcc68c57089a020df0b847c5109d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.9 MB (302859732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae125b81f2ed5d4c83d1accaeba68360a41f2748e68d64c705ad1e9c657cd0b0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:41 GMT
ADD file:5007beabc318acc6a33d879e231105324ef7801fb709d3d69813b180e883d64f in / 
# Tue, 12 Jan 2021 00:41:44 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:07:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 02:07:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:09:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f1b527eede6bdcb4cce85e897c3a92fbf04bb476403758d3b535dbf6e388d192`  
		Last Modified: Tue, 12 Jan 2021 00:45:27 GMT  
		Size: 52.1 MB (52107904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f7f4dc3450e7b31e01a1746ba85df290d5b698d495c8ab448923393956e52c`  
		Last Modified: Tue, 12 Jan 2021 02:16:42 GMT  
		Size: 7.6 MB (7649499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945c37e35656a95430c56e2a6bb0a416252a37130eca65d1f3beee38efee696e`  
		Last Modified: Tue, 12 Jan 2021 02:16:42 GMT  
		Size: 10.5 MB (10525963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7df15c7e29c90193fbc5bf8d91410b9860ebc7c3975d2951c83c543f5cef88`  
		Last Modified: Tue, 12 Jan 2021 02:17:45 GMT  
		Size: 53.3 MB (53327354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c3bff3ba098dec8b91e286ffc94a19d9311b5981a74dae3dd90763f8dbe259`  
		Last Modified: Tue, 12 Jan 2021 02:19:06 GMT  
		Size: 179.2 MB (179249012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
