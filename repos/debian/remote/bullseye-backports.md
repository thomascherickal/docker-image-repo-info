## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:e81b8c5eae8c5ef05ce5e6e923ea70557270cec4fb1ce85dc01040471f331c83
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:fedf51c398206775c017d5d178d00886f9276e283af15b7e885a9e3a9c3fb376
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55046559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8685fbf169b1e0a9107b32d57f5d1e855c41c6326d19d4dea33a0556f1da898`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:43:46 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a52ddb2faea46d24c36492e711d991fac328e4f4ef8bf6a4272f932a5ac452`  
		Last Modified: Tue, 25 Oct 2022 01:47:44 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:2cc9fe0583e04de83a0d23ef9784d16442a259d47518d98babe0aa30a5ae3d09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52547421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5483d59c5a23b20d84523cbb668633f9dd46e349fa077ba3fa80daf6f467e15`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:48:56 GMT
ADD file:e5a40ed79070e00490d94152874430cb225b3b00e8ca84eed2bf5fc8c0bd8155 in / 
# Tue, 04 Oct 2022 23:48:56 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:49:03 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5662b6ce27f2ffe436703124b1912c3225002537510f22d7c95f9a34c5ec19bb`  
		Last Modified: Tue, 04 Oct 2022 23:53:20 GMT  
		Size: 52.5 MB (52547199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098fdc40de8b6cc08dda6bee291651148366ec0aecadaa8f7a8628ad2a56c4c3`  
		Last Modified: Tue, 04 Oct 2022 23:53:40 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:c0c1465f0625b4b538ef7c72ca9c6168542e83df7c07899192e52cc5b8dacb9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50209313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2406bcdf56ba61d48051546df49fc18baf80e3d93f9822dac882d2688d17074`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:28 GMT
ADD file:47a3f2948af18c39686ca59a88a439c25edaf286064d3a2ccc5dab47fee2fc52 in / 
# Tue, 04 Oct 2022 23:58:29 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:58:36 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e19342fb46cabf6147aec1d1c6af1f3a82736530cf3b067835fc8a09da092ce3`  
		Last Modified: Wed, 05 Oct 2022 00:04:36 GMT  
		Size: 50.2 MB (50209087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485dbc56063010c53a5aeea3de25ee61bfc1448ce8f0a5f8e44f39a04247e4bc`  
		Last Modified: Wed, 05 Oct 2022 00:04:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:421bcb39cf3597a945491b0613e3b0586830cb87d6358cc5b29fabd8597c267b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53700852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60836a486e3dedadd42c5eb6bc16cb708a106474a4cf4f4050efc797ad6e37d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:26 GMT
ADD file:59bc45fad9cada77bf8e44ebdd982c7f6e575816b5ed6b7d1d8494faddd9b8b9 in / 
# Tue, 04 Oct 2022 23:44:27 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:44:35 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:172730635f67c8f081f43275b390514bd8a05a4a7c3c467ae74ee42a029dce2b`  
		Last Modified: Tue, 04 Oct 2022 23:49:51 GMT  
		Size: 53.7 MB (53700625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cb4d1cc1c47818ba7b48d6f1654fcc01782df7c92ef4bc7522dc195036e24e`  
		Last Modified: Tue, 04 Oct 2022 23:50:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:e345a26d0bb005531cebd9c61d8ed8d255b92717829bb75cefd94c1dfcbe458d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56024031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533d16b2b39f50deabc1ebf0ba61a0a619102ec31acd9bb5ec23b15cc04d5254`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:23 GMT
ADD file:4b457c51f15ab38743966e658d3174639e9eeae2719929bb637bb9a59a598d97 in / 
# Tue, 04 Oct 2022 23:39:24 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:39:31 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:783379f2cdb66b4983dea0044fb0e139918a738a077f65fff29c85bb20119942`  
		Last Modified: Tue, 04 Oct 2022 23:45:03 GMT  
		Size: 56.0 MB (56023806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03446ab2d3a93e68fd3303d1ebad22441b967d14d3673e0a76bef1dc83ee8c94`  
		Last Modified: Tue, 04 Oct 2022 23:45:23 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:d2767c0f822a56b642a28473fd2661cf29978271cd524530bfaf3b3ba1ae3e80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53266064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a2b43d1f610f244f69d1eadb4ee03af2e93fac8aaa767640b21a7622698eb0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:09:48 GMT
ADD file:ca40db2df3dbc600910b8cd139c564cf5b8bd6c1a06cc517cae2c1c05cff6dde in / 
# Wed, 05 Oct 2022 00:09:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:10:04 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:25bcd35faf05f859c3077f0e2e7010d24e56cdcfb77efbdeda236e47dc08e14a`  
		Last Modified: Wed, 05 Oct 2022 00:17:52 GMT  
		Size: 53.3 MB (53265834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753a0f44f6a133163d3cffdecb076b58916b16b2bfe294b7d5a9d925b4b7e808`  
		Last Modified: Wed, 05 Oct 2022 00:18:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:a08ae989ab7e2137fdc7bc09523bb9c5145e535c2e5d3967fdddcdfae4d4ef7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58917486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:021e2846de4a47018b4e6d6ebfca090e0f55e3b6353017c0cd925481af943065`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:17:40 GMT
ADD file:74537fb4eedf6a0c9693fcdd0c9acb2797046cca66098b2e05d5c1a536a9aeda in / 
# Tue, 04 Oct 2022 23:17:43 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:17:50 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e05b86739fed11b3d0c5663063e627eebea0138239b30345630bc7e3f2549d5c`  
		Last Modified: Tue, 04 Oct 2022 23:23:34 GMT  
		Size: 58.9 MB (58917259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd03a9e8c1d6b166f06d589cdf410461d1e8274acd83490e5e58b8778ec4055`  
		Last Modified: Tue, 04 Oct 2022 23:23:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:ecb899df1bf1c6dc735d44d72672f9c700c5aa2064add61eb9ec2288d172c11d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:854f86818df518fbbd8e1a07665212ba69d31812e95a3031395632674c7ab0d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:14:24 GMT
ADD file:06f15d8a3c04752d271a052e820fb13fcdb76f0d18f6c9afb6e70391d10348ec in / 
# Tue, 25 Oct 2022 01:14:27 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:14:35 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a556186e8bea4ba9925d0c17bea2c12bfbb931653cfab1b980036800482cf0ad`  
		Last Modified: Tue, 25 Oct 2022 01:18:39 GMT  
		Size: 53.3 MB (53279106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df24abe952c77dafb89ceef29a5c3b51ad93dec220f4f1beb4162770ef179dce`  
		Last Modified: Tue, 25 Oct 2022 01:18:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
