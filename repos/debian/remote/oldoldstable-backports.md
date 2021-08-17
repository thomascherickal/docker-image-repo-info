## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:7b21b08331179b9cd900c5c4762efb79226d67ded7a1f53e33a22b77bcec8f56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:229b862e38b8a38f713a2b039c3060396dc26fce1c7b22904f440341271825c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45380170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546e353cb0ac1aa2359bb64abe05f04cce92e5f17ba6e4470b36abee0d7d811e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:17 GMT
ADD file:baee0d1b2f877558f1acb1122c485a282c09888ae9727e80a3996491ddd78a67 in / 
# Tue, 17 Aug 2021 01:24:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:24:21 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:223dea9d4fe0256aeb75b4dccfa82fe784a491d8571e6ea2f50f42df43d1a7b1`  
		Last Modified: Tue, 17 Aug 2021 01:30:41 GMT  
		Size: 45.4 MB (45379942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa67c12303ef4fc6bc76b68037c4e651fb5f23cc71b78cd66817ecd213aa56a`  
		Last Modified: Tue, 17 Aug 2021 01:30:51 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:402fe463da7b7656b1b6ee9fe9cb3254915f45ab4297031c4ed62e0c11baf880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44092080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec93c872c82c853bececdd5a5d3fc2fb572ef3c2ef26216ea5fcf3493f5c66e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:57:17 GMT
ADD file:b8c5338c0156c44d6c283c0d9219581d03295620a138b8d5985cfb8b1f26de32 in / 
# Tue, 17 Aug 2021 01:57:18 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:57:31 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c043942312a0a3f1f9c16eba90cab7933a4c3d5c4d2757553a776efa224c2b49`  
		Last Modified: Tue, 17 Aug 2021 02:13:29 GMT  
		Size: 44.1 MB (44091850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c72e6b2da9df1703c3b7fab56a297f5a8a86325c7d67474926884391542c88e`  
		Last Modified: Tue, 17 Aug 2021 02:13:42 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:59057ed0ab64f48f4602059ca431d3ad9ebd369cffea5b54b79776bdac450dd7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36620191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af713ba3aec6f1645af0f3a129c4d1af4b83b851cbc58b6fd3df9e7422c56f2a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Mar 2019 13:06:27 GMT
ADD file:0caee109b4cdcee58b1f6d8abcd0cf00f38860b85cf7a8909615e37b6954b58f in / 
# Tue, 05 Mar 2019 13:06:28 GMT
CMD ["bash"]
# Tue, 05 Mar 2019 13:06:37 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:65fc7f64df1df19bf879ad0a100f67326a874355f02d8bc25769fdb3d7e7e2ee`  
		Last Modified: Tue, 05 Mar 2019 13:16:06 GMT  
		Size: 36.6 MB (36619961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb7b16994722c8b29fbc263967ed8cf48f4f625c7e2383ea2bc7c290b9ec6ff`  
		Last Modified: Tue, 05 Mar 2019 13:16:15 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:60e2498222cd13fac3a57f60b2fa28c4bdc4a0cea9030ade6be78d801d89c89f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43177917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db9d3377c257bbdfc7038263b0617965ceda17a978adebdf94c2fcc5d69f5fd3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:42 GMT
ADD file:3cf60abf9f5227e23d0e753ad3a4f3453be83da1d5574be522e54a80a00eae4e in / 
# Tue, 17 Aug 2021 01:46:43 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:46:48 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c9d798901bc9c12062d35c23652c101d4b87a1064d4fa1019eba67059f98754a`  
		Last Modified: Tue, 17 Aug 2021 01:54:45 GMT  
		Size: 43.2 MB (43177691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae23ef3a68babc86cd41bd71c23f772a361d05b7bed479a29bb726cdac06e435`  
		Last Modified: Tue, 17 Aug 2021 01:54:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:02dc946ffb9c60672186861bf2c6f49d8a47263c89a5319978f8ef6ca33612a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46097507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68777e8a55fcda817f68cdf4402c81310d7634cbfc63f87266aa781f9f941a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:32 GMT
ADD file:2630d2959b6158722fa0a864f0ea1c1e15bc26cf1a139b0132bb8d6dcf7b9aff in / 
# Tue, 17 Aug 2021 01:41:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 01:41:41 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6462db426304928b210edaf7719197f7e7ea0a785522918c8fa942f50f55786f`  
		Last Modified: Tue, 17 Aug 2021 01:51:23 GMT  
		Size: 46.1 MB (46097279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e15aa6c54719cde8f47a57683d7eba0eb45439f8300de742c2c8dd37e8cb2f`  
		Last Modified: Tue, 17 Aug 2021 01:51:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
