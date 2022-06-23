## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:7f988ca1544dbe54f5db44a9b0e74f9ede3bcbe7da1c63b65358de2239b21e9a
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

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e29b1d0e636faaaab0d309b057b744605d424501fd3789917230f511c2a426ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131784236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d6b8717186a33e6b3db8fe42c54e93bdc3c94c440ac713b4f488ec60c85caf0`
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
# Thu, 23 Jun 2022 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:73e0035db86f2c4cb2e7be73d8634723047f8cca5c7260b8e2792b5d7a795402`  
		Last Modified: Thu, 23 Jun 2022 01:01:13 GMT  
		Size: 58.0 MB (58008546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3267a5f4342163a406898874527933d2a47040f1c9ed77e4b8e9ddfd4ce21e5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126311633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca754385cbba8dd34c4706df7000efb985151507d6d0fe293a4ba3e9fd03f607`
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
# Thu, 23 Jun 2022 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:23056815ddb644b67590d8378ba4910f8a02cbf63fec8dffc8e64a3fe5f1605b`  
		Last Modified: Thu, 23 Jun 2022 02:08:32 GMT  
		Size: 55.7 MB (55660019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f0c306b7e214d4f02d5b66ca26ad3fa883563678893109aae543ffede2087980
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121298032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:359ee98f448a75a647321f5a292d095517e0b633da45957764d554b779f8df53`
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
# Thu, 23 Jun 2022 01:55:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:0cb1f9d675028e4babe5d9856696abdc7cfa4b462b98ef48396f316fda0b620f`  
		Last Modified: Thu, 23 Jun 2022 02:19:25 GMT  
		Size: 53.6 MB (53585018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d3303a17c94ae966f4734754be9d2d091b2e55d9c0694e1b1a3a4fa36d1dda3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130453704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62edf6792cff0f27d834f133d7c23ca4b2901aa0a24290171c1800afc156d48`
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
# Thu, 23 Jun 2022 01:14:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:35bb12213e9f6fc3859b16595e8478ff8f3156869e99a0f9352d29da9911e50e`  
		Last Modified: Thu, 23 Jun 2022 01:24:36 GMT  
		Size: 58.0 MB (57991660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e1f1bc3f1310339b07caf890d9ea7cd0230c7380f848425153526681209a16d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134606360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6232b96a9f3559f92841699393871a63ec25303a3a10b4f7432e93377cb7aa7`
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
# Thu, 23 Jun 2022 01:15:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:553753d1d94d5a84b19b44ef5dd89152d8c95834466d6f78894d6f8d41a1c878`  
		Last Modified: Thu, 23 Jun 2022 01:25:05 GMT  
		Size: 59.5 MB (59495261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:449a0169809c35be36bb3a36d2ce6d52e19d083682ef815d43b7f1ef13eceb5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128614028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8afeb8a2e1b94e3e1a5fbfa5b2364f8c2dd33add5a5348b1cf8a48bcad17baf`
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
# Thu, 23 Jun 2022 02:11:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:0c6364d9f384bb225f74e3d8bf8e4a3192ed0f948fd01551882314335e40caa9`  
		Last Modified: Thu, 23 Jun 2022 02:27:18 GMT  
		Size: 56.6 MB (56634014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d214a6253973e331422ac82033ff47535c2b8fd5e4c8bc23b07143927157e37d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.1 MB (142131235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c2648b8a5deb29847d8e241bb03e6c05fe3e7b54f738b743d162d38886327c`
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
# Thu, 23 Jun 2022 04:37:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:0e496ab4ce171004942cb8ef21469520bc06b27da4ba9e5ca43224e9a82dc2b8`  
		Last Modified: Thu, 23 Jun 2022 04:59:31 GMT  
		Size: 62.8 MB (62768398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:a554d40bdf614dfd9e405a249dbfe2bff02cb93429ca042ff9db3c8e0b1c3124
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122419082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eef1028664b4597959820e5ea3724c58b7a5eff1763e4f7d9729c7729d13014`
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
# Thu, 23 Jun 2022 02:04:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:feebc8d66990654882c5fa423a1a4c713b77656fe3fb7540e4e51bbfcd8395d3`  
		Last Modified: Thu, 23 Jun 2022 02:54:14 GMT  
		Size: 53.9 MB (53944102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bfa48de8453399271b66e5612d28e4436b65b5983adca44a3c284719a6c9cecd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129148802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf096a0894e660e861779adbc9771c22a119a9e6af8f849b416789a64de559f8`
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
# Thu, 23 Jun 2022 01:26:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:d62041429a13a43bfbfd7d47a92db7f8c23e3aa09f835ed06612710629f88b9a`  
		Last Modified: Thu, 23 Jun 2022 01:37:10 GMT  
		Size: 57.3 MB (57299234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
