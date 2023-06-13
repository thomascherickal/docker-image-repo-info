## `debian:testing-backports`

```console
$ docker pull debian@sha256:e0ed21a0928e6d5f22f214ac8aa7fc72f7d3acb85d41c3aa4f8598b7e047f0ea
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
$ docker pull debian@sha256:ad44ce21476bdc3413c59e267f3b876c83dce135c717a721e5497ea8d1db0db2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49552333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23c96d04fe8ef5db0b0e6f7392791a72d2b67bc5f727e15e52b144ed2103e6e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:23:22 GMT
ADD file:418560b5057bb018516c119e87b040f82c7dce4d4961e8bf73268adb278e1635 in / 
# Mon, 12 Jun 2023 23:23:23 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:23:27 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dfaac2cc63fd541e1c2e3738569929f032b19fa4217d0885ba3920b8a4e9e69d`  
		Last Modified: Mon, 12 Jun 2023 23:29:32 GMT  
		Size: 49.6 MB (49552114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a0cc64ae67aaa051a092beb142cc5e0a3bd6692808014c6f10eb35a783a92d`  
		Last Modified: Mon, 12 Jun 2023 23:29:40 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:7648dd154d7dcbb20c1a937e134787e976d775a8c4738c63280fc26bb3305d8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47403455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:350b70005bda1837555e203cc078b5f4548aa5a85c04dd0648c7cae564f2df5f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:49:39 GMT
ADD file:35030d9d4624a1a802acfb4bc440ed2f55b7993fbe0bf5b2792190de725c633b in / 
# Mon, 12 Jun 2023 23:49:39 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:49:42 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2384ad9b3804a19403d23168d3fca6dcc9be198493eb4cb1dd0bdba8f7cfc839`  
		Last Modified: Mon, 12 Jun 2023 23:53:58 GMT  
		Size: 47.4 MB (47403232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9b59de89a20535c1b038c48550dc28808412649595f65c9507e409acb1c29a`  
		Last Modified: Mon, 12 Jun 2023 23:54:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:aa53d8c74f66d41efd8598b2bfa6fe55230dbadbb781219afc7e9083d036c132
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45236393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1f47c028ff26d547c33ae2a296b3678cc5c7dae5e754759f118052e44cdd5a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:01:27 GMT
ADD file:b64c67ba0e28271141124bab3303d56c809b801ee29f7f6620de1c8a1de21b89 in / 
# Tue, 13 Jun 2023 00:01:28 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:01:32 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b2ce7d8b1c0598c2e67a91cf379ce592bfe21db85460aaa797339e82750d3319`  
		Last Modified: Tue, 13 Jun 2023 00:07:31 GMT  
		Size: 45.2 MB (45236173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f55427d67232dfb48f4fb4454483c99e94000e1c4b5f47d77bc642785c8b51d`  
		Last Modified: Tue, 13 Jun 2023 00:07:39 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:22b86a48f0f1d071e29e4c2dcb7d12c2e86bf0720d9da6c583c2d2d8292046cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49573381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:702a4e3a935b382e27d8bbf73ae4fb97213a4413e978abb65ec59245af9c7497`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:15 GMT
ADD file:9538b10221306d569a3379a42ad14f6a04e3400effaf2e6093c219ad3ed820ff in / 
# Mon, 12 Jun 2023 23:42:16 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:42:19 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7f36dd606efeffdc09debbf5d2f9a2a9f9cc7b769ef21cc6ade380d05fc0bc8e`  
		Last Modified: Mon, 12 Jun 2023 23:47:29 GMT  
		Size: 49.6 MB (49573160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df6782ebeffaadec7aaa82de0a63099438deb7916ee4e26fee93e1bce399c5c`  
		Last Modified: Mon, 12 Jun 2023 23:47:37 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:fc30249799e61e937c89665f31eb3c9276c79052e245cbdc31e47cbbe7bdddca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50562617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac193aa9c4f727eabab408d298c4739d569a8bee63c95458e3e184cb0f9ba4c0`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:43:23 GMT
ADD file:f24049f634b6590eed9ed3e10420c4d00579a880a5a561c7ef5c6f03611f432a in / 
# Mon, 12 Jun 2023 23:43:24 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:43:29 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9879a6f3c670f447138db14564ed395b00d6f91ed6887a41bbd0e84282f11130`  
		Last Modified: Mon, 12 Jun 2023 23:50:36 GMT  
		Size: 50.6 MB (50562395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4489f332182d9e27b163e16c834ffed4169dc5fc8703841b6a427d5d538f7e7`  
		Last Modified: Mon, 12 Jun 2023 23:50:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:b922a88f883913a9ffaa675fb4165950ee47e0e22a55081edc7a593e83fbb275
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49541761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3143afc33fa585cced5955a7b415c317d2d72f950b12844fdea1e126832d8ea8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:15:55 GMT
ADD file:a714ecc1d06fa2be0e4b336bba5b8d84a128d33c82cb3ad6da9357b51b69761a in / 
# Tue, 13 Jun 2023 00:16:00 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:16:16 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:67317167503a5f34e0e7d6389bb904e1fcc700bc4f9a5b7fa8057d590607fbd9`  
		Last Modified: Tue, 13 Jun 2023 00:28:21 GMT  
		Size: 49.5 MB (49541538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf06b0f58fbaa227540f42b40230ce9411a82cf2e9b14e7eff3cedce59740294`  
		Last Modified: Tue, 13 Jun 2023 00:28:31 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:db71c86aedfb43273383f9b4f0d360e9f17a5dc1a278512899df622de181e583
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53536978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa43df3a03754d00f193191cf5a7b567f9d5669899712ee090aee9722987e78`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:50 GMT
ADD file:c800eebe5b5256d5f3eb9d436f7401634618c397b30f31d8beee6daa24772dee in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Mon, 12 Jun 2023 23:21:00 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:da363b5a528e02b2ccc2452bd956ac683fa34d495ffdfd1407ffd0bd41cb001a`  
		Last Modified: Mon, 12 Jun 2023 23:27:36 GMT  
		Size: 53.5 MB (53536756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e23b368c7284e37b37c0671c043a33f1458cf8106cead436a2ce1315c3460a`  
		Last Modified: Mon, 12 Jun 2023 23:27:46 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:b16ef23cdc032d4778fe8c1a48f1deb34c20540b320fb109329c4b6dcbda0fe2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47921819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ec2af4f9773853b712f56605736e955e53beeb16fb912890ca9a2f549a8a2b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:31:54 GMT
ADD file:db470514d90937dab99540062bd1d63a3d21f955b13492e99665e3081e72ebac in / 
# Tue, 13 Jun 2023 04:31:58 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:32:05 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6fc736e25918c8d44a93a09b96e2f37f7bcca7f1aac4e82dff1e4ad58dec740c`  
		Last Modified: Tue, 13 Jun 2023 04:36:10 GMT  
		Size: 47.9 MB (47921599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1109dc93d832f96e6bcc511c00570a62674a61bfe0e1a07ffd6f45a7a952b`  
		Last Modified: Tue, 13 Jun 2023 04:36:15 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
