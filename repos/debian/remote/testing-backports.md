## `debian:testing-backports`

```console
$ docker pull debian@sha256:8128a23385bbf6e7995f7f846a804fd4fa3af6504c6d359929280f806ca8faba
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
$ docker pull debian@sha256:e86c4b3c72a0e8768b551a6c28932e95ddef46f3e4f04bb112b7dc762d915eda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49299469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1294805f7eb298e58fafe932b38e0a21f5937227e5f253c3dc3d64988473a5bb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:48:15 GMT
ADD file:27b4229d808812579f1eb7609d08a5bb2177380a480279009a4ea17e05193323 in / 
# Tue, 02 May 2023 23:48:16 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:48:18 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:56c7136ddbfad3eea4cd5c38c0703e58fd25630219d5462a9099387c4b3a4160`  
		Last Modified: Tue, 02 May 2023 23:52:53 GMT  
		Size: 49.3 MB (49299248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6401c83577903f6232bbd710060d2f90fecad3738c81eb1d49b11bd794829f7`  
		Last Modified: Tue, 02 May 2023 23:53:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:918d74a55e77e38f689b8a89a5432933f9800414607a7e62dc4db75df8006d06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47167421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af579121f47265597149cf1d4b3096174818eb5633881e970472aba2eaa2e20a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 22:49:27 GMT
ADD file:e453aa4ddf2f5bfa2412dd44d2457067e34bc3a8fc8f811568b37ee5c39828a3 in / 
# Tue, 02 May 2023 22:49:28 GMT
CMD ["bash"]
# Tue, 02 May 2023 22:49:30 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e2772b4d1fc0f0569b1a8bf114666e528e1e520ff336a1c359016b38622649c3`  
		Last Modified: Tue, 02 May 2023 22:52:54 GMT  
		Size: 47.2 MB (47167198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf7669d81f1ef2de32d6f289764ea41019e0224e0eabdb0c99df38b94bdf02`  
		Last Modified: Tue, 02 May 2023 22:53:02 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:f779aea173e34e335d8bca392f2c46e1364eb4af82955f7d757b89f44e31b07b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44988294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fb1c6db153b20c145fe8104663efd17a59c91585b5df1159a4ad4b13d7a48d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:49:21 GMT
ADD file:05f043a303cc0f4a85b0f2f0a32f504031ee3936fae55558de52a22283c53838 in / 
# Tue, 02 May 2023 23:49:22 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:49:24 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9a05bc73d931b8527d6b295b6546dc720a48d4e2891ef21178cbd3c61c7e33fa`  
		Last Modified: Tue, 02 May 2023 23:54:09 GMT  
		Size: 45.0 MB (44988072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfadfd114bd9019a114aec77267b5c6dc9b5a3542bb85245c611b30daf401a56`  
		Last Modified: Tue, 02 May 2023 23:54:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b958a8b8c944c4c932a8809c5c9761efe58c0aa9c8fc20798933b3418b50b86f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49345587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df509ee94bba241f03867afa48de9f523a716eb39d96422153ed75c2a38844a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:46 GMT
ADD file:80a4d0d891f9f28bd3948de18579583b6c11a4a8805b6230daaa0ac2a35c453d in / 
# Wed, 12 Apr 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:40:49 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d1d33b0463b9cb723855fca4aff8cdc62c34a1907b920e8e626bd38d7577387f`  
		Last Modified: Wed, 12 Apr 2023 00:44:53 GMT  
		Size: 49.3 MB (49345366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824085549218ea0d8a075e376c040022cb0bdb5d2c70f355da9f5b74fdc5d64e`  
		Last Modified: Wed, 12 Apr 2023 00:45:01 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:4893190675e0d4c9d9404b29a9510a4c74974d4a46b25dbf43f60f9271d9056f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50322051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198ca4da2f0e4c7e0b615705dea612c105216b8614fd088341fe21cf9d5869eb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:02:49 GMT
ADD file:3d066013b3be4718550f5260b0a8f7ddaaea611c99e260d567494c5ebf34a3ff in / 
# Wed, 03 May 2023 00:02:49 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:02:53 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:35877175544499592a9beaa849d512b12a1677842b2282927c4bcad3159d4f6a`  
		Last Modified: Wed, 03 May 2023 00:08:05 GMT  
		Size: 50.3 MB (50321826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3f1853cfe401b9a8e611240391f128f3f0d2099ecbe0bf8eae66115e738d1c`  
		Last Modified: Wed, 03 May 2023 00:08:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:239edb18b6e94287d837ab76506f385d6061ceffcba88f7d80558bdd92063394
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49301583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c36f38557118db4f48bad830c8d7fced11d48c0bd918aa89306792ccfe91e5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:52:51 GMT
ADD file:5db05cace0a0464480d86b847c4a96ad31c798fb2bcf52633e0a463f0e063853 in / 
# Tue, 02 May 2023 23:52:57 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:53:12 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6618f5c20ebe646969576379f9b25c6efa1dbf3817e76222ffdbcb9f61df2abc`  
		Last Modified: Wed, 03 May 2023 00:01:16 GMT  
		Size: 49.3 MB (49301358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bd0d7748a6bf64331115c897a28c01a7fbdf81fd0e69bd156e98809ea7cbf`  
		Last Modified: Wed, 03 May 2023 00:01:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:96d7b54f0268962c06529af3d7a7e5ff47172d33d6bd7cef62f240b57d688561
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53300211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46d22bfb580d41af378c86caac475266f2e64c5d9d53d80df106cbbdac63e0eb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:10:00 GMT
ADD file:107d4f159f2bc5b04467e08852422f5c78548e0f92853bd29d5d2b05b387d3a9 in / 
# Wed, 12 Apr 2023 00:10:03 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:10:09 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a4fca5aa8bf3f9957686fb6705daa645629edb94592f35c71e46e52a1742ed1a`  
		Last Modified: Wed, 12 Apr 2023 00:15:06 GMT  
		Size: 53.3 MB (53299985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a64bf96cf803ffe2505fbac1e0c249266e23f4901c9f082ece5ea0af9c8361`  
		Last Modified: Wed, 12 Apr 2023 00:15:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:8ac017a8c6eb467c9ac5140e50fb9481d203fc191eddc7de9142f439c8ca8e71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47670629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ccb3922ba228fb9cb3d2d4b1ad27f87fe6a2301c2c337986cf5610d264c207`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:02:57 GMT
ADD file:a04191f521f5135016e837ec503a63f4e8488c1a13030ba67c96cc8f68da9d50 in / 
# Wed, 12 Apr 2023 00:03:03 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:03:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0d66e85e2f078d0a3241d6085f175f28d3ed3f6304a2561cc20fd703234bd4bc`  
		Last Modified: Wed, 12 Apr 2023 00:06:14 GMT  
		Size: 47.7 MB (47670408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014d306832faddd6ad34c518e489793391a11865755e5a2f833e5cb6269f39c1`  
		Last Modified: Wed, 12 Apr 2023 00:06:18 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
