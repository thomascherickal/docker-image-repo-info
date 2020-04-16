## `debian:rc-buggy`

```console
$ docker pull debian@sha256:6745d68a0ff463b1e4b04723b02733693d6ee016a324c8cfb0ac8be22153daa3
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:a3a97fe2f73df4a52ef339f887171c75a99d39be232d1d8d8a26bdcbbd6a0c65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51949907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42259fa414d18433f876b07bfa92c86a335df9f3f66821af22a7a71d483570b0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:22:48 GMT
ADD file:7562f01f4040e4f21a40337301dd14e4377f3d101bd0919a96ae05bff37d7087 in / 
# Tue, 31 Mar 2020 01:22:48 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:25:18 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:616821eae326bcd1b2974181d172e5949f2c8c091398159b63b0f483913be88a`  
		Last Modified: Tue, 31 Mar 2020 01:28:20 GMT  
		Size: 51.9 MB (51949680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2f9241c0c9662e3cbef87039cceb65590240de5c7eac2b7c644679bc6cb6b5`  
		Last Modified: Tue, 31 Mar 2020 01:30:32 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:dcf26ec00ebaf3e582fd60b161f02ff14f43b0567a7c78fa1959adf5ab9f397c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49930977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749255c4e4e9d7b5f3ca5f1ab53657c6e663bec0e2ceb98943eded4f8164a9d6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:52:56 GMT
ADD file:bd1d9af70dc12dc4f17f2b7768c241504faf686b41fc7a690e618f93048fde8e in / 
# Thu, 16 Apr 2020 00:53:01 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:56:35 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c1a8f9f50766a877cfcad4d61e0db97b4f5cc37823b5af730a9b1e2a867d6410`  
		Last Modified: Thu, 16 Apr 2020 01:00:47 GMT  
		Size: 49.9 MB (49930750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5a08e0a72f6bfdffc513b2e2b6dd5ea3eb668ee7e77f1aac4d36c25dddd0fc`  
		Last Modified: Thu, 16 Apr 2020 01:04:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:5599b08fd45f8ffccdafd58c4e90254703ecb5e45f43c72d9568b7aca5f4eec8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47655645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6928af2aaccba746d4cdb4ec313eb495cee51e310ee81ff6c6428436fa803830`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:02:49 GMT
ADD file:5de6dfe62ae35545ab2dc195cdc7ed6211867d4583f721d08acfff371bc7cecd in / 
# Thu, 16 Apr 2020 01:02:51 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:07:12 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9d58ce8574bee4c2429ae80f47b2650443254f3f9a0dd9fc1c8d64277895520c`  
		Last Modified: Thu, 16 Apr 2020 01:11:11 GMT  
		Size: 47.7 MB (47655417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da7d91e5c1ec36b1ee0d05011506444062aca7d3c7dcdb1ce5e2087ecfd831e`  
		Last Modified: Thu, 16 Apr 2020 01:13:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:2a46c5910c3679e374a6af8380b203a6399a47fa40f87ef8f15570a26db737a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50910266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9833de3e1ad8a6a77a1bdd762d7589d7d2b16eaad9e775eb943a5b65975a40`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:43:10 GMT
ADD file:ff8b5c2517d26b49a4c8114e515f5413a0c64b28ff1e5d3fa1bd70603aaadff6 in / 
# Thu, 16 Apr 2020 02:43:13 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:47:18 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2f361d4eae096128866baf55f9d19448df20331f319ad8df0f05397bfd2fe7fc`  
		Last Modified: Thu, 16 Apr 2020 02:49:55 GMT  
		Size: 50.9 MB (50910038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739460fdccfd5e56d180db795788aaa154e5e15a24bc61535c35dbe5d928e191`  
		Last Modified: Thu, 16 Apr 2020 02:52:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:08cdce11c288f76ce25493698b72b2e6d7f4f0c045f81a5e6d85119b97ff2724
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53130267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60989f9c1deb61067396eb902bbe729db47c557ddf2f146b4d85045552effeb4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:41:56 GMT
ADD file:af11f81927371cc0ed957aa36f4036c71c73a0b79ab27523cf0d49d8e0260041 in / 
# Thu, 16 Apr 2020 01:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:44:46 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1cf4ce40baf558f42709af03658907805f477c72b1b1a39869aef429cd35cd3c`  
		Last Modified: Thu, 16 Apr 2020 01:48:16 GMT  
		Size: 53.1 MB (53130042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfcd8282e43dbf1cea77e28bd5ad700b732bba316fba970acb53effe0f23774`  
		Last Modified: Thu, 16 Apr 2020 01:50:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:67a66bf0b745f030a537eedc2d43aca5026f7001ba8935b4f77973ed28ec2738
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55860722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:691c0f3a71b70cfbdf9507774b3f02ac3014d101a17161849a5be4505715eb69`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:40:28 GMT
ADD file:68afd6d0e23ee44127b8e1f922e1a6977efc12c46c7aa7afff807e146187d870 in / 
# Thu, 16 Apr 2020 01:40:38 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:47:34 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2b17b1afa1bd62e539e75bfdf0ac70297d76a76fc7df9fcbbc67ef6c31717636`  
		Last Modified: Thu, 16 Apr 2020 01:58:42 GMT  
		Size: 55.9 MB (55860496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471b39a9eaef3316ec47d72bc88b0ca7ac8cdb6ac7819b763b7ff74102c21fb6`  
		Last Modified: Thu, 16 Apr 2020 02:08:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:9aef58a1d00eb649e5bd82086947bf1911acc6269d87d3a0fff0ea294852db65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50576768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe0c5ea939294cf7e6b580171d09df588bb9ea7823890fc4ece66a1e14a7135`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:56 GMT
ADD file:1d96a73c9c03d31b0a60aa6b4e0215085afcdee6dc39954655798110c12c223f in / 
# Thu, 16 Apr 2020 00:42:59 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:45:02 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3633d30b569d7f8e4addec62b3bb5c460572eb82d6568a9bc40a9f189dc4bdcb`  
		Last Modified: Thu, 16 Apr 2020 00:47:02 GMT  
		Size: 50.6 MB (50576543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaca0a3bce5169f41f3ac3d87cd12d99b2642f25d43b674bf973ad8ff65ef79`  
		Last Modified: Thu, 16 Apr 2020 00:49:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
