## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:1339997b849e8ea3f13e4c2e5510dee9352d848a8874088b49f97f0b5a86fdd7
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
$ docker pull debian@sha256:409e20c0edd33ecd1285dcff3d42d8f6adc5a001df7630c16ffa5634a97cc1c4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45381602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5f7297fd30a9a66f028e2604cf926ba395d1ef43d1859570330506147e3ccaa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:13 GMT
ADD file:d2e687f740a5885da2758286b4ea6cac4376173166f657c15bb648af564e4b56 in / 
# Tue, 21 Dec 2021 01:23:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:23:17 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a2442be161f48c1463b127bdc62cc81b11b61dea1e2e2ef127ea615df038b95f`  
		Last Modified: Tue, 21 Dec 2021 01:28:53 GMT  
		Size: 45.4 MB (45381374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b707f423a4719d7b278da72d414cc831e55327df3fe4e38ab66fd2da4f1c7982`  
		Last Modified: Tue, 21 Dec 2021 01:29:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:f7f677d189e265c48565c8021b9ad2f0e4e3e9aa8ba8cb2f14243876e9e7113c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44092035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0b2d5b1f77f33c779ca3e4dc504c2d105279e19d950e150f899a0783c2e6825`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:51:59 GMT
ADD file:01899ae0edfca717e465cff9457ba9632a63843dd53ccd79d189328618c4937b in / 
# Tue, 21 Dec 2021 01:52:00 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:52:13 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e5d4f913d9c5ce85c81dea9a3a68b8b3574d3140fe74cb1a024e353ca82e480c`  
		Last Modified: Tue, 21 Dec 2021 02:08:07 GMT  
		Size: 44.1 MB (44091805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30608e501232abdeb3d7165235a92ab83d45bd0440dc7f73e337082cd56de152`  
		Last Modified: Tue, 21 Dec 2021 02:08:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:805d9c6d89c3bc4ec6de2edf9ddaa6c483ea60ac5ae6aa9a38ea4314c7dfbff1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42116991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84d9a9df02c0eeacf186f3d9d32387fca813852848927c1b91e1895ea52121d1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:06:50 GMT
ADD file:2c7f4bda54cfdfdae4a314befc1b9a7296fa3a4716d990b9912afc6baf77bceb in / 
# Thu, 02 Dec 2021 09:06:51 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:07:04 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5eab1885f78efd73eeeab13af59a0136f7ba9efbe9af58aa5407e225986e7f75`  
		Last Modified: Thu, 02 Dec 2021 09:23:10 GMT  
		Size: 42.1 MB (42116761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c312e6edfdee45dc552281b41f3a7ee83fbb9d43813548155a5eb5079e57a47`  
		Last Modified: Thu, 02 Dec 2021 09:23:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:8ef465cbce411196477034f9a0aa4f88edeb1346330172fa8b85b51ff31996f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43174011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06676dce234a7d8d8660e89ca07dc49b5b92a87a36b02844bf617c17c2a05149`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:59 GMT
ADD file:491e3a0ea44e1a3f803c046becea18be4fb893a7e0069e0cce5aa27cdee6c564 in / 
# Tue, 21 Dec 2021 01:43:00 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:43:05 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:109fd60c281aeae4939c60210e1ad17d1d0dff1c1258e45e6a156684496e8adb`  
		Last Modified: Tue, 21 Dec 2021 01:50:05 GMT  
		Size: 43.2 MB (43173782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a530853fdb6be7f359b49fb1bc6706a1dbd494706e31f93b709a0271868339e`  
		Last Modified: Tue, 21 Dec 2021 01:50:16 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:f49941a34fd955e5bf767d31eb0c6a31db60d92afbf10afdc265683c5416ade2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46097974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:416b26928e7a1c68bc7051bdb1ecbee12911a560615273bd5d3f7298da9b5b1c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:41:01 GMT
ADD file:9d07d01555cb40d9d71ffb0cdfc81f07c91a703032ea8bfbcbb0a782baba3589 in / 
# Tue, 21 Dec 2021 01:41:01 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:41:07 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1b26f60c651a6e7738b5d390724ae54babc5413cdf591401f32e8ee0b97e9c01`  
		Last Modified: Tue, 21 Dec 2021 01:50:14 GMT  
		Size: 46.1 MB (46097744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b69711856f8e424d967b596d6d8bd926ffc97de19b635815f67314d82c5b7a`  
		Last Modified: Tue, 21 Dec 2021 01:50:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
