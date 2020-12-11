## `debian:experimental`

```console
$ docker pull debian@sha256:7816c9af4785acae2a5106f17b02f631ce188c20c857f9513d8e94f50baca522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:7c6161579a9240be3ff26f9853f8f31968b80abd89244b93e7310d92f174a928
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53352878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ea08a04642486a96cda9a7ec6be6b1ddf4163f385295355a89fba85c4426806`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:44 GMT
ADD file:0ef8e76cde130d3f049e85bdfac1292f2411a3d65f704e1b3b7775fbe2a4c98f in / 
# Fri, 11 Dec 2020 02:09:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:10:02 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:38f54f0c57a31d9522970c134a72491612f81faaf99832d75020d1ad121d3b9c`  
		Last Modified: Fri, 11 Dec 2020 02:16:38 GMT  
		Size: 53.4 MB (53352657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0eec07f7ec70c00916bd7070e7c2c7f284b59afba369242f6746ba8c31b505`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:0e41899f9267353e2ab7bc38690267ff68c9cafed807207686c7c22525711493
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51288667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc44c3a3a3c22757760cb03912bb79f3c861cb90b599a168509bd0b18d0942c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:28 GMT
ADD file:a7f4d580cd66a64f3f242b117a4f08059e38aa1c473f0ac7dfd92629c479a01a in / 
# Fri, 11 Dec 2020 02:11:31 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:11:57 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1ed8d7ab56d0ede8aa8b5b8b9a8b26bbbdf5fb7c57fda6626f4fadbc4af41367`  
		Last Modified: Fri, 11 Dec 2020 02:20:32 GMT  
		Size: 51.3 MB (51288443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604dd85673d3505f7d765e0407833b6c7e56057accb9d7ea9fc64f1b779242ba`  
		Last Modified: Fri, 11 Dec 2020 02:20:58 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:230373f95d5f46a8d27a6d8e3b96f1fffe080ae82dda9f0c0c9c64a08f678417
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48987546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fb5d6eb47d4b39fbebfe510a5e85cf29ace658c2c78119cdc46f514fdaf40b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:29:45 GMT
ADD file:248943592a8d918c05de04875ee96a8ccca11efd6594b80eab867d848f5f5107 in / 
# Fri, 11 Dec 2020 02:29:47 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:30:13 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8595e153f2c82822a0ebf4b38bc9ae14094244a9a165aa45bc2909d6f060da08`  
		Last Modified: Fri, 11 Dec 2020 02:38:15 GMT  
		Size: 49.0 MB (48987322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45da047ab758c383492e60f717d33351b53abc1765d70b37c0c3490e38560b8`  
		Last Modified: Fri, 11 Dec 2020 02:38:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:740938296ba9a5364285f1eec47eaa952297a748e0f324e398012108fa90293e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52214611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10654e8bd9e13a9d162a35e8a290ec5ad82ac3bc61ac8149ad6ac9c031d991da`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:49:47 GMT
ADD file:987fe6b3e9dc3765e6bc14d3aadc50a8bd6fa377b3e2ecdafbaf88566d35b133 in / 
# Fri, 11 Dec 2020 02:49:49 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:50:16 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e97e991b121a19ee45d4f495386a02f820116cdd040f3d8dbe6800369c4a614d`  
		Last Modified: Fri, 11 Dec 2020 02:57:07 GMT  
		Size: 52.2 MB (52214386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ecd0b3c7c2ed678064d044c10f97a27a3b5d10c1da54e174adb74f5c912127`  
		Last Modified: Fri, 11 Dec 2020 02:57:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:d23ace22f185b8b9226b7b662b25b569f32dd1a94578f055ab76761a9f231795
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.4 MB (54407862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382dc9a73d6d250c2b83160ea6e3d2fa5927e5a2004a42056c3f0d428820e4f0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:43 GMT
ADD file:56dbdafae9410b4af6abd589cf205b4ece531f0fc87050ce72455a70fbf37681 in / 
# Fri, 11 Dec 2020 02:06:44 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:07:03 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b114787a7074ed08a66d9547ff66ad04ffe3321a8031dc27ba2142dd3a3ab4ce`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 54.4 MB (54407643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e0c40a5e7e224646b063a215fa0923cfeaf8a392a88572cbc7ab814c811ba1`  
		Last Modified: Fri, 11 Dec 2020 02:15:03 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:62cf88f81d7cfa4649a8ab39a0fe015a0ef873619f752bc49d18d838da65aa73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52069992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ddbdae1d0b6339f06025295a99769c499c31e96ec0c6cdfe8543cf0fa8e180e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:15 GMT
ADD file:ab83ffe984d9ce30a32e6fa263f04ca1ca71fb5ffaabd9eb84478243bdc7a32c in / 
# Fri, 11 Dec 2020 02:06:16 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:06:39 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d65637219aa0402b13e0cc678214757e4d88927afdca61d09a0398e107fd8912`  
		Last Modified: Fri, 11 Dec 2020 02:15:10 GMT  
		Size: 52.1 MB (52069770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991cc5c8626f01349109bced570854a5cac18dd0759d2c765c53d7d3f2a0bbaf`  
		Last Modified: Fri, 11 Dec 2020 02:15:53 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:a908e52d5355a2a26cb60952baa24b115ec4c1fce0b4405c7cd751b3fcff676d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60189559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6913c9f94ecb7c43ef8285660308b0d32fab85f6ca6d9368bf661322a2a06071`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 23:26:25 GMT
ADD file:dbbe373789a3ba2897f063390858924d6f2ace4771f0b5ec513a2a9e7c8257fa in / 
# Tue, 17 Nov 2020 23:26:32 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 23:27:07 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5c5a40ddf44192866bb0c05807090374b3439dd2b53a5fdf3c7450526cc56881`  
		Last Modified: Tue, 17 Nov 2020 23:40:05 GMT  
		Size: 60.2 MB (60189335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26c74289059a54e79c43d6699da27e83d22dd4eb38c91a5f52d247bd5ad6b45`  
		Last Modified: Tue, 17 Nov 2020 23:40:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:15a2b9735490fdd661dd118b7878b5fbfce5dbb678b7a3a47ccaa4749123f1dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51895147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5062a3f6722ee9ef7ba367c92ae5bd59583802f378260288313584ad1c141b64`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:14:34 GMT
ADD file:5cc0b74720267cc407b6e4f6a0d0d5000b9b65020d0ac589fd1c787cf848c614 in / 
# Fri, 11 Dec 2020 02:14:41 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:15:05 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b71c38c2b8727673d6f36619760e457d5ec964324ef67ce41a36383912590e35`  
		Last Modified: Fri, 11 Dec 2020 02:19:08 GMT  
		Size: 51.9 MB (51894923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7690542d6d5fef443ae2ef3aaf0036f43c33772b55af0d4d0757a17fb06e35c`  
		Last Modified: Fri, 11 Dec 2020 02:19:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
