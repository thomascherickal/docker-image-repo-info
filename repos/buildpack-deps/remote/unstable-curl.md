## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:900a8aab0dccb61127a03916c4a1b17f3456963cd78afd95035e3d848b22760c
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e15b0ebf87528fc62a78ae3f06c442cc402577b56123248ff3aec845e5a67155
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74496044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebd36b9a38239c28cb251683fbcd556458ad6e99a6afa8d0d58d34fa9e5adc75`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:22:27 GMT
ADD file:bd8ad5ff1bfae3fed182d348486f9719820be43c8b6b13ad4385f6cc6a15ce87 in / 
# Thu, 07 Sep 2023 00:22:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:00:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:774563c7ab34b698df26f2291a44ab24b899f0da48b5794c4a9e51b889427e90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70346529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be2e6d9a14df3fc131f09bce7ad48cdbaba68d086d00efc976e7c7d409a7f17`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:44:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f883267a6e0fd23a7321e7809daf18ea9fde5af7d382347913aa6b73346ef73`  
		Last Modified: Wed, 16 Aug 2023 00:49:09 GMT  
		Size: 22.9 MB (22942748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f47f8706411e7685f82d48308aba1d5602ba2ccb172f9637917bf5b1c3f0e5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67846339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9dcb9b4c2955701a428ab7e6043efbb12f0286ab44fe433d7a7ccae9cde5ac6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:59:28 GMT
ADD file:48b9003b5f16cca577ade266eaa0f16a82c1470540f591ca5b3478846402f252 in / 
# Thu, 07 Sep 2023 00:59:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f357b484f94d65bee85830215f8a99bd873b9b6c588d9b18d73a660d1b7d230b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73342350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad8010747ba13453458120a56606c915f892703fb198850dde407010ab2ae49`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f5de6e756ae0263d5d8056bc2a6f2a8e87f5e28dde8b746fa6cb29bcd33513`  
		Last Modified: Wed, 16 Aug 2023 01:41:04 GMT  
		Size: 23.8 MB (23810620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d97b42d29a664dcae93cfd874db1be9d3c194cb92623f2447128c5bb0a572761
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75747069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ac27c3bf31307e25bfee6c4ee200ddeab2b6f606757de278d52f1d0566c9aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fb36009acd0e1d753239daf3a185a717a7e268ceb556a566bab97416024ee1`  
		Last Modified: Wed, 16 Aug 2023 00:38:32 GMT  
		Size: 25.1 MB (25115714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d1ddb20b6c6c4ebcb6f619d7b4e2503cce3bf074a79fea5a448ca6205752efce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73898559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d642cd22dab7865238e8f52fe0ef068190204e79158a4fd459db79e3c4b1ed7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:12:16 GMT
ADD file:a0f62fb4629026abfbc8955434580788fb6798315ec2cbb9fff3b490cae4ae5f in / 
# Thu, 07 Sep 2023 01:12:22 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:01:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dd603885105b996b2f2ac71bdbc6418f425ef338b8ccd9a0f89d91b542e774a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.5 MB (79495428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a1a539a3d7557346dd1bc8a2d6ee409a1be725c2e2443794e3c9a9de8a62ab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:11:08 GMT
ADD file:34567402b37eab48970f90189fd56c47e39acba6d260f0587409ca36a8d36458 in / 
# Wed, 16 Aug 2023 01:11:10 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:49:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0db36c7b4f2702f9e0075ee892fe4761e0f37f5cc9d73192725313c01591737`  
		Last Modified: Wed, 16 Aug 2023 01:18:29 GMT  
		Size: 53.6 MB (53551877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08327233d2cd5240264b2d14e300da4220731205ebdb79a082288235d814fe5f`  
		Last Modified: Wed, 16 Aug 2023 02:13:00 GMT  
		Size: 25.9 MB (25943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:463277650cb87ff963c4f3e246c78101c2bf595bfdcfda04fb4db350e9dc1592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69007846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46d4dea6048745e0f58711f73e97cfebd76971edb90fbbf0cf7dc14a24ec144`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:73e2126ec2291bed137d5f9c5330d0204753c6db3a7554483204c6114f0cccca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (73997872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50f42b1bae1cd7c8e757a17832da18ddc9ab1b268b5c893dfa8b0451bb329f40`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:45:36 GMT
ADD file:bd3fde5e3038704806827aa08d23e09a06b39ae915868b757132819f9c65e50e in / 
# Thu, 07 Sep 2023 00:45:43 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:13:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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
