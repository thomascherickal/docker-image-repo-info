## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:5d94cfe554e762305b0772aa4cb250c87ecd2d61ea0204a503cb39b58e7afcf6
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ae84357f52e576cb9c07edf3b2ed0fb638b3ca1e78a999a12785c8866fe1a8cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139172157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537338076e2cfd060cf0874ba2421016857e92b0caee307b8772729990c2dad5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:22:27 GMT
ADD file:bd8ad5ff1bfae3fed182d348486f9719820be43c8b6b13ad4385f6cc6a15ce87 in / 
# Thu, 07 Sep 2023 00:22:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:00:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c36f0cb17f99a82a25600b41f67d97eba8474b1cc58f325f0d1307303171b68`  
		Last Modified: Thu, 07 Sep 2023 00:28:36 GMT  
		Size: 49.5 MB (49492324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b764f7b6e030a499bf8ef09bc0ce09547c7bcbd95b0454538450c65a9adb1`  
		Last Modified: Thu, 07 Sep 2023 03:07:53 GMT  
		Size: 25.0 MB (25003720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0383dddb5ef2d2b7f853291557ef1e8af6166b53bfd59d8bfd946cbe3d236bb`  
		Last Modified: Thu, 07 Sep 2023 03:08:11 GMT  
		Size: 64.7 MB (64676113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d7cef4a472a5ca7a490a7ea040d084550a5e9952803328c7200b25737c46d7e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133111781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a5dec75b6ddffc03e63e4e031675d785a7ce0a9857d73ffd028d69f5e0e737`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:49:09 GMT
ADD file:65d133984adb1710a633ac35df6dab81e453734fdf5cabf6936e9a60011fc410 in / 
# Thu, 07 Sep 2023 00:49:10 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:19:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:20:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501694e1228126374bf3e18e7ce91920d16f560440d860976cd128b459e62654`  
		Last Modified: Thu, 07 Sep 2023 00:53:15 GMT  
		Size: 47.2 MB (47191094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf1e8fde0a23e63f1853d8dcb4c7a8585aa8b9c8391f01712b567ce1ea29f44`  
		Last Modified: Thu, 07 Sep 2023 06:26:59 GMT  
		Size: 23.6 MB (23645705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318d821d91da4851762eafb4cc38bfc7d350acc025b7a6e1000c9b77ff93d8e0`  
		Last Modified: Thu, 07 Sep 2023 06:27:19 GMT  
		Size: 62.3 MB (62274982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d1c5159a907ce955d1a542f88b087778e8a946270e284c7e472c75d282c97fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127733940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb4dc11f8b6a8d147e6635cbb5e17f8ddd240f89b8903662255229d9de89c6f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:59:28 GMT
ADD file:48b9003b5f16cca577ade266eaa0f16a82c1470540f591ca5b3478846402f252 in / 
# Thu, 07 Sep 2023 00:59:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d85f55a7a6c774695f75c1a7ec0bc0caeb915349d9250d2f4e6737e12fcc92fc`  
		Last Modified: Thu, 07 Sep 2023 01:05:21 GMT  
		Size: 45.0 MB (44983245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b914bb1a1428c8af17f4b5fe2002cd56706f2764ffe325bc5a8693a2d5885cd`  
		Last Modified: Thu, 07 Sep 2023 01:48:19 GMT  
		Size: 22.9 MB (22863094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cce762d527587259cc24735a7095b0706f16c46d1015868fffe9995eb694b6`  
		Last Modified: Thu, 07 Sep 2023 01:48:38 GMT  
		Size: 59.9 MB (59887601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c67fc501c2730dee6a8dc224578a0be26e7d4cf26c82c39305ab384669a20dff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138594998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cee1bd935201fcb863061005ba4e8adad960f8289d76427ace95073719e373`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:41 GMT
ADD file:3fad0766985d4815384b52dbb02c3f23c3f0c6e9b05ae96cdb2f60692ebe3c47 in / 
# Thu, 07 Sep 2023 00:40:42 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:55:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:55:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:352986db96f4040761867c771dd7419bd03916c5a2f552680219ad48902eec34`  
		Last Modified: Thu, 07 Sep 2023 00:45:36 GMT  
		Size: 49.4 MB (49413074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48ca0dfa7863c95cd7f5922e7ec0194090cd24c969b9936d768cd01354881a4`  
		Last Modified: Thu, 07 Sep 2023 07:01:59 GMT  
		Size: 24.5 MB (24531894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b08339dcbbaf894091d82da68954334103340d1d2952574feaeff7a2ffd4a`  
		Last Modified: Thu, 07 Sep 2023 07:02:16 GMT  
		Size: 64.7 MB (64650030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:61f1734eb7cc2dffcc102632dc09a5bf8eac4d56b528e6fef08623fee11dada6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.8 MB (142841779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a0a20c531aafa83ea40d559fdcadaf5013136e02231a348bc42f44d62956c19`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:40 GMT
ADD file:ff611322e6674f9fde9d60d146cd9f1206176a7ad0bffa135200bb5ce18ef6fb in / 
# Thu, 07 Sep 2023 00:40:41 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:32:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:33:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e341a6bda5bb8b3c55cc00b75f2a70088193c4ac06611dc91b32f6ca7c58df58`  
		Last Modified: Thu, 07 Sep 2023 00:47:07 GMT  
		Size: 50.5 MB (50501474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199c1deb7fa20bc9fa5f1c71efb48e77dbb9169e65a80ee76e1af76eb11ef7bb`  
		Last Modified: Thu, 07 Sep 2023 05:41:15 GMT  
		Size: 25.9 MB (25854651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bdb07681e939562c846b9666284e56c74395ac42f0c90225a11e7174a6a41e`  
		Last Modified: Thu, 07 Sep 2023 05:41:38 GMT  
		Size: 66.5 MB (66485654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2ed02c5afc812e283e49488df73a5333dad23564f7d501700cd380babb708be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137511760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a286e41e2b73000aba3e8f5b518f8ee3ff06d41f06e562199fc9cc02a96565c2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:12:16 GMT
ADD file:a0f62fb4629026abfbc8955434580788fb6798315ec2cbb9fff3b490cae4ae5f in / 
# Thu, 07 Sep 2023 01:12:22 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:01:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:03:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbf3aa413814601f6b34fe509eeee19b8570d10547318d9e50b786a1305da8f5`  
		Last Modified: Thu, 07 Sep 2023 01:23:38 GMT  
		Size: 49.3 MB (49337937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c57139e98311e15a5beb5188d286eb35893fd7b66379668ca38afc3c3926810`  
		Last Modified: Thu, 07 Sep 2023 04:26:24 GMT  
		Size: 24.6 MB (24560622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe5e62077ec632bacdfa13759bc11189801d913e3ad23d63f1a3c430854c2b`  
		Last Modified: Thu, 07 Sep 2023 04:27:16 GMT  
		Size: 63.6 MB (63613201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:03395b14cec765817b07515b2f3d51fec66ef4c69056c1538b1bec4dcbfc2752
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.2 MB (150248129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71570d594efc2de8ceadb692193649fa7c3c535a74b057a895ea21f64b68f0a8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:19:03 GMT
ADD file:0a03052b027b835521a56eb544f68d37afd082caf6b0f2a86d36ba3a4df23574 in / 
# Thu, 07 Sep 2023 00:19:07 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:32:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:33:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61513ad4f292fbcfceaab5e01ed63b82ba881a99736b2ffd97579f96947c0829`  
		Last Modified: Thu, 07 Sep 2023 00:25:38 GMT  
		Size: 53.4 MB (53429824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af30e0c1afcc76f65c4a2143f30e1403d1ff2bff1ecc5e0fee30d5f20906d81b`  
		Last Modified: Thu, 07 Sep 2023 09:46:15 GMT  
		Size: 26.7 MB (26685074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40404ef47fcfffb836201c5b1dd0e820e464c6b2a6a7467a3d61e3b2beb302d8`  
		Last Modified: Thu, 07 Sep 2023 09:46:43 GMT  
		Size: 70.1 MB (70133231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:06889be21e43bfdf203bbeae5d75d850689f386ee4790a6ed4857666dc24961d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138275015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49b4e5a393292328bea352b663f143396f7f5586d61d02bdee2d0315f4f474f2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:45:36 GMT
ADD file:bd3fde5e3038704806827aa08d23e09a06b39ae915868b757132819f9c65e50e in / 
# Thu, 07 Sep 2023 00:45:43 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:13:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:14:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee0f0030591cd1c61bb2bb7366cf7acef7874305f79e676bf8fcb8d10698613c`  
		Last Modified: Thu, 07 Sep 2023 00:50:52 GMT  
		Size: 48.7 MB (48730438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e552f7737ff7ce568b8ed95d29640fc89a141d02eb8ae1ff41a15b8e8305a3b`  
		Last Modified: Thu, 07 Sep 2023 01:23:57 GMT  
		Size: 25.3 MB (25267434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5438a4ee4569f4cfcd590fac3b9d0967f9e05e28ee9229c56cff8f039d32de`  
		Last Modified: Thu, 07 Sep 2023 01:24:13 GMT  
		Size: 64.3 MB (64277143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
