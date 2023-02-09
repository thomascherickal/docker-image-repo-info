## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:68815c48aa5d657748d73f93c83bc4a304a017cebfa8d05230824c27f693ad37
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

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:56f8c111573567cfa35fc79f64ae8cbbab72fe19659f28bc70133e1836193eb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71067485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0800fe62d0d170a7731adb37d176bcfa73d80a1d2b87e423c640ce94ff512a0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:88d6bf7f297c65361a8de6f3fdf1e7253d735ebcf86e85cc286f5b9870e759bf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68198024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cccf748dcb97e9be4012b53c0e5376bc79145a80fbf056ed84a28377fa4dc4e1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:31:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:31:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2355e17d09850c64d649a557a5480aa67d5780f54692d771fe1c9c1a91982d`  
		Last Modified: Thu, 09 Feb 2023 02:37:33 GMT  
		Size: 5.1 MB (5072358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033683e85ebf7bf5988c5e89fb437d067288a5d39c937e111cc7aba783033475`  
		Last Modified: Thu, 09 Feb 2023 02:37:33 GMT  
		Size: 10.6 MB (10573870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:58088822c082b8bb558a5f0f42196f5946fbc58ce60f5b341b4c7fc538d65a7e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65341944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:747e35b1d9fdfd612617a1ff76c69b4ee71cb7b4da9a868db6bf56313ffeccab`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7407a6dee0f4cc9a09e3ea72223db77f358d8bc451430ebb883596bfeadc2920
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69706696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96a319af67840ea0be3bdb27b4f43e3191bcff9ec03c1b808bbdfeee2e90eb87`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:45:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:45:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38880e907cdcb0da4f6bddfc0380aaa5b11d6adf12bf87034adce6372ba306ba`  
		Last Modified: Sat, 04 Feb 2023 06:52:03 GMT  
		Size: 5.2 MB (5151209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8181793414caae285b5e035037e19a57765aa12828ef23dd5e47e7606631696`  
		Last Modified: Sat, 04 Feb 2023 06:52:03 GMT  
		Size: 10.9 MB (10873560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b8e5430ffecb1e1f5234e821ada755c2c75e013511ec294fb072da5022d608b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72330019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcead7a40ecbdcda82781baf3f855239d87bea7aedf2b171f174323907b329c7`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:19:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:19:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebdf79aa6d9b2be45c2a0949ac3677ad52629968a8cf44b6973890003395dd`  
		Last Modified: Sat, 04 Feb 2023 08:27:01 GMT  
		Size: 5.3 MB (5291983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ad836118a1e95a24ffd64386a98d933a2a2f96eacc3e3a3c13804a31d7008`  
		Last Modified: Sat, 04 Feb 2023 08:27:02 GMT  
		Size: 11.0 MB (11032558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4b7b85b9386e8a62061db8f6de3d3f14d9c766b5afc78bce6a2277e61cb0d35e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68850538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e15959eca1ab694d171b213aa90363b529e588c0d215964cf8a4c3e6e8c0acc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:40:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d791a92fb38ebf78f5ed530cc39361869dd25ce941ea09d0580b866204f0e8e1`  
		Last Modified: Thu, 09 Feb 2023 07:59:50 GMT  
		Size: 4.9 MB (4921594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c347eddc487950d631dca4e7c20c1165566e8418703435fad325a721c0e8d`  
		Last Modified: Thu, 09 Feb 2023 07:59:52 GMT  
		Size: 10.7 MB (10662160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:12817cd0bbf75ce52e08aef456b73d53b18684709ac67f275aebb55bbc58b8d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75940979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90fba18621e51c45ddc5fab47d77fea751b6cda7eb72aef04a5bff0d570a6f0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:02:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:02:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01c913909aa7f93cc6ab033f1f6e61f49370709ea387f35a2022e742cd5d42b`  
		Last Modified: Sat, 04 Feb 2023 18:14:41 GMT  
		Size: 5.4 MB (5414184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edacbd3dc421aaeb6108d87b4dc4870994392f896c53946184172b80601b6659`  
		Last Modified: Sat, 04 Feb 2023 18:14:42 GMT  
		Size: 11.6 MB (11629731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c2507fe41cebfcad55c3fa9057dc9b8db9152ca20a9fdd8d73680b87e9c57134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69194092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:380526f174da4e2856e792c49f3f5c6fb5d9ee6f0685ca38fba173dfdb89f136`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:27:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:27:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6c93cabdf59ed2ae0e16b55f3f3c261e3d470a151aafaebfb14841492c699e`  
		Last Modified: Thu, 09 Feb 2023 07:40:29 GMT  
		Size: 5.1 MB (5148933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89bee0eba54958a826e0c254b818763de9882b96810e4be6ef4f388284b68db`  
		Last Modified: Thu, 09 Feb 2023 07:40:30 GMT  
		Size: 10.8 MB (10766263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
