## `buildpack-deps:trixie-curl`

```console
$ docker pull buildpack-deps@sha256:4f7864852534ba0243ffe4e2b75e1f8d7b1bb11be078397d78618535eda8054a
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

### `buildpack-deps:trixie-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0a83183f7c37c53a706b095ca3f476a1c685cdfae41ad49667eaa6453d3ac3fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69812643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c6248e338704ed0103a72cedf26cec4ec90af9944acd6776e9c5dfd2d07a31e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fc83c09b27b5464dc8ea8a5446245ac976b0539327658f64cf6f92fb6bcd3f`  
		Last Modified: Wed, 01 Nov 2023 01:06:11 GMT  
		Size: 20.3 MB (20325758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:031cbfec3788de366368b6700cf07f976ca32f81b5388f71e97a642ceaf17d99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66536022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfeb4d63e6a42cebf132eda2fade400016c56515b7ccc382acb28f0ffaf96207`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:06 GMT
ADD file:a7de42b73a4591d75c2ea2f44cdd15d34ce24fa78ca8e57ac62e4fd3ffe2019d in / 
# Wed, 11 Oct 2023 17:39:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a100e11229dc40f9cdcd25e779cd1f10bb500c44c5b9ae24abec0b01f4b26b1`  
		Last Modified: Wed, 11 Oct 2023 17:44:09 GMT  
		Size: 47.2 MB (47166046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f41504078ef3db4155843c88e3eb49d76721ce77692685bb502799200ff810`  
		Last Modified: Wed, 11 Oct 2023 18:18:08 GMT  
		Size: 19.4 MB (19369976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0341d48d95c3e5a4d2c5a756bf9c02be5ac68c3f91d4d25430cb7e2b39f87798
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63592453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec3154dd1baa055cc85e3cde172b24a55a63577750ffcf2919f520810dfa4bc8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:26 GMT
ADD file:69ac67070b211f2a7980ec82da00c1d97d41dc6fe979f892e741ce9b7c566a85 in / 
# Wed, 11 Oct 2023 17:44:26 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53634a2dc8fdfb2e0bde3647302a9fd6183101ae18e9a9c89ec4d54909761e25`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 45.0 MB (44954093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2152d48e2ff44fb8710e1613ee9c264a844d0354cce2b66cb656364b0908e2`  
		Last Modified: Thu, 12 Oct 2023 04:00:35 GMT  
		Size: 18.6 MB (18638360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9fbda31bfbc609c550daf14bef5f22d3f176104c0821d8ddfe4582837d5a85ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69615576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0b60c14a1ee8b098f27d569ee70427ec60d1436140bb21e61e1e3ce0735f75`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:26:37 GMT
ADD file:ae967b7faba93d8a00f97f28b4d720835a90a27fe53b2f278072893f4cdaa8e7 in / 
# Wed, 11 Oct 2023 18:26:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:51:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddf19dd473b427de200cf2b123540cd1dce2dcb51aeeb4a1359b7f954dc951ba`  
		Last Modified: Wed, 11 Oct 2023 18:32:45 GMT  
		Size: 49.5 MB (49505530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3234e169293a5a7c5d4630e4d414fffc649556678901730a692ba3b43cd5e618`  
		Last Modified: Wed, 11 Oct 2023 19:57:45 GMT  
		Size: 20.1 MB (20110046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:805dd0cb6d20f9293082e2731dee26c4189ba2e05e33a9f191a996164477f318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71372123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b67991ebfd3a67bfb234e83a7242703653494aeefd5471beb24c4e239b52a8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:20 GMT
ADD file:ad97acda5f74778001aece2a9e280f0e58d2953cf8fdbd4740a049c4a595a225 in / 
# Wed, 11 Oct 2023 17:43:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce8ed34eaeffdeb7ac49225c6093f421b0005558aedb2b9c429731032d156621`  
		Last Modified: Wed, 11 Oct 2023 17:50:59 GMT  
		Size: 50.5 MB (50485846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94c813421107d5ab710ec3329c2cd90f1b42da6b64e3d4ea8428fc7802b293`  
		Last Modified: Wed, 11 Oct 2023 18:27:57 GMT  
		Size: 20.9 MB (20886277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2f51f1238b9640b9e5ee718926672d0df20e00b0acbf2c2b311248148673bbc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68895374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db4384cd0f6fbbde63af84a9a7aba48e7ca88a8045c743733eb4c43414eed70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:56:15 GMT
ADD file:29bed270e296c5a95f2141f114580e0f25c1040c03609fa632757a8e48ec43fd in / 
# Wed, 11 Oct 2023 17:56:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0d54eafe706e7144ea10a18a0abaa975cb4f7f92fd40e292f388c2b1321a794`  
		Last Modified: Wed, 11 Oct 2023 18:07:41 GMT  
		Size: 49.3 MB (49301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5204f5199336e47ca287487c83b254ad7b0260c5bf568e92c8927077786ee91c`  
		Last Modified: Thu, 12 Oct 2023 00:05:30 GMT  
		Size: 19.6 MB (19593645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:591e2f9c3b9c350ed8dba9ca0614e4c7b44b3610c178f9e4448c57ad5e3133b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75062217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdae9eab9b095c3c61aa347d6635f9ce2117099144c8bea9931d276e481f2711`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:47:23 GMT
ADD file:24d4df221ce118a8059e0559a8bb2d715512fa6f5b15cd1397dbc177ceaa1bfd in / 
# Wed, 11 Oct 2023 17:47:26 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93b578febbe769059c90eaa91e9dc027d172e6088856c2c52dc3e26dfdf01d4c`  
		Last Modified: Wed, 11 Oct 2023 17:54:24 GMT  
		Size: 53.4 MB (53418134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576f9c6569231cdc2bf492ed27ab8c980261301252c26c4d6fcf8dec4fa4de9b`  
		Last Modified: Wed, 11 Oct 2023 18:41:22 GMT  
		Size: 21.6 MB (21644083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dce98873fc650b5ee64351ca6ac11454fe20bca0ec37aeca46e3f5eaebabcafd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68965809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3887383a692e4e80043fe7ea299b03d5845a16f8d443c12d78177cdea73045e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:11 GMT
ADD file:7f7d0fe596110ed400f2bbc2fe6edf5716a5a62332062c86009df0df0cc0a257 in / 
# Wed, 11 Oct 2023 17:53:14 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f47ccc9a5d62eac06dcd9bcbdf51b3bf5f494156a2c21d58d93d11f5261baf4`  
		Last Modified: Wed, 11 Oct 2023 18:01:45 GMT  
		Size: 48.9 MB (48924346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659ce526b11a7e72319632cba55fb2631fe06f2d042501bcb6fd357be98825e4`  
		Last Modified: Thu, 12 Oct 2023 00:38:24 GMT  
		Size: 20.0 MB (20041463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
