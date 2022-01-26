## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:cc7b9bb9bbd6658f03216d6c6728d1cd984c2b663ce28611ca42946148e83a9a
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:134588d920a54b2e55d3cc7ae1900166d4acb6f04d556d8d37f11c6c32dc2cc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70941632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1830fff917b741d987b7a7e6b50a59e7cf144247feca85ff287287a63af7dc73`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:22 GMT
ADD file:9cca7f8e4abcd8309501cad216ff33a28932386ded66461a7591c0fdf2c859d3 in / 
# Wed, 26 Jan 2022 01:40:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0c6b8ff8c37e92eb1ca65ed8917e818927d5bf318b6f18896049b5d9afc28343`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 54.9 MB (54917164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412caad352a3ecbb29c080379407ae0761e7b9b454f7239cbfd1d1da25e06b29`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 5.2 MB (5152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d3e61f7a504fa66d7275123969e9917570188650eb84b2280a726b996040f6`  
		Last Modified: Wed, 26 Jan 2022 02:22:09 GMT  
		Size: 10.9 MB (10871783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:1dd1f3fd80c3b8c3b1e325c8851efba8e31e46792d57a2c4cc9c048b6bdaa078
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68101388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e13214d319c7157048ce0e3462b9e5ecbc0f1590ba407d95e364342ba4a42f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:21 GMT
ADD file:5c238170d9d1bd220e05ede3d517d33fadd813f341546cfd0f2a29285092ac05 in / 
# Wed, 26 Jan 2022 01:41:23 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:30:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d09eefb6f859064403eeef43dadb425a65a1b745075123e6770f3131f93d2679`  
		Last Modified: Wed, 26 Jan 2022 01:56:45 GMT  
		Size: 52.5 MB (52466598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83efc7fce4dcc748daecd48cd04a42feec3863b3e40f5e21296b06f7d260933b`  
		Last Modified: Wed, 26 Jan 2022 02:54:36 GMT  
		Size: 5.1 MB (5063642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e1c09054215ea3aa61fa205896a78ebb6d0d9e130df0466fb9491fc80a5e8e`  
		Last Modified: Wed, 26 Jan 2022 02:54:38 GMT  
		Size: 10.6 MB (10571148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6d55f4b96825255d5771423f36d6634272fe44f4484e03cbee47d624e04cb30e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65256583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:056755cdff3324feccaa697055f39b14eb61b1bad173fe195ebeb859d5060e12`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:30 GMT
ADD file:19419917274a4a5aa3eceb0a6202f89e5b508368314f2bd0105897a847db4930 in / 
# Wed, 26 Jan 2022 01:41:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:37:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:38:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:046501ac4c58f014cc320324f6023bbef17f28025428833449198a62a97849c0`  
		Last Modified: Wed, 26 Jan 2022 01:57:13 GMT  
		Size: 50.1 MB (50117358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29bf76217944d3c3b29fb3234ed71ba5a004ffcec0595d3704c6e6cfa169b68`  
		Last Modified: Wed, 26 Jan 2022 17:03:48 GMT  
		Size: 4.9 MB (4922334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0e88eaa9f33e97d48fa77ed2c178123150031494073f10c97755b3bd6370c1`  
		Last Modified: Wed, 26 Jan 2022 17:03:50 GMT  
		Size: 10.2 MB (10216891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e820eae8dbf22a72ceac99b759bbf8c523449436e490e99bf43d4ccc84e82a53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69406317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c84a543a01e3633ed5bd5ec1a4d25a43b4fdcbaed3abf63cfa0ce004e22c68f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:15 GMT
ADD file:b6338a9c3c2f8d7ba1a23dcb7a1389c7d0eab75a7489ef66f21c773be56aa9ed in / 
# Wed, 26 Jan 2022 01:42:16 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:39ab78bc09e79a21f719ced771689354d1948f4afd57e86afed8dac6ffb47826`  
		Last Modified: Wed, 26 Jan 2022 01:48:34 GMT  
		Size: 53.6 MB (53608848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf88d09fc28807e643d4f619b2e0c559aaeddc7d7b8176e1144b065d63fa160`  
		Last Modified: Wed, 26 Jan 2022 02:23:47 GMT  
		Size: 5.1 MB (5141567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e019dd0368ba992803442a16cc7792c1bd5a3d06c3a1ae6fae17cb838822fb4c`  
		Last Modified: Wed, 26 Jan 2022 02:23:48 GMT  
		Size: 10.7 MB (10655902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:05891aa87b3470a8f3aa0b18f46cf23a6c0b3ebce8873faa410ab274fcbb45b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72472651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119dbe50fc1ae4148fd1149c05b07dab30311940faacf8a80ecee4566c31ab33`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:35 GMT
ADD file:dfb883d877f16913b7019d7b3bb938890bfa288a712901baeac6e1c7403911e2 in / 
# Wed, 26 Jan 2022 01:39:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:15:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:12e30620442951468b6e2349dbcb6a8a35c39b59f1cf8096f7b5eaf7ba0ec5c9`  
		Last Modified: Wed, 26 Jan 2022 01:48:19 GMT  
		Size: 55.9 MB (55939009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48de9c023436dcba7318657f0dbf29d61f11fedc2b373ae1603adb34943655c`  
		Last Modified: Wed, 26 Jan 2022 02:28:23 GMT  
		Size: 5.3 MB (5282945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bfd727d9f7b4b01a2ba31bb89f13672ebeff3d2714d7b242b5d3431cbdd709`  
		Last Modified: Wed, 26 Jan 2022 02:28:23 GMT  
		Size: 11.3 MB (11250697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:282571bcb8e3eb4c8db515ac929bf4eeb9714f979de522b21fb965d76392d8a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69168030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48faf91d03608d5b1fdfd8e40bbfee4d92966695d0ee18a1d073d4ca724eb27f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:19 GMT
ADD file:06fbff49d105bbaefb6199ecf549660a67db6cec16698f03c8ae0cf2bdfd6d4f in / 
# Wed, 26 Jan 2022 01:42:20 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:20:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:21:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6176f4ee4b1d3ab7c5f3f93bc9036b71aa337a53c743b4aa347dffebfc8c772a`  
		Last Modified: Wed, 26 Jan 2022 01:50:39 GMT  
		Size: 53.2 MB (53179965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95348eb2d40b4ceb8a78cd0f25deda3892c77ac31efd5b0650b8d374354d6b4a`  
		Last Modified: Wed, 26 Jan 2022 02:37:45 GMT  
		Size: 5.1 MB (5114720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6c8e8b27ca91be5bb90346420cd2dbf8981731b5c3b1a8a6fb3ec3df2f7b9`  
		Last Modified: Wed, 26 Jan 2022 02:37:48 GMT  
		Size: 10.9 MB (10873345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:10a9ab63aa9560c05ac0a2f22711c5a2fdad626b235fe25eae6663c236526a7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75861061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05f20938dfd8d706e64e8181b9a84d9b2253bc16342e5b12fe7a124e0ed05543`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:12 GMT
ADD file:2cbda28d396a0fa4e6d85b7b6157b40a40e4cd783fb7e2182bfbe03c1ba23943 in / 
# Wed, 26 Jan 2022 01:46:19 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:36:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:36:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9ecf2845789585f183c7b423fece4a8a51e9f5753452de12292282be543e2500`  
		Last Modified: Wed, 26 Jan 2022 01:56:06 GMT  
		Size: 58.8 MB (58833543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d4b2a71bc242bb2c81b203b94ce8cd6c281117b4cdb6386dca34b051bdcb1f`  
		Last Modified: Wed, 26 Jan 2022 03:16:33 GMT  
		Size: 5.4 MB (5401513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8199fa873cada4fef014c20726ab130549bd9ba220f667be9c63d8fbabfacc80`  
		Last Modified: Wed, 26 Jan 2022 03:16:33 GMT  
		Size: 11.6 MB (11626005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6c5b99d6d79809fd49d2f8e331784a043f8af9c5b08c67893d8fd251f908775a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69108531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cceaee8f391ce67824a4d8283d5bb222d427afad83515a0d0356b1e57428a48a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:54 GMT
ADD file:0ff9360660b63a458b2c33e09a38fd9413847541680cd01bd4dc78cb14dd0f92 in / 
# Wed, 26 Jan 2022 01:40:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:08:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:08:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:19a0c65e73a647e498e4b74e1ce53ad5b58d75b2e52e2c30058143495b1148d5`  
		Last Modified: Wed, 26 Jan 2022 01:46:36 GMT  
		Size: 53.2 MB (53210407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c066ada395dfc3e4bf0f1f36ff1520571a6b86306adf89f67acfefca7d3c817d`  
		Last Modified: Wed, 26 Jan 2022 02:18:07 GMT  
		Size: 5.1 MB (5136535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca475bd1faac63fb98161ddab9d6899d6835750ab6291cddf7acecbb5a24997`  
		Last Modified: Wed, 26 Jan 2022 02:18:08 GMT  
		Size: 10.8 MB (10761589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
