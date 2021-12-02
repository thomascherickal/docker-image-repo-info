## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:2300ab1de76f954889afc8847578477e70c4b232bb020dc17994b180ccf1c727
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
$ docker pull debian@sha256:cb37b86bbe2ba86b56a5c7203c87f1e6f01dd0e00c569b40ccc51009e6291b2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42117111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e2ce471b56e3825aaa732f5a4be369e4b8ac48246d4182caf19126e10cc45e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:01:14 GMT
ADD file:9fe034588d3d2f104d5aeabbd50c5962d6eaca10ab66ca53a733c09c2198092d in / 
# Wed, 17 Nov 2021 02:01:15 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:01:28 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b09753a0fa5832cd6796122a4aba45a3ed13f0371593065aef0ffef747c6030c`  
		Last Modified: Wed, 17 Nov 2021 02:17:25 GMT  
		Size: 42.1 MB (42116885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08254bee10751f58926233ae8599c4b0b561e99ac1e45446d67688ecb984055`  
		Last Modified: Wed, 17 Nov 2021 02:17:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:8fdbfa45bd7a8726650d2d9fac77131deb41faad7d7688b6968eaaab7377e5be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43174701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b06b908f38d2799d6c6f591f9b1a1980354bb617845ac1039dc41714d571d25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:55 GMT
ADD file:7a50bbd1118cbbcc95d6c4e1ae912bab0503d10209cf27e88bd7241a76390f9b in / 
# Wed, 17 Nov 2021 02:40:56 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:01 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:08e624181b9f21c13fbf44c78f84881aba565b51554e1bae8e119c729bd3d356`  
		Last Modified: Wed, 17 Nov 2021 02:48:29 GMT  
		Size: 43.2 MB (43174476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02842259569577bd1aed1ebb82de30ef678f78e4477945e85d1411807e4aa19e`  
		Last Modified: Wed, 17 Nov 2021 02:48:40 GMT  
		Size: 225.0 B  
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
