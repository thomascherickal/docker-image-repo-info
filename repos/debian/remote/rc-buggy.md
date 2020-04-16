## `debian:rc-buggy`

```console
$ docker pull debian@sha256:509ffd78d53cc05df71ba532afb9460f0d34e94bcc6b3db7a6c4fba6fff0ab70
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
$ docker pull debian@sha256:4bf18bf6897ae728888d62366eb00c51b175ec9d761c54df1773755ceafce440
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50882959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c16764e8c573b8352ba069f99c7e20a872ca0a5fe149e014edf7353304e8a044`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 02:06:41 GMT
ADD file:89d1d53ca595aac3a67a5b8b833603f2f27cb35fff838b1e022c7b8d9ab52c27 in / 
# Tue, 31 Mar 2020 02:06:44 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:10:28 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d022a4286a83893fda6e1ecf3f90454f2247ecc550aae515cf06acb929d6340b`  
		Last Modified: Tue, 31 Mar 2020 02:13:07 GMT  
		Size: 50.9 MB (50882731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0a66a391713894ec23013f32966921536585d488a978291754ba30a53b851a`  
		Last Modified: Tue, 31 Mar 2020 02:16:17 GMT  
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
$ docker pull debian@sha256:b0566f1a0885fb8172d6ae1013f74ecbbcdb6c13e49977531f5443e78738b16a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55835165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b31c7d7a9ea539db7bf72787f3694a65d82f48ce772aa17dc3948b08252a51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:34:16 GMT
ADD file:8f010ac42180d1a69abeb831a2cf65af2b505dc37ca5566d1f8e0af98223a68d in / 
# Tue, 31 Mar 2020 01:34:25 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:39:36 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5a96cc3285dca9557b63f3a1daed7cabe2c2e3fd70599474a054f37ae9105c6c`  
		Last Modified: Tue, 31 Mar 2020 01:48:49 GMT  
		Size: 55.8 MB (55834936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9657bf84fc9144585bc0ba1471997b7f7282b2ea7c08b5bc6df55efea8bdbbc2`  
		Last Modified: Tue, 31 Mar 2020 01:58:25 GMT  
		Size: 229.0 B  
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
