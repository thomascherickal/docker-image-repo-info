## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:081f73114fd1179247d6c52d4587a49df29db04e3674ed3ed33041427c68668a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0733bc03d34f574505df1a0cfba342b7bd5815837ad135480b60b8241f09841b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.6 MB (245638896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:282add056a3925d0513e2e9ad1f897312d0c20a8496a9eebf2f2d5bc525b1216`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:30:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:30:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 01:31:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:33:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722543eba393b6f25a2387b7f7fb5f0247f569506480360827733f1c7eacc0e7`  
		Last Modified: Fri, 22 Apr 2022 01:44:40 GMT  
		Size: 7.8 MB (7767495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09dd9938f985bb6f9e7b84a36bf26a8f5b9a6ce8d302df592a4dec2f5cc9a6d2`  
		Last Modified: Fri, 22 Apr 2022 01:44:39 GMT  
		Size: 3.6 MB (3624092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3211c2e623bb1f112789227d2d89780ef2b2aa4c4c4a1de78e90224e31c025`  
		Last Modified: Fri, 22 Apr 2022 01:44:59 GMT  
		Size: 60.7 MB (60724316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10e0c106e3532779fee5a6519b2c7a85be2eae445a01d37e30ad43d00c9b68c`  
		Last Modified: Fri, 22 Apr 2022 01:45:29 GMT  
		Size: 145.0 MB (144956995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bdafcf383d45f98a0222e82575ff6fa0a939eff8bac911e3c1b821241ab0b543
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.2 MB (211221386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7327f3e975f9998a8059b25347ff742b75bc8dd4ad35cace88daef7c68cd6544`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 21:52:21 GMT
ADD file:9f59ddec8394f9caab43f06cc89a42cf98b954a4704adcde23a874a6fbb1c15d in / 
# Fri, 22 Apr 2022 21:52:22 GMT
CMD ["bash"]
# Sat, 23 Apr 2022 01:37:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:38:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Apr 2022 01:39:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Apr 2022 01:41:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cae38e1acea3c4adf05af9bcb2081c5bd7b91154184db4b1cdc06deb53699b45`  
		Last Modified: Tue, 19 Apr 2022 13:14:36 GMT  
		Size: 24.1 MB (24074069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e00f37da1cee1efe8f3ed0a439fe489465bc7513311aa2ca3170bbc560cd4e5`  
		Last Modified: Sat, 23 Apr 2022 01:56:38 GMT  
		Size: 6.8 MB (6762032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64c80b52697a36bb40c76df32329cd361aaa2a3845b3a09ac751be3d3d9f518`  
		Last Modified: Sat, 23 Apr 2022 01:56:36 GMT  
		Size: 3.1 MB (3104206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8eb7d48a855c45758024d676fd7c67e43eda42914445b7d3e106246e555b28b`  
		Last Modified: Sat, 23 Apr 2022 01:57:27 GMT  
		Size: 55.5 MB (55450852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f850684e88de0909e9b3d9d6d7220e22b210b1d3ef8f7d0440687372ff63e12c`  
		Last Modified: Sat, 23 Apr 2022 01:58:50 GMT  
		Size: 121.8 MB (121830227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:08c309a4636ad7214e0fa8f35fc3ecf909fc66b6b8deec9700b027f6d4ec0595
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.3 MB (235349588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae96714be08342fde3e7ccef298e630e4bfdb6832a01a4e4cfbb2e743f6ccbec`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:11 GMT
ADD file:6ca4a270cea388f6267a1c7739fd787a34793f48bf8480740a383b5e73299af2 in / 
# Fri, 22 Apr 2022 00:54:11 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:31:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 04:32:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:32:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e1864f78be077e322819a4ce1e09da9389c8119cf552629dc048b713a3f42b`  
		Last Modified: Tue, 19 Apr 2022 13:13:57 GMT  
		Size: 27.2 MB (27169141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74fe2982ff8180e5b5c372c1f072dc9096e3aed337880012ec8898e140f2dc2`  
		Last Modified: Fri, 22 Apr 2022 04:40:00 GMT  
		Size: 7.6 MB (7633835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a5ae54463f481880df42328a0f1c57de3dd2da4998178d5094bb9227bf907d`  
		Last Modified: Fri, 22 Apr 2022 04:40:00 GMT  
		Size: 3.4 MB (3386488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7938fea964f7c21bf653e20f3d7731b6ce278cf456197569aac468959bd5a21`  
		Last Modified: Fri, 22 Apr 2022 04:40:21 GMT  
		Size: 60.8 MB (60776385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77274329672f48affdf04b9bc7bbc93834eaf0e94bbf167c08f1e6999338c97`  
		Last Modified: Fri, 22 Apr 2022 04:40:51 GMT  
		Size: 136.4 MB (136383739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2df6814e3217b6055fc7376c8a55ddebc10d99da8e8fff4f6e49a96313155419
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.3 MB (269339348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4e15014c4f5574c92ff08e3a93add7806087914c375a07e3767c39b35bc7d7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 08:08:14 GMT
ADD file:f1c44e93e7a6c0fb06800e11460dc680e252dff4a20297ab2eed86e559398616 in / 
# Fri, 22 Apr 2022 08:08:17 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:16:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:16:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 09:19:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:24:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:30c729c4ac9a0cf192e6c3e5618b0e930ca2ecdd73c01d9c5fed5b0707eb8836`  
		Last Modified: Tue, 19 Apr 2022 13:15:19 GMT  
		Size: 33.3 MB (33290375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201e69fef602ecd9c604dbc526e412a7f9f53da3d9073dcf9b13e90174bdc39e`  
		Last Modified: Fri, 22 Apr 2022 09:41:50 GMT  
		Size: 8.7 MB (8721811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2269d321fbb9bc5909b0f64e4bd17d6910613bd979b25648123ea6ada12e8fcc`  
		Last Modified: Fri, 22 Apr 2022 09:41:49 GMT  
		Size: 4.5 MB (4456029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16173b57d4ef7ed2d38f9b4db91f53dc363095ca8362df80de0e936beefe33e`  
		Last Modified: Fri, 22 Apr 2022 09:42:17 GMT  
		Size: 69.4 MB (69419169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859c64aeb8a32ff20e3f4560849b31c54c94c8d84d345d7eb6e0a9254ff70f0c`  
		Last Modified: Fri, 22 Apr 2022 09:42:57 GMT  
		Size: 153.5 MB (153451964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:93b49d57c3b4fe00589bda757d5675c84040a6e9fe4260d76b103174c9d4ed34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226439445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:957f32772700167bcd2bdd217b3f9922d3a8a6b2134570ea831a8d17ee69b0e4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:34 GMT
ADD file:a5fe3b5fef5d5d99022e3a45894edf18c9e5f79c4be8020d61724cdc164256b3 in / 
# Fri, 22 Apr 2022 00:39:39 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:34:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:34:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 01:36:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:37:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:716ba34a9a0241d7bed3fa68865e745000f025af68d21dab7d692215c5074a58`  
		Last Modified: Tue, 19 Apr 2022 13:16:37 GMT  
		Size: 27.1 MB (27085718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7951284cb68b6a00917429e8710567f9cf59ec824346159a9713e70fd897f937`  
		Last Modified: Fri, 22 Apr 2022 01:51:30 GMT  
		Size: 7.4 MB (7422499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908eb104679df5b72b639e9dae6c144a0e2c32ef5438c9f65a897d136539dce8`  
		Last Modified: Fri, 22 Apr 2022 01:51:29 GMT  
		Size: 3.5 MB (3542368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6882d1539676b156631ed86fa61945c5523a759c52d3e9d64784fb441aa719c`  
		Last Modified: Fri, 22 Apr 2022 01:51:49 GMT  
		Size: 60.0 MB (60009418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c402f7e86545a380f5dbe46f229b26e98397dfea4a710547e1ae2a683f5990`  
		Last Modified: Fri, 22 Apr 2022 01:52:16 GMT  
		Size: 128.4 MB (128379442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
