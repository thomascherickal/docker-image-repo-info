## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:95542375733745da567ef600959c7910fea6f6969563ddee82e7cdd0e109d455
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e042672f1de31e5ecc5bbf7df2a9eac7d1cc012a5a620ec3b0b5aa0ccae9e610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110781699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49daeb05d0974f360f43581a6691f08a5b169f1813fcc867a41293f40e7e4b5e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:15 GMT
ADD file:36e7d2a782d933f47ccfc8692ebf95cacda9f109a51c46514f00b78754070254 in / 
# Tue, 28 Sep 2021 01:25:15 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af4c2580c6c3e68236ce4f353c045f871e4780b85fdb54c00529426e09bc36ce`  
		Last Modified: Tue, 28 Sep 2021 01:32:26 GMT  
		Size: 45.4 MB (45379654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea40d27a2cfcec3d38b2a0ebe5ca77633d27a394541c449b500fce4639516d4`  
		Last Modified: Tue, 28 Sep 2021 02:01:24 GMT  
		Size: 11.3 MB (11297892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523d612e9cd24c2fca3c4d97b340e89c7dc6bb326a9d75d5a0476f56680d06dc`  
		Last Modified: Tue, 28 Sep 2021 02:01:23 GMT  
		Size: 4.3 MB (4342401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fee6a1847b07f4933116726f66b9218dde8c59d1f7b94de92f9f0683571a362`  
		Last Modified: Tue, 28 Sep 2021 02:01:42 GMT  
		Size: 49.8 MB (49761752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6a816944d99fd57824326754aafd407ee856c330276eb41194f40c7ad02ada82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106588257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf701630150bd83ffd677ef202986223117afacb24dc86cc90592ff66cefd33c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:05 GMT
ADD file:f294a28ee9da17e8a289348f6b85aa865b9f1925aebadee96124e1d4a81c8401 in / 
# Tue, 28 Sep 2021 01:56:07 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 03:01:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 03:01:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 03:02:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a237f80116468b0593b0195bd02cdb78fb8bea8e44f206ec86fd61a9377d7a06`  
		Last Modified: Tue, 28 Sep 2021 02:13:48 GMT  
		Size: 44.1 MB (44091934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ebbdc0a8d4cc096a5c44b4a13000717d6e8dfeb21442b4b375e5d1b9327935`  
		Last Modified: Tue, 28 Sep 2021 03:17:12 GMT  
		Size: 10.4 MB (10350664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaa304c7ee32783cf53bf48ea782d989a9874bd108e27ddae6d1adfb8b2eb3f`  
		Last Modified: Tue, 28 Sep 2021 03:17:09 GMT  
		Size: 4.2 MB (4161453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e7d03d992607295ece45259f5362cdffa8e3620933d03ee8100e7b58f2ced9`  
		Last Modified: Tue, 28 Sep 2021 03:17:59 GMT  
		Size: 48.0 MB (47984206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2e3b13a826fc616ef225b08428059bbbe6fad1d52fab5bca1ed3745152a47070
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102122379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aafc37f0496b761630fecaf39bbcfd07af95e1926751d29862b817689908995d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:08:56 GMT
ADD file:effbc465353f5199d8051d1de4db57a4630b13cee7af167ffe8bb92d6f21adf2 in / 
# Thu, 30 Sep 2021 18:08:57 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:43:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3fe5664b6df9f22a16cf7e44f293e1a45ff5f90d666a258058705f3abe8f585`  
		Last Modified: Thu, 30 Sep 2021 18:26:14 GMT  
		Size: 42.1 MB (42119512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7eacd3cabb0c1d375b065b7a41c992d34da5d0bb6b1b557e7634047833b7b6`  
		Last Modified: Fri, 01 Oct 2021 06:01:33 GMT  
		Size: 10.0 MB (9955749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d987bc3d40f9d014061a746eba028c7c856ad39c980d9b6dc3de5ba1f7829`  
		Last Modified: Fri, 01 Oct 2021 06:01:29 GMT  
		Size: 3.9 MB (3921194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a914caeb151e7903d0d778c1ae44d420945c84af10ba750a5abfda6b9a99f65`  
		Last Modified: Fri, 01 Oct 2021 06:02:16 GMT  
		Size: 46.1 MB (46125924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9c1e7cd43e43670fe1f350da75e1fb17d84ee12262a0ca4a50e28bc4e69d033e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105229149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35055b08b062ab3a45ae326dd3105f396e28445072acb2b43a382c2296bdd397`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 02:14:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6106ce195cfc2ea7282dab1677e8563168fee21f184a937b32a9370944ccc077`  
		Last Modified: Tue, 12 Oct 2021 02:22:54 GMT  
		Size: 10.2 MB (10217927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499bc8ad963810c8e2cef0d22542dfad2339032cf43a8210066a9a817fd6a869`  
		Last Modified: Tue, 12 Oct 2021 02:22:53 GMT  
		Size: 4.1 MB (4096622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91449e92d9f0601eac3dbf717abf9680c96962909ab07b8ccdb946cd89230178`  
		Last Modified: Tue, 12 Oct 2021 02:23:13 GMT  
		Size: 47.7 MB (47737903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3dd7dfec75397dae002735d04557b86aaaf641dbf609cd11f267f7740392d841
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113285816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10424f2f9fa56c237f5a1cb67f32e5286a03841b408bf07e8c6d4f87b5757030`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:42:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9020db84c7cf31b7929c21a2b6fe2123900e91c7391ad6f4ee5560a934f382`  
		Last Modified: Tue, 12 Oct 2021 04:52:49 GMT  
		Size: 11.4 MB (11358857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8cbe9196a8b6bd3825445c718bc5a248b7c295b4d9f45756819e8bf27cb72b`  
		Last Modified: Tue, 12 Oct 2021 04:52:47 GMT  
		Size: 4.6 MB (4565012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7454f0fe0ebf5d024897d682d46181ab978a980f7f40caa2492a83cc39f75ec`  
		Last Modified: Tue, 12 Oct 2021 04:53:20 GMT  
		Size: 51.3 MB (51264783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
