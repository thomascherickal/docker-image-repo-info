## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:fab0d74459e4ad832a2d414d7e97a51995fe7141127e7c6fc4cc0efd185d69be
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
$ docker pull debian@sha256:c78f94d1005e8472ca12fe59889e7106ebf3fa9a7ee2565b7b4dc75e58b5d51e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45381552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16296cda9405218299f36bd7babf76350902df7b1801674279da24ea1976066a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:52 GMT
ADD file:4936c145a88c6d4cef38323effecff9d2ea508ae4ef1e8acec89d608e30adfcb in / 
# Thu, 02 Dec 2021 02:48:53 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:48:56 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5d4c2d0b2125c7fe27a5b4da78da68d4a3ee9a13dfc5f7fcc794f858e24dc358`  
		Last Modified: Thu, 02 Dec 2021 02:54:53 GMT  
		Size: 45.4 MB (45381323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61afbc6af7dc258bc2460a7e95d3c4939c9f3a9d6a217f6bea07c379c5eba388`  
		Last Modified: Thu, 02 Dec 2021 02:55:02 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:cef5f416e69e883d7069bdd103e0cda1d226f8d8a888ca40983148adb05132ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44091951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a94998715d37801c8b88e84e6f3a7ba8a03f1665ec7249a05dc88a60f9e4cf1a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:52:13 GMT
ADD file:ec5c88ead938480e038320db195065e67dec82487fc7e3fed88c1a50a5b732ae in / 
# Thu, 02 Dec 2021 02:52:14 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:52:31 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ec1b2f076054f4da2c34099fd2704b49a61b199dda30edc4ab51bad0842c0862`  
		Last Modified: Thu, 02 Dec 2021 03:11:26 GMT  
		Size: 44.1 MB (44091722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef333df593a67b68d3a0d06d3c0343ccf6bf395de6c88bf4a1dd204525eb36c`  
		Last Modified: Thu, 02 Dec 2021 03:11:39 GMT  
		Size: 229.0 B  
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
$ docker pull debian@sha256:1d091be61948b3682ac204555773dd73d772fc54d23f11f54a877e682079106e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43173957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068e55d9ccb832137cf74d2acf1f127c85fc901bc0501c31c3379e0f69889e08`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:45 GMT
ADD file:c8d29846964db5e39169b0d94989d4a59d857c03fed14a03aa2c1fecd230c8e3 in / 
# Thu, 02 Dec 2021 08:08:46 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:08:51 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ea6ba488d01118326ce3936e5f472b463556a131bde28512575183a637588cd`  
		Last Modified: Thu, 02 Dec 2021 08:42:00 GMT  
		Size: 43.2 MB (43173730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60249d4b51c0c5e4b233aea90aed153794cf33319c871f25634262c0c9f6d11`  
		Last Modified: Thu, 02 Dec 2021 08:42:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:e1e33da8aecc0d220372b899415786a7498350b30e078b7ad501cdabcf370c39
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46098109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80ed0c56abafbf205ea6715bbf27987668c7039693053d229e070b727c882280`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:40:38 GMT
ADD file:7f4efb948dfd5e8709d59734c33dccfdc6eed9a05ab3c38c1fc1d4f77e759c06 in / 
# Thu, 02 Dec 2021 02:40:39 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:40:44 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c0785bcfb4273ebe4098782af34b666ced8d70e867a2765fa042e79fd3b2eb60`  
		Last Modified: Thu, 02 Dec 2021 02:49:29 GMT  
		Size: 46.1 MB (46097880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ac0781be9275beda93c8a07c155de9a0b966c6010587dc86df172b0b4ee5e4`  
		Last Modified: Thu, 02 Dec 2021 02:49:41 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
