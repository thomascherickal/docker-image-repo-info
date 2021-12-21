## `debian:testing-backports`

```console
$ docker pull debian@sha256:af1a6c4cf33d58072cf13cf562b26c607b0a09a505be8b317322c79d6bdebf61
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:dfca9b85ab886bb246fa3f0b253cf3d832652c756ccd76f13e07ebd5f683b209
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55599008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3bdb30cea6ee6a78740e302e39b3f72b7853a96b6697c69b77fff5d11e8a69d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:51 GMT
ADD file:d302405af930cc11493038d472572e46ae1d7253df1c141916634ac984b48b88 in / 
# Tue, 21 Dec 2021 01:24:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:24:55 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:277c3ceb6ade1082faa3e2b17e1f8fc09ac549df797657b97f6f47253b55f4d0`  
		Last Modified: Tue, 21 Dec 2021 01:31:57 GMT  
		Size: 55.6 MB (55598781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a841ce30c4c9dd50a4f4eefaa16b535a6ca42378f670ad2be5b574aef6f55476`  
		Last Modified: Tue, 21 Dec 2021 01:32:06 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:78afc7c25430a890c957acaa76cc5b52ef1102464ebb4482cf86229adcca76ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53031472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69ac556ed9cbe484dc5a910246951dce3e3d6badab284cef3e5a1d986e54bc5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:58:37 GMT
ADD file:24d5cbaf475011d519415bede0f00a59e3d60e3fd564ec5377d69f12a2e79146 in / 
# Thu, 02 Dec 2021 02:58:39 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:59:00 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c46357bdde6cd4bf4e75bdbb33f3b028ff99f5015c3d52a5e57ca8a33eda9b26`  
		Last Modified: Thu, 02 Dec 2021 03:16:41 GMT  
		Size: 53.0 MB (53031246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961a7932cdb8bc61f8a247cbf698e484c224e9b6aa5276f65eeaa132f53c1633`  
		Last Modified: Thu, 02 Dec 2021 03:16:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:9edd2d704e33ed2e31ca8aa8dd0501d431fcc6d82bdea18f90bb288095c77451
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50668012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b663779c017d8e9cd27687a8364842ebbe2b6faff8b834ef5098ae825b52aa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:11:43 GMT
ADD file:c21d3d7908d4b616ae5afe976c1f83ac3240f71d57af0a436a192404d7dc2fe6 in / 
# Thu, 02 Dec 2021 09:11:44 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:11:57 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0b32638dc1ab8dd9d3bf82f9e41332502a0e05dc227f1b5cf3214828cd856f51`  
		Last Modified: Thu, 02 Dec 2021 09:29:18 GMT  
		Size: 50.7 MB (50667787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e420462da7f86f26ae7487c26ad036aa13ebd0999db85fb8f77fe27a2c3b1e`  
		Last Modified: Thu, 02 Dec 2021 09:29:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7b0c522a52d260273ecbc95709c9aabf426a473b6ac760b50396597562eada92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54598060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66714187b6378f00c5ef0b61d7d12ee9fdca355438ca67839b0b6836eeac03ae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:49 GMT
ADD file:436a7cbc9b247e837b1662f418559e588633a07d97fbe015b61da9481fb8a8f0 in / 
# Tue, 21 Dec 2021 01:44:50 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:44:56 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ca972f55dc0f92867c66012e7edaba4ddfecaf3952bbd20e050677fdbce9fb70`  
		Last Modified: Tue, 21 Dec 2021 01:53:28 GMT  
		Size: 54.6 MB (54597836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7762072f71dd07afc77f174def188806b78b9350da91f791cecc387df2faf847`  
		Last Modified: Tue, 21 Dec 2021 01:53:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:5e84598344c352393e60dfe19bfb11aa34dc71c6cbb0892d083458301256e1d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56659089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9469660171b7468bcde6944d869bd63c99ac60ffea8baa7a854b33b0ca6659a4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:43:44 GMT
ADD file:fab1ec7b084bb10dbc74380fb1e54f057fbcf6f2adff18fbe85ddbe3c9384bd3 in / 
# Tue, 21 Dec 2021 01:43:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:43:51 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bfd913943f9efe4f7d6ee24376f044314cf7778304a152b131dabcde41c0e0b6`  
		Last Modified: Tue, 21 Dec 2021 01:54:16 GMT  
		Size: 56.7 MB (56658865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ce75a702349433ddc42fe91d82e55a6e79092ae971261fa8e1082507cbb2d6`  
		Last Modified: Tue, 21 Dec 2021 01:54:27 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:7ee00aa23f795c51c4d67f5410de3632fe94eb73d119a7f5e49abb9d9baf2914
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54269653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041961c10f8a86f8d06df9561685284c922eb8c57efe4d0799bdf10b8c032ed0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:13:07 GMT
ADD file:f2e37e70b9a9096d2fb1678f2c206aaec8dc42e69e0036fc44f20c968ce3b6bd in / 
# Thu, 02 Dec 2021 03:13:08 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:13:15 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:31362d457f7840e760c1c73187ddb15944d8264def91872c40ba7eba7e592b20`  
		Last Modified: Thu, 02 Dec 2021 03:51:16 GMT  
		Size: 54.3 MB (54269428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6706e0fbcc3bcee354a93169c8547bf70727c39d46b1a5c5c461bf40da3eb2`  
		Last Modified: Thu, 02 Dec 2021 03:51:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:16d1d07d7a38d7562da7bc0775020479c3548f99f050b84f146cda0a68c95edc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59851603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adb5b28a95b6b7da518860967b339da4893144798ebb43b70086f061f4ee328`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:25:01 GMT
ADD file:972506a48e285b7044e7466c1fa928ba46a90a71739476caa955522c0964e3b6 in / 
# Thu, 02 Dec 2021 07:25:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:25:22 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5f25ee39fd078e721939a7b9f385a6d99e8ecaf99aeffe635d773726e347e325`  
		Last Modified: Thu, 02 Dec 2021 07:35:23 GMT  
		Size: 59.9 MB (59851378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f683037078d613d4b5426dca3078cb3c414be896856d0b868295389793cf7c`  
		Last Modified: Thu, 02 Dec 2021 07:35:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:555162d68e9ed12d159e08bb5cbca8b220b94a0286c4c7a3041a15ac002afeaa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53888621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0edaa6b225b01c8d18401a2488e3a10a3888cd41ebc75a332789163f98ec0d58`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:29 GMT
ADD file:fab1fb88494aec56291007be8c0c54cc9bf3f56228b1e709a070150030986221 in / 
# Tue, 21 Dec 2021 01:44:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:44:38 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:38bb00702c0ff4b51b50541d1787108666c6714b6282d619229305becf8d14f8`  
		Last Modified: Tue, 21 Dec 2021 01:50:33 GMT  
		Size: 53.9 MB (53888397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad63e4bfa25834511b868c121824106819fe64cb67642a54b96b6f769081a83d`  
		Last Modified: Tue, 21 Dec 2021 01:50:41 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
