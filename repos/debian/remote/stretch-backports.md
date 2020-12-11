## `debian:stretch-backports`

```console
$ docker pull debian@sha256:cc292e05fc707d82f0e4a3d57d0cae44b78b125acd898e7f8bfdff2f94030771
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:stretch-backports` - linux; amd64

```console
$ docker pull debian@sha256:295d3b7387ab8ed0e894e3983b002bcb62d93e0d2c0e83ba82af8624368e2ca4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45377831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8189c3ec092d80176da79c0180c5614bb45ca8bdc3dba488d4568a430f00a822`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:08:48 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cc8d678b6176945c416287541970f8694c2d057ef3fa8e5caf4c5706170fc7`  
		Last Modified: Fri, 11 Dec 2020 02:15:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:c20e0394e1fd6e49eb02f80952b5557a5eb7820bff30e42835e05c1caa58c434
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44089822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2359ce44a9d46e3689e64b70aeb1242d0b458672a8b8b6cd5f7f4eca9eb62981`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:23 GMT
ADD file:ecf2c81fa53759cae3e17b1b743a884b747d5d2b2676bb7f14bdb4fb1a5cb38c in / 
# Fri, 11 Dec 2020 02:09:35 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:09:50 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:74944684cd609943dde5912069d99b50bdb10f0cbca3bc5f96b0b17fc41f8c18`  
		Last Modified: Fri, 11 Dec 2020 02:18:35 GMT  
		Size: 44.1 MB (44089598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ec90bfc6f97072aba8ce584e221d07cba8122464330a5960cff85acfd3102`  
		Last Modified: Fri, 11 Dec 2020 02:18:52 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:c1bf144beca7dec666bd2ea1023e7819aea0cdfc1fef71f34e4e6eb457aab04c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42118175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:311b520a5204e58687c9d5a9b00613c234093824e85ee1b1a50a64aa70877634`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:28:06 GMT
ADD file:e74dce76704e3faa6198db5cf4192fd431f5addf55f658277eb5b60d254fee8e in / 
# Fri, 11 Dec 2020 02:28:09 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:28:19 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:062f5403576d7e3aca1c92115ff0a9ea110b270cb0b61013efa86744515666fb`  
		Last Modified: Fri, 11 Dec 2020 02:36:48 GMT  
		Size: 42.1 MB (42117949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc851b10c29c2fa9b500ea87ae3de2ac3a0449f1015fd1a02d67c0bf558cd01`  
		Last Modified: Fri, 11 Dec 2020 02:37:00 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:2b15c4e861d0e9a5e717bc0343d37b94bc616fb4f8fe3636c37bc107e4242401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43176165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c990962c4766d53b8b8e99a95122f246cef070ac58fbcfb8312be38c606c06`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:16 GMT
ADD file:48e44714f486662ed380343e556f0f7411bd6600d916440063753c55d1f94b45 in / 
# Fri, 11 Dec 2020 02:48:17 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:48:29 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ecefb91918e846819df74a1beb8e41f454bef156738373818c20656a3a46d5f7`  
		Last Modified: Fri, 11 Dec 2020 02:55:36 GMT  
		Size: 43.2 MB (43175941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d162bf6df649b8a4b57177887c1221bbe041a970c62ef4d2692005a404366c1e`  
		Last Modified: Fri, 11 Dec 2020 02:55:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stretch-backports` - linux; 386

```console
$ docker pull debian@sha256:e8a7cac84d2357f580ea294f32b99e4709d78fc5d7c0ba3ba11c87120bd7e8a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46095339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb29f313be63e899f15d41d4f57ed8484e1feaeadd7c8e31fd41ebd04402ee4b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:38 GMT
ADD file:65da710638e196cb40b07b1d2461114bb3c8b34d69693449a905397c192f1ac0 in / 
# Fri, 11 Dec 2020 02:05:38 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:05:44 GMT
RUN echo 'deb http://deb.debian.org/debian stretch-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c6c30bba175680710c6b02f65235cc2a0b8adf1ec4be1e440e260afda9487b37`  
		Last Modified: Fri, 11 Dec 2020 02:13:22 GMT  
		Size: 46.1 MB (46095117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a128f4e7f74045abf271ae04ebcac17d7a3b2093d1b4479b398546b5b1f31f5e`  
		Last Modified: Fri, 11 Dec 2020 02:13:30 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
