## `debian:experimental`

```console
$ docker pull debian@sha256:d82a5db540521787ae58cb9c82fa35edf23517089db94b4c58616f5b55d53333
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

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:7ed2f1729a2e49b53b19733779eb763c30901fcedd89c3508e8b3c7b4e4acc0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52769000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e26f8d70f370666e8f61316464730a954bb39a7f09736fd118d89400a1d038a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:22:36 GMT
ADD file:fb5801241cefe989ebaea4535c1783ade754d3f110b6582a1bf373193075d454 in / 
# Tue, 23 Aug 2022 00:22:36 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:22:47 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9982fb59e253104d024374bedd9697731eefe95d4c35d5f4d76b419739ba8548`  
		Last Modified: Tue, 23 Aug 2022 00:28:22 GMT  
		Size: 52.8 MB (52768778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92dc0bf0ff16d9a34d1c033e455af7967e1f39edcbfac4a6d21eb5c1459ce38`  
		Last Modified: Tue, 23 Aug 2022 00:28:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:65bda137ef63b6b3b342e7c9cb06b77a4f717221fddbf5842a778f5cb8ecbb2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52021628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22bf43d48b8acb770ae16c12f63dc174ed8451a2bbf51cdf58f0945107a3345a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:51:50 GMT
ADD file:8165c0d978757c272b0fc9aab3bf8bc8644579a857290a6ba3d25f5e06be2ad4 in / 
# Tue, 02 Aug 2022 00:51:50 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:52:07 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c32afc4cc9c9df6d376376afbae71bc1e87837dd8838c5d55f5854ba7298b657`  
		Last Modified: Tue, 02 Aug 2022 01:01:30 GMT  
		Size: 52.0 MB (52021404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13804901e30c4db3bf34c853bc1b62a7f18ab26005b2da85a952728ef852af2c`  
		Last Modified: Tue, 02 Aug 2022 01:02:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:47a59dd79c99d0396ea8c2319b0b2804dd4227a552e2df587e27f9bcd36ca001
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49735552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9344370ae235d094c05fe6ca1ae1a95fa40393664f3dad7f4973cad5f528e447`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:26 GMT
ADD file:938fb1d62b5f37e34560628bf97a9d4b02fe5c41d5aa62171e22f61fd6820e14 in / 
# Tue, 02 Aug 2022 01:02:27 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:02:41 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:25465063d4ddc9b103f13125cd4fdd8eb57bdc4e5ad39afe15db8f828d80d508`  
		Last Modified: Tue, 02 Aug 2022 01:11:16 GMT  
		Size: 49.7 MB (49735331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7071ec524d8a3c1f295379d1a6441356a595ace9a7c3a0f8e065b61cd265975`  
		Last Modified: Tue, 02 Aug 2022 01:11:42 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:58e8138be5496b8e39af0d52a9560cb08b32ea8408971b0d687c37e81d337eae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53312003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9881d82d4e8ede46b1c4a370dffaa02c73b4e485e347e2bceb4c97cfa162b26`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:43 GMT
ADD file:f319e3ad56cdacf4f559c33e21c65bc34192203c7cfe561c49951febe8d41d11 in / 
# Tue, 02 Aug 2022 00:42:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:42:59 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d7f89fc086c7d917b11f43154b1526ea2314922b905525b6bd85dcd4b7ad7e96`  
		Last Modified: Tue, 02 Aug 2022 00:50:22 GMT  
		Size: 53.3 MB (53311783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba2758a8c5115b90983ff91e9450cf9b37718bc7dd5da83f326213a388a9526`  
		Last Modified: Tue, 02 Aug 2022 00:50:52 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:9c6767364508033bf234cf39b17b6eef7285da5f9a70091ebba1620033b1d277
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54195289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9542ed6f00ef909f4d84470f0a8f4cd531f9336da9b31ef20d1e76173bdc5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:33 GMT
ADD file:86aa5ea5e610e7d9bd402025a337e0f305b103598be63b78b6b0cdea7a3df4de in / 
# Tue, 02 Aug 2022 00:41:34 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:41:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5699b5f3fd16f897714b4784f589776f740c6550b1714d3050d6370b669db263`  
		Last Modified: Tue, 02 Aug 2022 00:49:25 GMT  
		Size: 54.2 MB (54195065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0841e5987f50cdeaf45bf3836fa418307c90a4e91ac439e2fa3451c95b330918`  
		Last Modified: Tue, 02 Aug 2022 00:50:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:7f1b884cbbffa5b3e0d22f887d427dbf8f9b7f7bae3e4085dd5aee0a0baab28b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53216875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7054f25de1425f072e88a81807a07f1e3f38fc2072c6807c4dd3a120cb230e4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:15:27 GMT
ADD file:289ff967122b94852c18b08616d72bff729cc9d607c295c6c758bb8917ce5864 in / 
# Tue, 23 Aug 2022 00:15:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:16:13 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:10ecab1bdcec7f490bd4865c91fc25cfc0d3d5506b9673055d7740a86765bdea`  
		Last Modified: Tue, 23 Aug 2022 00:24:06 GMT  
		Size: 53.2 MB (53216652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8187526258e55e7a283249775de7fdac990d25e667fd1d930ae0538e05ef8d`  
		Last Modified: Tue, 23 Aug 2022 00:24:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:8ceabf78899abd35ed519aad4d1dd26b176bb7fe4baf0bc6d0eba73dded0ae4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57440435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c42cf3beacaf18a40e1c51df95e38a13aa8ba31ff28414e192ea25b98aa5e439`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:28 GMT
ADD file:00f45e966a1bf81446cdb8892a3b57307803b4b3807e49c2216eb498d072aee5 in / 
# Tue, 02 Aug 2022 01:20:31 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:20:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:85140a3e683aba1b971bf67cd28210279f0d3da9cf83b37f47047f37badf66f1`  
		Last Modified: Tue, 02 Aug 2022 01:29:43 GMT  
		Size: 57.4 MB (57440211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe215d99685d0bf9c634711ca259fa19427e5788734d2972a6baec2e58df978b`  
		Last Modified: Tue, 02 Aug 2022 01:30:17 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:d0fc011bc400eec92d94f1fd20be03a0b297fda36f5c500670e6a3fc607ce352
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49268422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b818a232cb48bdf3ca4b84bf371194cf9db7306df1a847f76a5b93c975490ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:15:54 GMT
ADD file:922879b545740da41d47ffaf3bb1d9f5cae855386457ae213834f5f1eb869dac in / 
# Tue, 23 Aug 2022 00:15:57 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:19:28 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:243eeed5cf29613bd014532fa4bc8fb367b678d2973dc4a950c09bd2df4886c1`  
		Last Modified: Tue, 23 Aug 2022 00:34:23 GMT  
		Size: 49.3 MB (49268194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9074adb383b955e8e4e755127062849db72c1e821950bf6386d8470eff567f`  
		Last Modified: Tue, 23 Aug 2022 00:37:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:2cf3bb5edcdadca734a6b4cbdd3512205941b22d6f79ede0aad35e46219c3579
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51734886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a25d77266bb510f6a354a417d2426e60d538f5f05f61e1e31267bc62cbe9c64`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:44:54 GMT
ADD file:984d42e0d8c3e13cf8d8ee6608f0302c63c5b967b172fdcf3761d14a4b52a4b9 in / 
# Tue, 02 Aug 2022 00:44:57 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:45:12 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b0185da9188245470949775bd4011291c882eedfed309ae9f441a1037dcf027d`  
		Last Modified: Tue, 02 Aug 2022 00:51:18 GMT  
		Size: 51.7 MB (51734667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4138c8d0e1ae99014aac269457329e461183d106799474d741363678a97449f`  
		Last Modified: Tue, 02 Aug 2022 00:51:35 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
