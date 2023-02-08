<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `fedora`

-	[`fedora:36`](#fedora36)
-	[`fedora:37`](#fedora37)
-	[`fedora:38`](#fedora38)
-	[`fedora:latest`](#fedoralatest)
-	[`fedora:rawhide`](#fedorarawhide)

## `fedora:36`

```console
$ docker pull fedora@sha256:17ab257e353f7e0247ce4b1a6ac7a4dd372cf217e532f27d67feb876a53af471
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:36` - linux; amd64

```console
$ docker pull fedora@sha256:c82170503f2bdada53d529edbbb883cb8432a37f037a15491d2fb4d67d9c1a9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (60030410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e68c6a5f825ebd513d810702ab00cf4a800962495b00473cebd5d4eab42f5ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 10:46:00 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Mon, 12 Dec 2022 20:30:05 GMT
ADD file:f5c78ed041f4a21587bde12afd55c548dbf305c037474ba441e7db1f3b4f993c in / 
# Mon, 12 Dec 2022 20:30:06 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c13ad3937d9103327c4b061cc7e2ce6c8f6c0958c24eaddf0afde5a0114df4d7`  
		Last Modified: Mon, 12 Dec 2022 20:31:05 GMT  
		Size: 60.0 MB (60030410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:36` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:2cbc55fe048741ba72410e74c86e78bd7d3e2fc3f39e0de9c9ecfe0f74e2e7b8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58109409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f04f301acc316b3857f8f1111a4b59f5e3df7cdf7db9b867ea079a9d0a92c7d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:22 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Mon, 12 Dec 2022 20:40:55 GMT
ADD file:25227f4ea55a7ce1fad54f00d8549d9f4f52d45a0adcd1480b42512cf92ffac8 in / 
# Mon, 12 Dec 2022 20:40:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:88e4f16cd8916547add1dcf1c000a62ec73cd49b4de6392a9425bffcd79f1ed5`  
		Last Modified: Mon, 12 Dec 2022 20:41:49 GMT  
		Size: 58.1 MB (58109409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:36` - linux; ppc64le

```console
$ docker pull fedora@sha256:b5feb613afcc5797a769df28f54e4a77018366fcc389b08f3d92454731460fa4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65451966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e09305483c83beb6c29b29f23b105d4e6dcc373db2a767a48d83b2093e10592`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 11 Oct 2022 12:17:27 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Mon, 12 Dec 2022 20:21:18 GMT
ADD file:9273cd71f145243373170320c9835b1f94b6892419b23d26333befd23f39c773 in / 
# Mon, 12 Dec 2022 20:21:22 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:41acefe4f9db1c91cd40b42bde05d7b730c518e766fb5b019ff38cd139080897`  
		Last Modified: Mon, 12 Dec 2022 20:23:21 GMT  
		Size: 65.5 MB (65451966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:36` - linux; s390x

```console
$ docker pull fedora@sha256:4b85fd20a7ae71bd646a8b991ba580feb764f136d67c714f53a77ccd9250659c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (57007109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba5dfca5f087ef4fef620ffc49850202fad225fb418fdec78aed1bedb6754ea5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 04:31:33 GMT
ENV DISTTAG=f36container FGC=f36 FBR=f36
# Mon, 12 Dec 2022 20:42:52 GMT
ADD file:d2c6b81b4ef7a85b7a04a3e7e0dbfbbd30ba07691e0a0978f5547a33448dd558 in / 
# Mon, 12 Dec 2022 20:42:59 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ae0977f45148340713b798f63bc95e0d47655130510c55ffee457dc884b50a1c`  
		Last Modified: Mon, 12 Dec 2022 20:44:30 GMT  
		Size: 57.0 MB (57007109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:37`

```console
$ docker pull fedora@sha256:3487c98481d1bba7e769cf7bcecd6343c2d383fdd6bed34ec541b6b23ef07664
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:37` - linux; amd64

```console
$ docker pull fedora@sha256:99aa8919afd1880064ec915dba44cdc5b52808667717f605750329d55006538a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66089720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95b7a2603d3aa3135d58410efdf7f020ab28f0286ee56724a7a774d48a5c08bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 10:46:14 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 12 Dec 2022 20:30:17 GMT
ADD file:f2b3208c015da1e15b276f742a84b540238210afc4f92ab5d1e561fadcc2f2b8 in / 
# Mon, 12 Dec 2022 20:30:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd974119263e78652ccbbd00decd88e307abef723a1ccf622fc9d6c0baf58bb2`  
		Last Modified: Mon, 12 Dec 2022 20:31:21 GMT  
		Size: 66.1 MB (66089720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:37` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:c79287c2216a5e4597b8f2495b7c95ebe49d58f225cb1d254a34c0798647d6a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64277683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:191f4272c9599b43c04cf6bb9f2dff1e36b139c2567b06a9f1f53efde55d57d4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:31 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 12 Dec 2022 20:41:03 GMT
ADD file:1dfc04bc317cf79be2d36db1c828953f6a02ea24a3e2b9b8a5b226bb5d72638c in / 
# Mon, 12 Dec 2022 20:41:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:030a67402fc8bf84745e5de2ec579b0a324b0047a58f18eb2cb602ed0a9eacde`  
		Last Modified: Mon, 12 Dec 2022 20:42:03 GMT  
		Size: 64.3 MB (64277683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:37` - linux; ppc64le

```console
$ docker pull fedora@sha256:32dd8c2ccde8d9a99139c62f46da08530825497899b54ac839531566b8ef4545
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71792440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d11e7cc3a41e6cf4f9fd4a44eba2e3d013630b0ba493677d1b8118a5f3dccdd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 11 Oct 2022 12:17:51 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 12 Dec 2022 20:21:43 GMT
ADD file:185d47007b3035e3bdbd2bc0c29331bf10a3e2a68d58dd6338ac9433a9558617 in / 
# Mon, 12 Dec 2022 20:21:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cc547607d96a15f100f968d797e5004fcb7b32369d053da6b750c68cbc2a43c7`  
		Last Modified: Mon, 12 Dec 2022 20:23:47 GMT  
		Size: 71.8 MB (71792440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:37` - linux; s390x

```console
$ docker pull fedora@sha256:22940f57917d5225c894e44a4aa529e9dee7ac60f97150a272744dfdb444acaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63240068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf8678bba3999bec3ddd059774fb395e84260b2b162597ac2bdf7fb5d67a4e8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 04:31:50 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 12 Dec 2022 20:43:14 GMT
ADD file:4fe96c025aa3784afee14e6a1a96e880d708ca1cae2101c2d2ee76e46459f0e8 in / 
# Mon, 12 Dec 2022 20:43:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:531e70c1dbf9dbe2d42d80b906316194070e428456f111bae7b11fed2e57208e`  
		Last Modified: Mon, 12 Dec 2022 20:44:43 GMT  
		Size: 63.2 MB (63240068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:38`

```console
$ docker pull fedora@sha256:66e2c0e498c3981483157b1f45ceade507bd7bc006c4609f71ab17a99aa0240d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:38` - linux; amd64

```console
$ docker pull fedora@sha256:ed0bafb5fc0ef5128ebe28c3d4bfbab2770913afd791d1f5b413d7b20b586ff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0351297d3b545bc05375ed0840922dcec05689cbc1f62a93e6f8e567b23c72d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 20:41:02 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Mon, 12 Dec 2022 20:30:28 GMT
ADD file:12caea7acf1386183d21f9953f0fb83a25a03bce7ed95f61d1b191e4620ef74b in / 
# Mon, 12 Dec 2022 20:30:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:44bfedb596e53987608e6059b456b8b768958ed274494eed38424d8baaf369b5`  
		Last Modified: Mon, 12 Dec 2022 20:31:39 GMT  
		Size: 66.7 MB (66653473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:38` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:434d0b35e4984997427e4276cd0e30ffbf38e1bae4313aaa3e1f4c5bcab4a54e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65014649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b76c6eef85f03d9bbdd2697ce5618fd88e349dfcc5db98d20091eceacc213952`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:41 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Mon, 12 Dec 2022 20:41:11 GMT
ADD file:a9c578bc16857ca505e7e0da7fe48ad83f2647f8323c89727b09814afc9a0d89 in / 
# Mon, 12 Dec 2022 20:41:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:05549b64f51a5e58cabf063b0a71db77eaa36a5f92189ffd466aee8a6f449c44`  
		Last Modified: Mon, 12 Dec 2022 20:42:19 GMT  
		Size: 65.0 MB (65014649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:38` - linux; ppc64le

```console
$ docker pull fedora@sha256:341ab7e099ac74b82aa486f88d77bd9205ec5d177d4b31c50f59510434976550
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73145146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef33ede04de4ab9786ad6aca9f402f1fe524608dc08540b5ef1ed0848994d83`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:19:02 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Mon, 12 Dec 2022 20:22:09 GMT
ADD file:0839850f991d073ae80b34dcb3413028fdc2c403bf8770798539b1d41965cd4d in / 
# Mon, 12 Dec 2022 20:22:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:590fab9de796fd021f74e1039449b2ade4966198a27f5780f31bb8fb03b56489`  
		Last Modified: Mon, 12 Dec 2022 20:24:18 GMT  
		Size: 73.1 MB (73145146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:38` - linux; s390x

```console
$ docker pull fedora@sha256:f4688211b4ec002889c26bab47e27b8925efe5cd48b757e40f7c51194b9c565b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64492212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457f2ad30c63c591f49cfca7d9a9f9f2926f9bee13b43f9e8a47ee5d8f733ae3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:31:13 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Mon, 12 Dec 2022 20:43:36 GMT
ADD file:4b07bae1c2870958d906b51fee56f4d3fdc8d0932f8bdf007bcf0531b6ac3095 in / 
# Mon, 12 Dec 2022 20:43:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:51a2a7647f8363ce6e5a9502afe51c4e9651ab6aea92958531d1116b3dc9dcf1`  
		Last Modified: Mon, 12 Dec 2022 20:44:58 GMT  
		Size: 64.5 MB (64492212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:latest`

```console
$ docker pull fedora@sha256:3487c98481d1bba7e769cf7bcecd6343c2d383fdd6bed34ec541b6b23ef07664
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:latest` - linux; amd64

```console
$ docker pull fedora@sha256:99aa8919afd1880064ec915dba44cdc5b52808667717f605750329d55006538a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66089720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95b7a2603d3aa3135d58410efdf7f020ab28f0286ee56724a7a774d48a5c08bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sun, 20 Mar 2022 10:46:14 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 12 Dec 2022 20:30:17 GMT
ADD file:f2b3208c015da1e15b276f742a84b540238210afc4f92ab5d1e561fadcc2f2b8 in / 
# Mon, 12 Dec 2022 20:30:17 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cd974119263e78652ccbbd00decd88e307abef723a1ccf622fc9d6c0baf58bb2`  
		Last Modified: Mon, 12 Dec 2022 20:31:21 GMT  
		Size: 66.1 MB (66089720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:c79287c2216a5e4597b8f2495b7c95ebe49d58f225cb1d254a34c0798647d6a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64277683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:191f4272c9599b43c04cf6bb9f2dff1e36b139c2567b06a9f1f53efde55d57d4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:31 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 12 Dec 2022 20:41:03 GMT
ADD file:1dfc04bc317cf79be2d36db1c828953f6a02ea24a3e2b9b8a5b226bb5d72638c in / 
# Mon, 12 Dec 2022 20:41:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:030a67402fc8bf84745e5de2ec579b0a324b0047a58f18eb2cb602ed0a9eacde`  
		Last Modified: Mon, 12 Dec 2022 20:42:03 GMT  
		Size: 64.3 MB (64277683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; ppc64le

```console
$ docker pull fedora@sha256:32dd8c2ccde8d9a99139c62f46da08530825497899b54ac839531566b8ef4545
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.8 MB (71792440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d11e7cc3a41e6cf4f9fd4a44eba2e3d013630b0ba493677d1b8118a5f3dccdd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Tue, 11 Oct 2022 12:17:51 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 12 Dec 2022 20:21:43 GMT
ADD file:185d47007b3035e3bdbd2bc0c29331bf10a3e2a68d58dd6338ac9433a9558617 in / 
# Mon, 12 Dec 2022 20:21:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:cc547607d96a15f100f968d797e5004fcb7b32369d053da6b750c68cbc2a43c7`  
		Last Modified: Mon, 12 Dec 2022 20:23:47 GMT  
		Size: 71.8 MB (71792440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:latest` - linux; s390x

```console
$ docker pull fedora@sha256:22940f57917d5225c894e44a4aa529e9dee7ac60f97150a272744dfdb444acaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63240068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf8678bba3999bec3ddd059774fb395e84260b2b162597ac2bdf7fb5d67a4e8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Sat, 19 Mar 2022 04:31:50 GMT
ENV DISTTAG=f37container FGC=f37 FBR=f37
# Mon, 12 Dec 2022 20:43:14 GMT
ADD file:4fe96c025aa3784afee14e6a1a96e880d708ca1cae2101c2d2ee76e46459f0e8 in / 
# Mon, 12 Dec 2022 20:43:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:531e70c1dbf9dbe2d42d80b906316194070e428456f111bae7b11fed2e57208e`  
		Last Modified: Mon, 12 Dec 2022 20:44:43 GMT  
		Size: 63.2 MB (63240068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `fedora:rawhide`

```console
$ docker pull fedora@sha256:66e2c0e498c3981483157b1f45ceade507bd7bc006c4609f71ab17a99aa0240d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `fedora:rawhide` - linux; amd64

```console
$ docker pull fedora@sha256:ed0bafb5fc0ef5128ebe28c3d4bfbab2770913afd791d1f5b413d7b20b586ff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66653473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0351297d3b545bc05375ed0840922dcec05689cbc1f62a93e6f8e567b23c72d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 01 Apr 2021 17:59:37 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 20:41:02 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Mon, 12 Dec 2022 20:30:28 GMT
ADD file:12caea7acf1386183d21f9953f0fb83a25a03bce7ed95f61d1b191e4620ef74b in / 
# Mon, 12 Dec 2022 20:30:29 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:44bfedb596e53987608e6059b456b8b768958ed274494eed38424d8baaf369b5`  
		Last Modified: Mon, 12 Dec 2022 20:31:39 GMT  
		Size: 66.7 MB (66653473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; arm64 variant v8

```console
$ docker pull fedora@sha256:434d0b35e4984997427e4276cd0e30ffbf38e1bae4313aaa3e1f4c5bcab4a54e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65014649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b76c6eef85f03d9bbdd2697ce5618fd88e349dfcc5db98d20091eceacc213952`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 03 Nov 2022 19:58:13 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 19:58:41 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Mon, 12 Dec 2022 20:41:11 GMT
ADD file:a9c578bc16857ca505e7e0da7fe48ad83f2647f8323c89727b09814afc9a0d89 in / 
# Mon, 12 Dec 2022 20:41:12 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:05549b64f51a5e58cabf063b0a71db77eaa36a5f92189ffd466aee8a6f449c44`  
		Last Modified: Mon, 12 Dec 2022 20:42:19 GMT  
		Size: 65.0 MB (65014649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; ppc64le

```console
$ docker pull fedora@sha256:341ab7e099ac74b82aa486f88d77bd9205ec5d177d4b31c50f59510434976550
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73145146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef33ede04de4ab9786ad6aca9f402f1fe524608dc08540b5ef1ed0848994d83`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 11 Oct 2022 12:16:45 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:19:02 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Mon, 12 Dec 2022 20:22:09 GMT
ADD file:0839850f991d073ae80b34dcb3413028fdc2c403bf8770798539b1d41965cd4d in / 
# Mon, 12 Dec 2022 20:22:14 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:590fab9de796fd021f74e1039449b2ade4966198a27f5780f31bb8fb03b56489`  
		Last Modified: Mon, 12 Dec 2022 20:24:18 GMT  
		Size: 73.1 MB (73145146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `fedora:rawhide` - linux; s390x

```console
$ docker pull fedora@sha256:f4688211b4ec002889c26bab47e27b8925efe5cd48b757e40f7c51194b9c565b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64492212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457f2ad30c63c591f49cfca7d9a9f9f2926f9bee13b43f9e8a47ee5d8f733ae3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 23 Jul 2021 02:30:24 GMT
LABEL maintainer=Clement Verna <cverna@fedoraproject.org>
# Thu, 03 Nov 2022 21:31:13 GMT
ENV DISTTAG=f38container FGC=f38 FBR=f38
# Mon, 12 Dec 2022 20:43:36 GMT
ADD file:4b07bae1c2870958d906b51fee56f4d3fdc8d0932f8bdf007bcf0531b6ac3095 in / 
# Mon, 12 Dec 2022 20:43:45 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:51a2a7647f8363ce6e5a9502afe51c4e9651ab6aea92958531d1116b3dc9dcf1`  
		Last Modified: Mon, 12 Dec 2022 20:44:58 GMT  
		Size: 64.5 MB (64492212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
