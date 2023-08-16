## `debian:testing-backports`

```console
$ docker pull debian@sha256:1e66e7e0369a4c3d6033647e95ee553b70c82f732672ff67ba0a9e3e856e6d18
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
$ docker pull debian@sha256:3be7f2ae8e72d846342c37a045586e9b66a65c13358a55fa50f789f4f8552f3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49596918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b94abc53341f94fb3cd012528642faead73bb5f2e3cb0148225636033e4b1f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:27:06 GMT
ADD file:232c5a22b11e6861c0419feb6529d7da6a1b93600f93db9ef865f2b1d8526e58 in / 
# Thu, 27 Jul 2023 23:27:06 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:27:10 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1c40f7ee433c5de1ea05b673e25cceef231449d9025fa7a0c84e238ec3fefce8`  
		Last Modified: Thu, 27 Jul 2023 23:33:16 GMT  
		Size: 49.6 MB (49596696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ff8deaffd80b0df693f26e9c697dd7006a7a91226b803a234d7509e4f406a1`  
		Last Modified: Thu, 27 Jul 2023 23:33:24 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:dff4dea1e6b5d19e2a93c23a579fb635843b3dbd9697b20105ef5110ce3d93ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47395394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe438aa5eb21d8d003a92333887d79ad05c58ad1efc15dcfbfab3009226dc75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:40 GMT
ADD file:5e83651ed24b5e4ef15b8f08928bf55bb69bf326bd2c74abf8f978804598162a in / 
# Tue, 15 Aug 2023 23:49:41 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:49:43 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:86f1da9e05d82606c06a57cacf13425ff6707ecb80697885b03a52539ca02b3d`  
		Last Modified: Tue, 15 Aug 2023 23:54:09 GMT  
		Size: 47.4 MB (47395172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f2854ce8d4ce99b2b8d9df48e2b7befa1aa3b31beaaa71d9be3d51366d2304`  
		Last Modified: Tue, 15 Aug 2023 23:54:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:7a067a851f6c6e831bf907947760743b50f74ba24bf05aebb500f8d175550458
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45212448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a244da2a38e06703c7f74913da0dc15b340a2477690c9827a53a034ec0903e31`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 28 Jul 2023 00:00:43 GMT
ADD file:8e91c920955d8ab2b3460a4cf3a13c192194e92d62f2b0214da91deed5300a72 in / 
# Fri, 28 Jul 2023 00:00:44 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:00:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ba4f9bbc21ba8269a01460490071c98f69efa5cdb87ffbdcdb01d6d0eae7feb6`  
		Last Modified: Fri, 28 Jul 2023 00:07:10 GMT  
		Size: 45.2 MB (45212224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3877047b18c3fe164aa2510e4f6e2993c4ba675015e5b30d6e9ffbed0af463`  
		Last Modified: Fri, 28 Jul 2023 00:07:19 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:837f5c9e83b7b9203fad0bf7fbe0c35c786f6586d214eabb539fb63acab33ec2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49522293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:551b79016386ab268074676324a85cc91e6b81c7cf3aaf4e64f7628ed141c67f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:28 GMT
ADD file:4140d565c599e759836b448aa03732461eb29cbc683f3162d889a36569afd8fb in / 
# Tue, 15 Aug 2023 23:41:28 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:41:31 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:786a118997b083196267446ee0d1d1a908f05fd7748fa2ed8e7560d0db91bf72`  
		Last Modified: Tue, 15 Aug 2023 23:46:51 GMT  
		Size: 49.5 MB (49522071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de73fa2b0e5f203d25e13d5dcf0ec9596f20bbb869353bcc4b2a83d0b05e5deb`  
		Last Modified: Tue, 15 Aug 2023 23:47:00 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:849eb2ce1deef990e9db0062164d7cbd9b13715c9dd4f388a679e3bd67ba590c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50618662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e4d6620c8dfe69c156af07d6a0035aecae0b7ce4069675b76f84830b023f9ff`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:12 GMT
ADD file:a6c4f47b5f8dac4818251e5467ef149381281ebda173ce4edf783f1ba76fefee in / 
# Tue, 15 Aug 2023 23:41:13 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:41:15 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b599f8f04abd103aa7027fa31c11a44e706a3fcb77a3be9e4a64039851404afe`  
		Last Modified: Tue, 15 Aug 2023 23:47:43 GMT  
		Size: 50.6 MB (50618438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b99d82e229dcb931ec5dbf267a288192a06ee83793bf6c0c6ca1eb9c044d26e`  
		Last Modified: Tue, 15 Aug 2023 23:47:52 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:dbf230ef6e825cd9923d21ff80c5e8d79f81ec3ae39369c5f411d6b860cbc69c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49544645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b0ff7b716b316d0a01a476f090fb4002e63fc677d250a7062c4a0d398cdfd52`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:16:50 GMT
ADD file:36edbb732310d3835fd2c6a536e1f062390bd62e09f5a3a65ef35063a1021d65 in / 
# Thu, 27 Jul 2023 23:16:55 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:17:08 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:983342dfcbeef28222cd08e6111464390f87d09531fb648e36e74419b1e3794d`  
		Last Modified: Thu, 27 Jul 2023 23:28:15 GMT  
		Size: 49.5 MB (49544418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4e78361a8dfba8c917901f84027ef13c9cebfa9d54d5475f6f535823cd68f0`  
		Last Modified: Thu, 27 Jul 2023 23:28:26 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:6957f29e0d320c8ac2860f9be1673eba42556e7f82d87497de0ba5e0f0aef1f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53583401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d51c2269426aaa3467e8cd41465f76387ba8dbf493147e26c45fd88f94228ce0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:44 GMT
ADD file:1097cc2b8a1d0dc4c0c138509885cba995ea8e57aec72bb44c61ae10a1597c77 in / 
# Thu, 27 Jul 2023 23:25:47 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:25:52 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:131ae2bf0201dc28363a8c6f4442669eb10652bb0360afa95a3bf4c626d1ffc3`  
		Last Modified: Thu, 27 Jul 2023 23:33:36 GMT  
		Size: 53.6 MB (53583176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee502461dc106f7ce524ee91344f2433df200fe967db2df6983da25570ae348`  
		Last Modified: Thu, 27 Jul 2023 23:33:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:b99dbb106b46ac78ea7eee6a47b172dd8577e8a5a8715e554ddec7a29340f930
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48540022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d673dc01a65ea4552de87c7abf45e75344788e656e29f605cdacf28c8fa24fd1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:44:56 GMT
ADD file:8ee59edaaa7d4498cb111901a75ed6d7cfa7dc646dde70eabca650d719fb7d57 in / 
# Tue, 15 Aug 2023 23:45:03 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:45:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:977206ef11492cbb9ef774b7ffa955b2066c215ff2be2d1fbb83d474a8d85cfc`  
		Last Modified: Tue, 15 Aug 2023 23:49:47 GMT  
		Size: 48.5 MB (48539796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0ee13cb82c7ccdb49719b845e408b2d158a9ca22ee4ea4aa77c94969d5df4b`  
		Last Modified: Tue, 15 Aug 2023 23:49:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
