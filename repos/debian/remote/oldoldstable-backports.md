## `debian:oldoldstable-backports`

```console
$ docker pull debian@sha256:4e1354741ec3e334916610d7f8af9763e9acd27fea30d82ce017fa8422da5db4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldoldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:1485490640111777c0f1998e3680b779ee50f566af86c8e54a7dd615a5eecbfe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50498222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76c07cdd7c99fdbd5dfaa95156f4d640ab72b30d18756262ff4481caff2414db`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:40 GMT
ADD file:5904548c7cebe86d8cc57c026ace74b16641c827ffeda42b583579ab4eeadc10 in / 
# Thu, 27 Jul 2023 23:25:40 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:25:44 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:58ca768125d9edad02f86eabe3a91bb7f738e885db5f548309dc4032244629aa`  
		Last Modified: Thu, 27 Jul 2023 23:31:08 GMT  
		Size: 50.5 MB (50497992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dedff65ab1936132ab2c7898e06c60efeb85df4b6ebfcc4af9bf7e3a0e2ca2`  
		Last Modified: Thu, 27 Jul 2023 23:31:17 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:e4782959639583bc3759c718c711d33e2aeeac01f2d475cb02606321047517b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45966434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd6f6d85e49b09554579c47808cde7a8aee3a08a80a1cb938a7adc1560b3632`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:58:58 GMT
ADD file:ff181fb8e7b3bfe42b3ecfde7d330ed92beb69bd17a23b6fb44d4d1099529d86 in / 
# Thu, 27 Jul 2023 23:58:59 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:59:03 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8a2da13915ac485da0fe0627bbe8d8287daf25ae815c9acf738ce1a100b8d019`  
		Last Modified: Fri, 28 Jul 2023 00:04:58 GMT  
		Size: 46.0 MB (45966204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f2b407fb1b91dfb229899ef8408fde06db4b45839c4a3be164a44cfd5a3fc4`  
		Last Modified: Fri, 28 Jul 2023 00:05:06 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7499de3f0216ce0ab613355a5c3bd857e5a6f1881eeb3eea17c59438b361315d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49291185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:588673c298c1540d9f5b512ff947f502d1d96bcacf774e587d76d4f420e5c1f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:32 GMT
ADD file:652930b08ffd1d8976a47ed7e4ea264b79e2c216bbdb53069fbd9af2dfe4e5d3 in / 
# Tue, 15 Aug 2023 23:40:32 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:40:35 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:18753a02e00a94d798f7f321b3e48c192a039e1d188042a5a2990c52ab5c5b2a`  
		Last Modified: Tue, 15 Aug 2023 23:44:53 GMT  
		Size: 49.3 MB (49290957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b75186aea109c014f21ec5352e16f2be1c6c254bfea9e319151214f07ca929e`  
		Last Modified: Tue, 15 Aug 2023 23:45:02 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldoldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:9d2d3cc1f09ebfc2485db25d89820924d45d6221bd7482fefe53985b57a49811
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51255689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c6ab7b40d38f0347ffbdd0f595bfa7ad48ce39fdfe1b59ec77c10dc9cec8152`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:53 GMT
ADD file:5e5c60db439ac2712e5cc3c01b553d0a0712fcbf936793c0a7e942d7480c148f in / 
# Tue, 15 Aug 2023 23:39:53 GMT
CMD ["bash"]
# Tue, 15 Aug 2023 23:39:56 GMT
RUN echo 'deb http://deb.debian.org/debian oldoldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:77ed33e8d735fc81e4fd83df07b93ff059e1da209645d4ec93fd47938b69bf8c`  
		Last Modified: Tue, 15 Aug 2023 23:45:17 GMT  
		Size: 51.3 MB (51255462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d716e6e1ffd7dbbe286b8f6bf589082b13ecc874730e2cf1d4b28cf4d4dac62`  
		Last Modified: Tue, 15 Aug 2023 23:45:25 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
