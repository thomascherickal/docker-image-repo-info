## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:f27195f537e96722286197fcae0bef5de85e74881b5c447bb08d3a81f2c64fb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6b16d828283382d7bb3097a1fcb9def9262662cf23258a15d5d2d100e31e81f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.1 MB (323129645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2edeaccc8ffa4777f5c3de18e463eb4f29c6c0308523b6d263baecfcfab29c1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:21:21 GMT
ADD file:d8f8a66e04b091b1ee6d1d330b5cd80472768f8cef96db861ba4dfaa2472fe20 in / 
# Thu, 16 Apr 2020 03:21:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:57:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:58:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:58:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:59:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d9ec154a243cb2fcf510aa97241fa4d7c075add5b018b19db3f1dca9f93c83a`  
		Last Modified: Thu, 16 Apr 2020 03:30:54 GMT  
		Size: 52.0 MB (51968339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f52bafd3e8510b30e30d2ccb5e044a4647586a4b5dcdee4e79b63b54296a77`  
		Last Modified: Thu, 16 Apr 2020 04:14:57 GMT  
		Size: 7.9 MB (7932617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61caa2b6b1a3f079feb31d0b6ce33740955163e262ec2f624070129b13ebc779`  
		Last Modified: Thu, 16 Apr 2020 04:14:58 GMT  
		Size: 10.3 MB (10298054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c043d752dd56512f49ba5efa050e0701eadb2605cd22b197ccffd7aef9ba742`  
		Last Modified: Thu, 16 Apr 2020 04:15:13 GMT  
		Size: 55.3 MB (55327131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b82bbc591fc6eff56ece85758231f4247dc995887d4c15339d736c17e97667e`  
		Last Modified: Thu, 16 Apr 2020 04:15:54 GMT  
		Size: 197.6 MB (197603504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7e2145c7574681908476a738c8af465990c3cc09aba85bd2d5c92e454e24fad9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295428790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c60bb4fab097e81393b0821bd8bb9a57fc476029b4042c067ac7436e3d7b35`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:23:41 GMT
ADD file:4315cf04b632155858b9a0c6d22c433dba5c9b23c240abe83ceeca80e94a841a in / 
# Tue, 31 Mar 2020 01:23:44 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:18:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:19:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:20:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:23:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0806b4d4e10fd104cbda1f65b5dcee9a5b4202716f5e8367e2bff3143216eda`  
		Last Modified: Tue, 31 Mar 2020 01:32:04 GMT  
		Size: 49.9 MB (49920582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0382c643bf4a04c23f9e10efeb789cdadcdcbfd9c890261da945bbfb379473`  
		Last Modified: Tue, 31 Mar 2020 03:45:41 GMT  
		Size: 7.5 MB (7504856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d3b4a29b142be89febad4954c371a81253e3970f04a9664005d4733ece339f`  
		Last Modified: Tue, 31 Mar 2020 03:45:41 GMT  
		Size: 10.6 MB (10645298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7480e7f26a4fddbd2129e9273b18dfd1c9e33989b1cf84be529e4861c12598`  
		Last Modified: Tue, 31 Mar 2020 03:46:07 GMT  
		Size: 53.0 MB (52964859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f805af4fcdc6590c0feea9ea5dadc1d0735f20fc8fabb9818c64b816ad6983`  
		Last Modified: Tue, 31 Mar 2020 03:47:03 GMT  
		Size: 174.4 MB (174393195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b0ae2edf42ab4247d850021931693814a477904a1109cacffc0127a0f19a05d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.9 MB (288899867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4ff9b23ab5a801721b7bbe2bb5698e91dfa207207c1a4266328e139b16b5a9d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:58:05 GMT
ADD file:353f89e64e5475f2d99be1c5e0eaa80d5aeb89e02c274ba507df4def8f7ccc8a in / 
# Thu, 16 Apr 2020 00:58:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:33:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:34:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:37:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a287a7fa81e293e147ba52c36ae34e643e975ef88ebe9a6f226a048dbb7ee9fa`  
		Last Modified: Thu, 16 Apr 2020 01:08:03 GMT  
		Size: 47.6 MB (47646389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47358f6975165f42a9cd9b867f0d03e95a00b52627d5e833781a9eb45eca84cc`  
		Last Modified: Thu, 16 Apr 2020 01:54:57 GMT  
		Size: 7.3 MB (7255347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376a0294fac4492ac4a3da9b92cdf02ee87e6bfd519ee19fb996c5db96da33ae`  
		Last Modified: Thu, 16 Apr 2020 01:54:57 GMT  
		Size: 9.7 MB (9672922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010ce0dbcbdea4c6cbef9d1bda1fb769c382107cb837edfcdc6258b8421fc200`  
		Last Modified: Thu, 16 Apr 2020 01:55:21 GMT  
		Size: 50.7 MB (50666643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdbacc256820bfc69a7a869f0393a627be4dbe452325b63a794d39b480a9f1e`  
		Last Modified: Thu, 16 Apr 2020 01:56:43 GMT  
		Size: 173.7 MB (173658566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:04f9ae467d92c5438cb5298f5b9c96bb87e79ad323847f8dd080069178137d88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.0 MB (314973885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225dd837cdcdd0a37e2d269db1e8eb901e77279a112dfee00f1d6141f65f9e02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:40:12 GMT
ADD file:27c25cdd69090f4b15f9f2f4a147879d1d7510b7b2f8c231a92fc74832325413 in / 
# Thu, 16 Apr 2020 02:40:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:10:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:13:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c6bfde49c5261423574a9f9bc077a0cd0057775509f9d9e061556a16b84e1d7`  
		Last Modified: Thu, 16 Apr 2020 02:48:01 GMT  
		Size: 50.9 MB (50901465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c744c6854f291e264392cb87f79c4675b05d5383ca93df9f5b4be8f447aba3a7`  
		Last Modified: Thu, 16 Apr 2020 03:26:27 GMT  
		Size: 7.8 MB (7807688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0a53c53b80bd91c029938e07ae8fb49e75ae1d45620212fa6fc041e97f5750`  
		Last Modified: Thu, 16 Apr 2020 03:26:27 GMT  
		Size: 10.3 MB (10294224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee1bd7b8a02f00bba05f898a3f2c91d213d6fff20796effafce1437c9b6cab9`  
		Last Modified: Thu, 16 Apr 2020 03:26:51 GMT  
		Size: 55.4 MB (55385347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781ae7550177e95dc9bef60c9d79bcb961a57442a98514b22c4c66ebbd7c59ef`  
		Last Modified: Thu, 16 Apr 2020 03:27:44 GMT  
		Size: 190.6 MB (190585161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:17dc4672a7caa05f11528a46b0a4deba0bfb8e533592e4cb8bffdeb48fa7fa8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.9 MB (332902465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eea222cad7187b501ebfecbb3bee61630fdb27e3f68b19afb0951d5eb081e34`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:50 GMT
ADD file:1d78edb74644d640409b64831c000f00654603e8888b50c46ac37ca0c186c3e9 in / 
# Thu, 16 Apr 2020 01:38:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:16:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:17:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:17:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:18:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d162d6311c3b7618a8b9a80392bb71455272c7ef63938e132282070923f16ead`  
		Last Modified: Thu, 16 Apr 2020 01:45:26 GMT  
		Size: 53.1 MB (53116500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d42814ec88fe50214d62dfdaf2c1a27abf7c61f1718b16dc664b952cc85492`  
		Last Modified: Thu, 16 Apr 2020 02:35:50 GMT  
		Size: 8.1 MB (8110131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97139d647978bbac84cf0fbb6575ccf2950e262ccf617d10aa0e60e479481bb`  
		Last Modified: Thu, 16 Apr 2020 02:35:51 GMT  
		Size: 10.7 MB (10657214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29d09c18686eb52024c1b28dd62d1ffe2ca03f040d1f82bf9fcfa657d41bb5d`  
		Last Modified: Thu, 16 Apr 2020 02:36:12 GMT  
		Size: 57.2 MB (57154439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41edbb06b555fa22e066e67cdce8398634dd1bbbea141496567ac3ea4c85579`  
		Last Modified: Thu, 16 Apr 2020 02:37:10 GMT  
		Size: 203.9 MB (203864181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2d74f141d33a3874288214318e545647573a04b756503715a59d6bf584942c45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343268895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19c3f00b4a18929f3d3bec125e891df15e9843ef499b849dc9d2dbe45fe8c59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:30:51 GMT
ADD file:544f960bbf6b0c556a3946247e7163ea2d8976c01f513bb4e7ed8eb8df4d09ae in / 
# Tue, 31 Mar 2020 01:30:57 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:03:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:03:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:05:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:15:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de0d878984bf9a338e5828a66a5f63ae0852a3a1838645e030f18c29df6748ed`  
		Last Modified: Tue, 31 Mar 2020 01:42:06 GMT  
		Size: 55.8 MB (55810298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80755c7f1f2b64223e3ae4cbc62d0e4c2a93eda7f1f3734ea3686292ae264420`  
		Last Modified: Tue, 31 Mar 2020 03:58:05 GMT  
		Size: 8.3 MB (8349042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436e4215faaae7e504e17484b61fdfc1a375ec0c1b46b37361c8b0c6de944883`  
		Last Modified: Tue, 31 Mar 2020 03:58:09 GMT  
		Size: 11.7 MB (11671337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ec1de538484d05e151adf76315f07e1874120a05c2fec146d2e7440407137b`  
		Last Modified: Tue, 31 Mar 2020 03:58:51 GMT  
		Size: 60.7 MB (60652046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b32f0f81198fa30d7e2f3bd135cf0394d9b1a2f73e666c4bf88cf1c9501670`  
		Last Modified: Tue, 31 Mar 2020 04:00:57 GMT  
		Size: 206.8 MB (206786172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:96226e6202d89a9fe3141789e2e2b7f4f86226494c52a2448b4e7f5ee708b259
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.8 MB (303815127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f66a0daf9e0e3d77750003cc4ec03e851991e30aa5acdb0fceccd9e17fd077b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:41:36 GMT
ADD file:91904e1cbd0660c7c48420aa34dd58c0e8619c69afe6c1412a495c364773b5bb in / 
# Thu, 16 Apr 2020 00:41:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:56:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:56:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:56:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:58:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:929a8c37dff5f4096f453d7847637ff8b3e3fa702bd1043408eb37af338237d4`  
		Last Modified: Thu, 16 Apr 2020 00:45:37 GMT  
		Size: 50.6 MB (50569040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625f45e55816a01b4e47db24dfb9857e953051816a723f6999906fa8fe1cb40e`  
		Last Modified: Thu, 16 Apr 2020 02:05:36 GMT  
		Size: 7.6 MB (7600032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af726635ebace664ecb1c229bba4cbd77183a3411aacacaae74f1cbb0882eadb`  
		Last Modified: Thu, 16 Apr 2020 02:05:36 GMT  
		Size: 10.2 MB (10183890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216e30525b6ed08c23f0a9ee26e1498e8ad2fa322601120a5936a44f2ddbfa87`  
		Last Modified: Thu, 16 Apr 2020 02:05:50 GMT  
		Size: 54.6 MB (54565876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bd07e10ec2c37edecabea97c313ab63df95e3593b44b7753294d4a4705e9be`  
		Last Modified: Thu, 16 Apr 2020 02:06:17 GMT  
		Size: 180.9 MB (180896289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
