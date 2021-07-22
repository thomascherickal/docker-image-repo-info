## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:ab89dc65b011974ed4a72c195dfe62ddfd232b557222f5ad41de57f71c1099f3
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
$ docker pull debian@sha256:07448ce9e4dbb93395391792817d1384b4b5725c68ccb92dcc9ef480fceccbc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54905075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34abe48ef120834131eab0a671412b7811056b870a5bd6c2d105fce74ad56d19`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:02 GMT
ADD file:fca2ea6b8fc69f3efb8a2f21cd3877d23a9ee3fbeee6ebe4fe21541cd1606a8c in / 
# Thu, 22 Jul 2021 00:45:03 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:45:11 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7a72d62e9d2fef13cf62e5d212cc6a3751b5c388cc6657bebf4dabc0ca3603cb`  
		Last Modified: Thu, 22 Jul 2021 00:49:21 GMT  
		Size: 54.9 MB (54904849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4170a018d3cf41bccb15d1bb87956bb75bbaaf1bb4459e822e70f5d244373a`  
		Last Modified: Thu, 22 Jul 2021 00:49:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:805111c9c6f63c8372c8bf2001304a3614ab66813d56dbbad31d463a26dc79e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52443322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7ac23d4e78d3dff137d0a4ca5cad453617e1f5ddaf72e618544fe21304e8e3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:48:40 GMT
ADD file:a5e191f39728e6e12b8f32edbaa7920930ceeaa50bd5db8a28faa1325a03c877 in / 
# Thu, 22 Jul 2021 00:48:41 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:48:52 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:54f61193f2822104b288f4b662f2a516401b23e0fba11d7ca2215f06378c96fc`  
		Last Modified: Thu, 22 Jul 2021 00:59:59 GMT  
		Size: 52.4 MB (52443094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013cf9cad76bcaae86b8ead1fd49578ecd7c97fcee7bf87aaa36bfb211f82f9`  
		Last Modified: Thu, 22 Jul 2021 01:00:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:730dc4b877861722620c557f2aa9701f638f28dbf72eba9000c1027eaa25f34d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50107857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f744e3726aaf0a6fe2c0214e7c4822e65bdd53ac144941efed671166c9ae08`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 02:02:14 GMT
ADD file:e95bfea309b4c4cf7a3a7367d3a3ed606af0f897282dd0e3e2effd01a126625f in / 
# Thu, 22 Jul 2021 02:02:16 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:02:29 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7b19ab02b95dd8c04699b4e2ac6ee9898e2f6813d01c5c529b1e3f2dd356d20f`  
		Last Modified: Thu, 22 Jul 2021 02:14:18 GMT  
		Size: 50.1 MB (50107629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1a3181b67e386e3c2c8e407e9ab7335bb6ec281b8e70036eadc51e8ef0c0c`  
		Last Modified: Thu, 22 Jul 2021 02:14:30 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ef757564840e136d4230444f9a700df952483c5fc4838f3347999f56180a91ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53590585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005fafe4b24648ad6358dd8c0e70779d128afa38dfa0e3211baf38f5f9d2ea9e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:37 GMT
ADD file:6733d7f2201aa0027287de4f81a7cabfb79c331e290d9d1f16bc68c8c0ce1473 in / 
# Thu, 22 Jul 2021 00:39:37 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:39:43 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a2fd60d6781333dbb2e2b453027f2c16737edf4afa6edc775fbe4983c9196c83`  
		Last Modified: Thu, 22 Jul 2021 00:44:34 GMT  
		Size: 53.6 MB (53590358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ca972476293c7de3d8b79dbd5357b5271049d9255b236c5fbe9aa4406819ac`  
		Last Modified: Thu, 22 Jul 2021 00:44:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:97c1dd93a7cf55158d4b7131c283446f10f58d1c06147da0ec2e5506aea79007
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55913253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f412d23d15b668d21592d8c84c894fc5010caaaf80d7d6d1a1b6e9bf19dba2d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:03 GMT
ADD file:24be74cbcea25ad750bd1443d9a3d411e145c2d8fb89605daa62634bc554c881 in / 
# Thu, 22 Jul 2021 00:39:04 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:39:10 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a83a0aff5ff3ee06144cc6d7633ffebc95f68ca4314072841360b93f72a8c906`  
		Last Modified: Thu, 22 Jul 2021 00:45:06 GMT  
		Size: 55.9 MB (55913027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b71564a720d829f00116f38a576aa853245516e9f17130bd1d2293d4187eb1`  
		Last Modified: Thu, 22 Jul 2021 00:45:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:d385e826d109a74964b53123ca08bee7bf4ccf13354b0e3d490943cba7bd2801
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53156514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc6406fe82a40d9919f51751702578174582d65f09bf04ef99a21e465e4d9fc0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:08:32 GMT
ADD file:0528720276c3b3b11a00595363f8a514e2655bcf1e4d9b8ba3f79621e44f0460 in / 
# Thu, 22 Jul 2021 00:08:32 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:08:41 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cf851126a635ad4c2c2a139ad19f922e1a4ce737641a782c32519868f02d804d`  
		Last Modified: Thu, 22 Jul 2021 00:14:07 GMT  
		Size: 53.2 MB (53156287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829c903d84f2fa80707ba5d7aed00cc9bb70549f4e99f4037edad84770388127`  
		Last Modified: Thu, 22 Jul 2021 00:14:17 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:d17c53cb37375c3136b61ddbc2267b0d0fb066bfbeb759e27b799c5b1a9ba173
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58813543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb4c57dd0547b9bb5a3a05f11afe4294201c8a8576bb72cfcf23a09cb9eb2c81`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:17:09 GMT
ADD file:aadb38c47e4a40c11e7ad3b380075dadabb62c20584e02f089c2e5c957ce04cd in / 
# Thu, 22 Jul 2021 00:17:19 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:17:40 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c0acfc4b0736fe9b7465e9b5f83f277c5a237585bf07da22048883229ecafad7`  
		Last Modified: Thu, 22 Jul 2021 00:26:21 GMT  
		Size: 58.8 MB (58813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86a630858a62f1d38af0debc1a375b9f34ba79c4e4437f537f65bd107aec8c7`  
		Last Modified: Thu, 22 Jul 2021 00:26:34 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:6fe4f579ab000c5f597aa2b02e524be0f8cb21ff4481aa95e43ef350e374b85a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53183780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cacbc2cd262007dbbfbc095a4878480c974b46fde24c19bc9a1e855ad55b8f44`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:34 GMT
ADD file:0a2fe191e4bb0a90f32a0829f6d49407139fa2c3517cc2097c51a94786075a8e in / 
# Thu, 22 Jul 2021 00:41:41 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 00:41:49 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:431c45f9c46bd0833127af2c090d5f6776b5c421df2849de5f3071102212923c`  
		Last Modified: Thu, 22 Jul 2021 00:47:15 GMT  
		Size: 53.2 MB (53183556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc51181c8ca607ba600ac713c87beea2240d068ab2a36f6e3768b077e796727`  
		Last Modified: Thu, 22 Jul 2021 00:47:27 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
