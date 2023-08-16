## `debian:trixie-backports`

```console
$ docker pull debian@sha256:c9c5b4426762cc7fd8eeef41eedeb2240c983963e1b2d47cf7de7efd418f2fd4
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

### `debian:trixie-backports` - linux; amd64

```console
$ docker pull debian@sha256:3168b88d2ef04836496da2e0f613077e94f15291f4f5340252c1b071e8749809
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49596909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab6b25e68689f589f9cdba17adf743b7131484e9daae056b569825bac3d8753`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:27:28 GMT
ADD file:8c4b165f14bf36d9d8615d86e330e2619791a9af4f7c82ed8489717ca4584aab in / 
# Thu, 27 Jul 2023 23:27:29 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:27:33 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c96befece94d6ccacf8c06c689180a6d127f115525a8914bcc579f9d88d893cb`  
		Last Modified: Thu, 27 Jul 2023 23:33:49 GMT  
		Size: 49.6 MB (49596684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51808ad42a6e4d118a4a9b1959c17a9756ca7115b1cc7d5bdec7e01b4fc4f530`  
		Last Modified: Thu, 27 Jul 2023 23:33:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:629317e1f5b90fadb1fb92a23a209f22e7c40dc97e29b18b016d279ccf28b40d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47395349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f67327679440f0036887b5d460b6838f89e8581f17c7afa8b01578a922c8def`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:56 GMT
ADD file:d0da838ea8ff64a44e445dfb0001a4f6a2442085f0c0f942d0129b6f8054c7fa in / 
# Tue, 15 Aug 2023 23:49:56 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:49:59 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e6d8f24fa9802404161e1d0ef0d1db6d5f4c20cb1f0e5884dd191e1d77f2373c`  
		Last Modified: Tue, 15 Aug 2023 23:54:43 GMT  
		Size: 47.4 MB (47395127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595fc3b761ab0750256a3059eb3a81984b876b3d315e76592af11a4b592c5640`  
		Last Modified: Tue, 15 Aug 2023 23:54:52 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:15cd142db2228ac36dc64d7aef39daf015ea0ec8b17b822716c1600f482fe23d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45212485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8da9097ddd964572ed429bb0de17e1b182ba077acea0689b1aa2cce93119c2a3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 28 Jul 2023 00:01:07 GMT
ADD file:e750a7c315188d832ff98e8e33a2e78c68efa5a12bb17c8f873d0b5644bfc544 in / 
# Fri, 28 Jul 2023 00:01:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:01:10 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6aa08574e3d848ebe16f5911815377a151ed265e55191125c00acdc60a10c7d7`  
		Last Modified: Fri, 28 Jul 2023 00:07:46 GMT  
		Size: 45.2 MB (45212257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b88498dfaecd471ee638a2d95c6dcf20f03143a0e6c209dbf9032a663c2cb7`  
		Last Modified: Fri, 28 Jul 2023 00:07:55 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c27b6c2a1965658833ec27edc0d3401202f109503eb1c81ce92a8f49a45f48f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49522202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d781dfed58f60b08e68e76fe17ec9922b573125dfddf4a7b53cebac07613559e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:42 GMT
ADD file:16621389c05de9ece6b8d40e6c62ca81465940296cc58f7f1c56571fac05b33e in / 
# Tue, 15 Aug 2023 23:41:43 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:41:45 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c5fc9f67522f8eb1fc65844ccc91e1d93595f85d410842d334c85f7e0a15d841`  
		Last Modified: Tue, 15 Aug 2023 23:47:22 GMT  
		Size: 49.5 MB (49521978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cf68cfe6022db91f0314621a18fe9ff3f478f6830df4e9bc27b45115d85891`  
		Last Modified: Tue, 15 Aug 2023 23:47:30 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; 386

```console
$ docker pull debian@sha256:d7aa4808a28c9c7ab4265dd27868b589ce9db8b65b8791f6e012d880765d72d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50618757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c001c00d8feb25926c94108161d32246aa67965e488752513f7f988d7a5af228`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:32 GMT
ADD file:4d14eb57255656e664c93bdd44713aab3556f53199d3002e8b099b8a4f99ee66 in / 
# Tue, 15 Aug 2023 23:41:33 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:41:35 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:92cb61533d6d73bc90b946ae69c5db6942d13512056cb4f565d14697cd7aa909`  
		Last Modified: Tue, 15 Aug 2023 23:48:22 GMT  
		Size: 50.6 MB (50618535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cb415975c46926f754f627525c5e557c0e3cb8667d931f9d29e549ca6f0540`  
		Last Modified: Tue, 15 Aug 2023 23:48:31 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; mips64le

```console
$ docker pull debian@sha256:6740522cc63cf9b024abf7076c74ebd311460a98abe2a7b8b1825cfc0e599294
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49544684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44faf8e5a10b39b992ec9436644ad71b09e84a56dfc7afc71ba6ffd254b1019b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:18:05 GMT
ADD file:dbad549f8e200f8f213a4e285bdfb551b16bfe40fb4f82e748ea3bda17afef8d in / 
# Thu, 27 Jul 2023 23:18:11 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:18:23 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:39f64a8ea6c4a8a8f170704f90e994bdc1c77dadd700a514aba55a887f406f57`  
		Last Modified: Thu, 27 Jul 2023 23:29:29 GMT  
		Size: 49.5 MB (49544459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aaa91b9eda6fc7f20c5d2a05db12085ce7bd4ea254771b8a2151aef6cd0738`  
		Last Modified: Thu, 27 Jul 2023 23:29:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:11fb93c4e082b3c3b5946fd9199ef067716b5556c36ab9ff16128e21766e6ce5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53583406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a945e51c9617a397ae0be4f81870d5ee7a2692e6e4be1afe1467328a2202b1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:20 GMT
ADD file:cf2133276d37e9779bd1b7d4236ac343e5eed1d08f1cbdf946c8b89663de5d2c in / 
# Thu, 27 Jul 2023 23:26:23 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:26:28 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:658eb606329d6eacf175892b5aea3b47f025ce1b0299283b73efe3ae9409fa14`  
		Last Modified: Thu, 27 Jul 2023 23:34:27 GMT  
		Size: 53.6 MB (53583179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c605497e77247002a358a9277fdbc7b9adb40652931f00d791aabb426609950`  
		Last Modified: Thu, 27 Jul 2023 23:34:40 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; s390x

```console
$ docker pull debian@sha256:ee76d8178ddfb5eca74c7971a0c36146a98b06d22671259da3db82e0bd826374
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48540033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738b5c61b570b03f4404f6bc446db1cb3a56a48546e80058d531356a1b21d721`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:45:32 GMT
ADD file:d99fe1ff201690fcb871123822de04002451af1e06ae75e1a18fd80ef531de86 in / 
# Tue, 15 Aug 2023 23:45:38 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:45:43 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:73c53ccb564b87caad8f214df94d16496ce4754e4b20ee558b3c8f3ac938e41a`  
		Last Modified: Tue, 15 Aug 2023 23:50:14 GMT  
		Size: 48.5 MB (48539809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd900779cc19e5cd930fab5f49a837be66dbdb8d98eaf247522a3ffb039e622`  
		Last Modified: Tue, 15 Aug 2023 23:50:21 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
