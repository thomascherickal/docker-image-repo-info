## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:8137f2f38a08b50e94afd26398e2d9762f52f02b1ce0e4bb36d2074d8e7ee3ed
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

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fb2d0990619ed3dc6203f8be4953146175b28e4d5462a08a79a31a7284097969
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120109523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0167bfe7e2deaba2bc8b079ca60aef2926b5bb3937e3744a7d678b871055c263`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:53 GMT
ADD file:be998d04a8927e9c4b105995e3b9d6800ea798807389f7c5921c0f4774328e21 in / 
# Tue, 21 Dec 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:53:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:53:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:53:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b99af5931b39ce167150ad668cfa57ddf7664697be9996cb7e0e6aebbf05843`  
		Last Modified: Tue, 21 Dec 2021 01:28:07 GMT  
		Size: 50.4 MB (50437136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6013b3e77fe6fd3dcf46a05f8e5b3afa9fbca7ba0161c62e56beb4058334dec`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 7.8 MB (7833863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbced17b6899896c8e4016d62c885d737fe667acace2733e17c64bb974232887`  
		Last Modified: Tue, 21 Dec 2021 02:02:46 GMT  
		Size: 10.0 MB (9997172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b609dabefa83fae157bcd42123a8ed45199bb6c301e09a11260c1cad9babfef`  
		Last Modified: Tue, 21 Dec 2021 02:03:05 GMT  
		Size: 51.8 MB (51841352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b624c82adca71338d88787d4c1d62354594755e19cbfde801885479201d138e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114794059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba62813b9112614ec37d00d477e6a0e1d57c23a463de1a580b2f19d0fb0697a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:51:04 GMT
ADD file:8bb721dc246dd73e2e3ceef5631a3d18a8e9e9b00e27322673163926e103af48 in / 
# Thu, 02 Dec 2021 02:51:06 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:40:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:41:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:42:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1593bc232eeb9f23957084e12e8d4be6b14f8a99d43fd93b74963cfca9a24a9`  
		Last Modified: Thu, 02 Dec 2021 03:10:08 GMT  
		Size: 48.2 MB (48154319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde1eb9c743b9a4dd4de997015e976a9fa479480637291cea144feb3cf8b43b`  
		Last Modified: Thu, 02 Dec 2021 04:02:29 GMT  
		Size: 7.4 MB (7377140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ff2d5ef35b41e4618bdbe605c4b67694a9136911e86a2d2c4ea3b2aaea88da`  
		Last Modified: Thu, 02 Dec 2021 04:02:30 GMT  
		Size: 9.7 MB (9687679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613d0fe1a090fd1baeb390040d371d74202bddd665bb9a8be878af8c04a6beaa`  
		Last Modified: Thu, 02 Dec 2021 04:03:10 GMT  
		Size: 49.6 MB (49574921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:da0594d9d7af2299cc382a296c2a7d9ef25bdd109e8dbb8745db72a0e0a791e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109744454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123c138711e369addaffc178ece4ba34f9dbe5ade8fa4d1b982e73d9647aed30`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:05:46 GMT
ADD file:f81ac7bc8750cba292278c6c9352e694325534f013022ec41fb4372853425a20 in / 
# Thu, 02 Dec 2021 09:05:47 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:42:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:42:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 11:43:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2c5d3a36ba44675d774d996a47340758fe658760807ada03e875b485efd98631`  
		Last Modified: Thu, 02 Dec 2021 09:21:46 GMT  
		Size: 45.9 MB (45918126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a599fc167ffc818b08596e6b54e1124fe1bee6e4f29e40795a47d4f16c64caf1`  
		Last Modified: Thu, 02 Dec 2021 12:03:12 GMT  
		Size: 7.1 MB (7125180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6b1bef9db4b6610c293de339defa8042ec5955d79112335739503860154208`  
		Last Modified: Thu, 02 Dec 2021 12:03:13 GMT  
		Size: 9.3 MB (9343672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec09c211e4695ce6890181df80b45c6b5620311d92f75a7028118f9c45aa6f9`  
		Last Modified: Thu, 02 Dec 2021 12:03:55 GMT  
		Size: 47.4 MB (47357476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d960df5afa6b3c223913083b6b7b4f7522b85a805400c79b7840fe8bad6dc1d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118854359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:809ba71d793dd0bf303a81a8ae0c046f5bb58a4871d69c68996ce0f7eac1de93`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:34 GMT
ADD file:73bd5e773b257a6ea5d29845b2b112ebce468878a9467e7c0fe61c69994bb47f in / 
# Tue, 21 Dec 2021 01:42:35 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:13:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:13:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:14:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:741eb94195433e00f9799629cc66740c97d607d6f3ed207e5738995897c52959`  
		Last Modified: Tue, 21 Dec 2021 01:49:16 GMT  
		Size: 49.2 MB (49223144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098cf33298807975a4d84f59f6689e0bf729b62fca9b7320adb80ebeaabc578`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 7.7 MB (7695163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0317c7db28bd6855b787608d1f4236185907b452f6f545a9954be870828af6`  
		Last Modified: Tue, 21 Dec 2021 02:23:45 GMT  
		Size: 9.8 MB (9767165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4301bfae0dab5df877b31fde90c919b02335f783b7405d66b6123acfe03e69e`  
		Last Modified: Tue, 21 Dec 2021 02:24:05 GMT  
		Size: 52.2 MB (52168887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6796e6185a246ca4b1cc836375a882caae3bc75decdf616b42a59a8e66d8e74f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122986427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c6c9ef58b1e4cd4d99a0107e9b96794bb50c1b741bb6d7456f0e31334c81f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:24 GMT
ADD file:4e982be228380a8d7632e31f19e39ed55ee76fb1db32130fa88d696904d6acde in / 
# Tue, 21 Dec 2021 01:40:25 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:15:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:15:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:15:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:342b01a61e0af68dc09681004efdfcf66d0443632988d6f247dd7b34bc18b1db`  
		Last Modified: Tue, 21 Dec 2021 01:49:14 GMT  
		Size: 51.2 MB (51207766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4759b0dba897041c21e226a9db50a85ca5685f19bb5036f16df5b231fd177919`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 8.0 MB (8000238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a258e8ae475665e88b0ebd438d4a945fa152a99c6d2ff863c06087a6dd4c7d`  
		Last Modified: Tue, 21 Dec 2021 02:27:24 GMT  
		Size: 10.3 MB (10340145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7754201e052c276668b8474d86f55c0df401d90074d1090dc57d978ce0be1a2d`  
		Last Modified: Tue, 21 Dec 2021 02:27:48 GMT  
		Size: 53.4 MB (53438278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0bcbc03585a27bddb4521166198954f8ed15c1d752bf4a8ea2314b53aeabcf07
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117194258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d84e97b522b8ff7ab9632602fa6faa9fa729a98bf68ba2aa96fad396a3b14e4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:09:36 GMT
ADD file:095248cbc68568fe0013b4326eccee4814a57b1d78090c33b74fd9411ab2da06 in / 
# Thu, 02 Dec 2021 03:09:37 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 04:14:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 04:15:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 04:16:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db00aa5bb460f25028e8f1293b6a9fc4b7a63ea0c2601b0b4e6f8b9e5acfa683`  
		Last Modified: Thu, 02 Dec 2021 03:18:43 GMT  
		Size: 49.1 MB (49079474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206f7ffdc13eb7bff312d6f81e765e1d28f1ee8e070a3b30065c991cac3dba79`  
		Last Modified: Thu, 02 Dec 2021 04:28:31 GMT  
		Size: 7.3 MB (7253558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b157e08170821b6719a87356a0763ce5361850a3186e5bc290782fc3de7e77`  
		Last Modified: Thu, 02 Dec 2021 04:28:32 GMT  
		Size: 10.0 MB (10016344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687520e5352575b7e49cf2f5c19b24ae437c69f0892a5ad44909efcd1714b59`  
		Last Modified: Thu, 02 Dec 2021 04:29:18 GMT  
		Size: 50.8 MB (50844882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6eca5bb12a5727b9d99d86fd3ac374e89965d8f0b67381592fd4a700ba6f8571
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130641693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8762ff6fef1f187fa73a31d2b548630818d6416b100a657ba7abccd6026fbac`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:40 GMT
ADD file:57b3fb8e49c4d437559f3682edb29b342dd97e4913269a33c178d9eadbba9abc in / 
# Thu, 02 Dec 2021 07:21:47 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:20:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 12:23:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e863e86537b5fca0c122c393c3cc05bd29095cfe10c60ec14e3024f0589df622`  
		Last Modified: Thu, 02 Dec 2021 07:32:11 GMT  
		Size: 54.2 MB (54183785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2269f1f2efe213e4295dfdab761d80dd9b1ebe099a1d7a12a142c23b7d014327`  
		Last Modified: Thu, 02 Dec 2021 12:56:19 GMT  
		Size: 8.3 MB (8272845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e56e0ceccb67a8c0971b09a1ee18b8d3ebd483e02acac944c568b66274be2c`  
		Last Modified: Thu, 02 Dec 2021 12:56:19 GMT  
		Size: 10.7 MB (10727737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f92bacb2d9316be25198bd31425e4da0864b497f7c8c3efad8be29979d09fa`  
		Last Modified: Thu, 02 Dec 2021 12:56:43 GMT  
		Size: 57.5 MB (57457326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9f3213860594aa2427e86f93f0f516bda8b96fc10d97b7ddd3bb3df5bc5d1fbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117670197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3c72dc161b766b179cb43858d5e3721736ca63c3ec5dacc964f3298a9852c87`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:39 GMT
ADD file:def95923e24cb6059ca87ed32edda32704debf3cdd64fb6c50e156b7528dce0f in / 
# Tue, 21 Dec 2021 01:42:42 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:10:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:10:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:10:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:506fcc46017f6aa41ccd20bb2ea02ae7698abd4e52104cd94243f7aa64ce5ee0`  
		Last Modified: Tue, 21 Dec 2021 01:48:31 GMT  
		Size: 49.0 MB (49005442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772d29bde24f2fb280843cce37b4d501dc938c6dd3a0d7b773ddfa9d88436c8c`  
		Last Modified: Tue, 21 Dec 2021 02:18:25 GMT  
		Size: 7.4 MB (7401365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c399d86e51de8a9246ca00799d46792b4022f28a3eaf98791e69f39047566f38`  
		Last Modified: Tue, 21 Dec 2021 02:18:26 GMT  
		Size: 9.9 MB (9882996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90037fcd44cf83c4b37c676c05e2c9d1594bc8eb2efbbc73b8d78836f08eaa8`  
		Last Modified: Tue, 21 Dec 2021 02:18:39 GMT  
		Size: 51.4 MB (51380394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
