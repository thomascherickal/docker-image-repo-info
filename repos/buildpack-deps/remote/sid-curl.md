## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:1d1d24b26af5373e5f8346adb86a82a073d8d768fdbfb62695a0cbc831dddf1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e38fb05e1eef87bcd37a3118b0c9bb3747956a8c24dbfe06a99f0693d41de459
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73775690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2dd96006267b6359c2acfc0789dd3ae3832cbbbe7910df34b6266b9a24dc36a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:21:33 GMT
ADD file:5d253befef9729db59927d6e0d60fc3d68d46edea7e014babd24f72ac3a437bf in / 
# Thu, 23 Jun 2022 00:21:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:53:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:53:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d3673f28ea1768e72855620961143c989d7f371e6bca9954aea151e92c37b180`  
		Last Modified: Thu, 23 Jun 2022 00:28:29 GMT  
		Size: 53.2 MB (53218973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ae65eee62be843f104a65e140f50abf4d3ec55a20e85b9e3f7d2cfad04120d`  
		Last Modified: Thu, 23 Jun 2022 01:00:54 GMT  
		Size: 9.3 MB (9292311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6091239aaf7cc50884c05faa6c40bbdf0de0a133524daaebd95e5128d36a0d9`  
		Last Modified: Thu, 23 Jun 2022 01:00:54 GMT  
		Size: 11.3 MB (11264406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3b3e1495c31fede91e9d108090dd559e138e566299827170a3b1e4805f12c3db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70651614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db8b6ee333e70199e30af333161a6f705ff01646a496d92767f95c8b4f6f9728`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:53:55 GMT
ADD file:c61ce49a77125d8bfa37b1d68da44ffa2207297ef1a388f6cbc60c3581e05940 in / 
# Thu, 23 Jun 2022 00:53:56 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:46:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:46:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4751ad55e93558178cf9d1055ba3e38784464e7a3468902f0853aaa656dfea5a`  
		Last Modified: Thu, 23 Jun 2022 01:10:25 GMT  
		Size: 51.0 MB (50998383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071df38dc5479b6ed9928ecc1ab278de3e42b55e4c042bd9bbec823d6d0946dc`  
		Last Modified: Thu, 23 Jun 2022 02:07:40 GMT  
		Size: 8.7 MB (8725463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfbf2bfd1dacae3b057f098ed7f523109a7b91940d7ea487e11a9acd2a7ee2f`  
		Last Modified: Thu, 23 Jun 2022 02:07:41 GMT  
		Size: 10.9 MB (10927768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4c66d10d2d7da5aa68a29db4d78562becc926db2133c316bfca39c9782b286fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67713014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:431c791598b945c7599ba7b616b5f660bec9cf5b25aa3a940b61289dae7f25fb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:03:16 GMT
ADD file:51a321e16e02701a4130fcd4804ef7e14f5facfab8a82cdef3c2fd228a4ba034 in / 
# Thu, 23 Jun 2022 01:03:17 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:54:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:54:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2391a5c3a80e9c0555d4b398df748ee8be95db129c7c16e82cb7755d493118a7`  
		Last Modified: Thu, 23 Jun 2022 01:19:50 GMT  
		Size: 48.7 MB (48734709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d1193f1a87016b7e352fd620d9d5e616526a8c1d9ac8cad6c77aeb6559fd09`  
		Last Modified: Thu, 23 Jun 2022 02:18:45 GMT  
		Size: 8.4 MB (8405462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59543246561323586b73771e4cfd176cd7d73ca9c0e20cceba57a93111ba12c`  
		Last Modified: Thu, 23 Jun 2022 02:18:45 GMT  
		Size: 10.6 MB (10572843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:96774ff26a7db2ca54314dee1bb5b89bfc10d08b442925511ebdd1bf218f39f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72462044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23e70fdb72df113d53a796ccecb8cd32eb147e7e6bcbc5ae2b445bd938233935`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:42:04 GMT
ADD file:f08e8dd302c69f11b0631751a00fb9468d4bd358c6e3c34e364eae4601f0a325 in / 
# Thu, 23 Jun 2022 00:42:04 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:14:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:14:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:40490949eb8203de1427980faef5b6b648ec81967b0cb93ef80fb4a09d798555`  
		Last Modified: Thu, 23 Jun 2022 00:50:02 GMT  
		Size: 52.3 MB (52287486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1881ca7c4691be4824f0eddf333c4f2ab5f1ac743ee1c8c554a75da079933`  
		Last Modified: Thu, 23 Jun 2022 01:24:16 GMT  
		Size: 9.1 MB (9132621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8852bea5bd7a74a6867d8c61780e5bdaaad07e160db0bada549bc1b04e63e489`  
		Last Modified: Thu, 23 Jun 2022 01:24:16 GMT  
		Size: 11.0 MB (11041937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ffbcf2722ef04e82df0329e8c4a891c3cd9e6eb1a91910e955e91e3c81b784d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75111099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86852b4e5c4a5363fed719d25e53dc3df0d92192ebbb94112ed4952fbe449a49`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:59 GMT
ADD file:8e587a340c6b6c6dfa097954552e77cf8a794c99a1462d0c2062dd4f3b905687 in / 
# Thu, 23 Jun 2022 00:41:00 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:15:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:15:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:82252cde47e9fb82645e6353c13b39594115b4ab4b96e5a602245359036bb69f`  
		Last Modified: Thu, 23 Jun 2022 00:49:29 GMT  
		Size: 54.2 MB (54181034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a804107ac0ac6b959662ec593acb07f7f7900f2753d01cc321b3f498797ff54`  
		Last Modified: Thu, 23 Jun 2022 01:24:44 GMT  
		Size: 9.5 MB (9465816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3278139543c9edfb79cec19d272bb6af19642454308507ba2015c252c4b5462`  
		Last Modified: Thu, 23 Jun 2022 01:24:43 GMT  
		Size: 11.5 MB (11464249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0ff4a74532f3523ffb2e37cb870db09a06593b35773de23f95c05f5df910f311
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71980014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f332c9f7710c0dbcca7ca00fc8c1cfb9d05fa74b0d47e3a03e3a58125961dc52`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:13:03 GMT
ADD file:ee6af73e7954397e332676cdf91fcc81e58c7039ee0e6b28c76a45bbcd35f878 in / 
# Thu, 23 Jun 2022 01:13:08 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 02:08:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 02:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1122351c74d1f54ed8c97871bc43b5e9e533e877516d1335d49d0b35a135e12a`  
		Last Modified: Thu, 23 Jun 2022 01:23:42 GMT  
		Size: 52.3 MB (52302602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b60fb601ee8b9ce8fdf454454bc04959e78f2245d78fb79c1fd28d74c735fe`  
		Last Modified: Thu, 23 Jun 2022 02:26:28 GMT  
		Size: 8.7 MB (8657901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a790127ad374d0d7dce1e83718b6927775398eff00185730060dfa660ee1c63`  
		Last Modified: Thu, 23 Jun 2022 02:26:28 GMT  
		Size: 11.0 MB (11019511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:70bf422e9a395c4b0a8197af72fba614ef40e2d75ed0608a4fa349126c4d2725
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79362837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a08e778d8f74f1ee130c5b7e78d15d7e4fff1768e8b3753a91d0cfe2e9ab8946`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 02:04:45 GMT
ADD file:c9757ca75462d85dc4d76c948caf7c9441b1f94311712aed484424049dfa236b in / 
# Thu, 23 Jun 2022 02:04:55 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 04:36:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 04:36:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e03a908039ec9067867d0cfb4e2137913335e7055a4de7caa5a17b06fdcfc936`  
		Last Modified: Thu, 23 Jun 2022 02:21:32 GMT  
		Size: 57.4 MB (57413710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012e0f9d40f6756a17c2a26c1540b57aef08309d861a58ee201ce546d8e16f89`  
		Last Modified: Thu, 23 Jun 2022 04:59:07 GMT  
		Size: 9.9 MB (9883975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26df9fd6cda08db21eda8015d4fac544f2e705c64a73aa93ac154c59b04ee95f`  
		Last Modified: Thu, 23 Jun 2022 04:59:07 GMT  
		Size: 12.1 MB (12065152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:bca1278dba382365d874812a9dbb88a443ec4d0c56f0892f79848db86ee8ec39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68474980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd7ea6e17b02b63be4ed898e0bb4b4a4237105ebc5126d9242a18d1d83beef87`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 01:11:50 GMT
ADD file:e156d172727c94dd7b17970577469d9b556db67960762f454d5b90dad3f746bb in / 
# Thu, 23 Jun 2022 01:11:53 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:58:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:59:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:70334332338a08f7ae515b43812936d5898e62e8ffd5fd38ba59761c5ed137d9`  
		Last Modified: Thu, 23 Jun 2022 01:30:12 GMT  
		Size: 49.4 MB (49429796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5fc26886e551b626bc82f99096f4659ee9ee5af689dad0d03fc75d88c37d88`  
		Last Modified: Thu, 23 Jun 2022 02:51:42 GMT  
		Size: 8.4 MB (8394795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6176147b43ca0f721514815cbe526cd0e19723ed30c23a9a3534a95d32d19cb`  
		Last Modified: Thu, 23 Jun 2022 02:51:43 GMT  
		Size: 10.7 MB (10650389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3b764dc50580bcd9788ad5266451e748d89f5dc26e741ff80a26bf4ebdb6b178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71849568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6fa28fd0e10954ecb957978d57304f527dff67b09f15d3bdfee00c27ed7fa95`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:45:16 GMT
ADD file:ab375e0cb8f5b6409d63f919593d858353b72a1583cd317ab360dfe14ea03d6f in / 
# Thu, 23 Jun 2022 00:45:24 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:25:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:25:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a8cf7e6e484c650a0d73e79e1cb371750be4da7ee1f80e6f2269ce876a0da394`  
		Last Modified: Thu, 23 Jun 2022 00:53:20 GMT  
		Size: 51.8 MB (51752635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f7c9785fe37d8cf623f10d952220284ffb99daa61aee3f8346d128877bcd24`  
		Last Modified: Thu, 23 Jun 2022 01:36:54 GMT  
		Size: 8.9 MB (8939375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282f27bfdfd818dfca8564ec63da5207a70fc4c2e78f1f0c5fe96ff585343b31`  
		Last Modified: Thu, 23 Jun 2022 01:36:53 GMT  
		Size: 11.2 MB (11157558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
