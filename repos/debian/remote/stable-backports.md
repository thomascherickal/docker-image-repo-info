## `debian:stable-backports`

```console
$ docker pull debian@sha256:f5edf1107dba5904ecc6b054c61c7f74ecaf73e87e71a38f680d5d725621e449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:d1b49dad5e1f9d53c4ecd98aa851c2dd9b64647637962f0364282d6fc48d8150
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50380013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7472ad6f2b369cef4062ef7041a60f6dd101b7ae2a3178e97cd928294c3094d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:01 GMT
ADD file:fbb4b2824d1652fdfa126a9451a32a6719ab396382f8dcd3cbed30fe82d59431 in / 
# Sat, 01 Feb 2020 17:23:01 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:08 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:281d7b89dd603273dea4d125d49c60138d29ba73bbcaa03529da79d25f5d7418`  
		Last Modified: Sat, 01 Feb 2020 17:28:17 GMT  
		Size: 50.4 MB (50379788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37710fcddce5df7fe92a8c9645161be581c0b173714763a45a22a9b16d0f9d7b`  
		Last Modified: Sat, 01 Feb 2020 17:28:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:198cf564a89280ff178c754db0d34bc7131de9bedb54587ddc2b9b5e4252f3bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48093148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a7a2fd8753801538c6186b6da537a4fb5cbfcbff2fb2c6874df35cf4d09c60`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:53:04 GMT
ADD file:af3acc7fcf4055fd890f3f8f9885c23ff868d7c7a4e19da0ef6449ba5a7d245a in / 
# Sat, 01 Feb 2020 16:53:06 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:53:13 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2ee893b61f2f93bc84fd6d580e90b0610df96a724bb3cbb434f14536f57f1190`  
		Last Modified: Sat, 01 Feb 2020 16:59:54 GMT  
		Size: 48.1 MB (48092924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148cbcdba5fd674aaa2813784114c7f65815efee33b6666342c006e6ab6a1d4`  
		Last Modified: Sat, 01 Feb 2020 16:59:59 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:e0ad9bbd0ca2d2e86409c4e277b84678ad56c44f45bb2bc2ec3c9c1649553b55
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45859922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3e69f469bfa9d984e21d302e5d8021553c3c53e325c72f06bf9148ff53a3ce`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:03:27 GMT
ADD file:a3edfad9f83c7a182b73290d40e6f5f6ee94a8a3e8b81971719a67208d1bce33 in / 
# Sat, 01 Feb 2020 17:03:29 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:03:35 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:57662fc8a1279cd8d42f3acdc7719cf7c7604a2e2397a4d75127230a2993ba42`  
		Last Modified: Sat, 01 Feb 2020 17:10:20 GMT  
		Size: 45.9 MB (45859696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7ecf0420add3af4c9ddc92d4317387820273ba36b6370be1b54de1a1762cfb`  
		Last Modified: Sat, 01 Feb 2020 17:10:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:7d23975adbbbac1b165bb9573dd153c65dbd8e3979c8243b5ed974002d17432d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49171936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ab979d8954cb51dbb53756797fc842959c9e02a0599af1c94afcb70961f34bf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:26 GMT
ADD file:db14bd80b506e5e1754a5e84f5db0a7e53b9fb85d8b6918b381de8f213538b2e in / 
# Sat, 01 Feb 2020 16:42:28 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:42:36 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fab170ceaa7d371d5a29b424744b1b61c4e7b546843bba74ded687d59ef8cfbf`  
		Last Modified: Sat, 01 Feb 2020 16:47:47 GMT  
		Size: 49.2 MB (49171714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f195d81e85bad9a889e854708c0689c8ec939736af187835c976f0417d89bdc`  
		Last Modified: Sat, 01 Feb 2020 16:47:52 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:cc20367dfcb3b7284d92acea3d0cb699768ec464f5b950c7edb05aeb14bdbc99
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51142191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ddebc3ec4aa32930e80a87573e7df16e6297aa992eada0a412c4b08f69e32d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:23 GMT
ADD file:484c6bc4e22632a315ad74ba6d46a0b7ba7eb019aa909d53e2ad85f8675a084f in / 
# Sat, 01 Feb 2020 16:41:24 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:41:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:eb87d2782b05f8264a824dc4cd626db163bd667f8031bda04ba8df640e20dd76`  
		Last Modified: Sat, 01 Feb 2020 16:46:46 GMT  
		Size: 51.1 MB (51141970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83c74b6ac480f652f0b6f04f237462d5526fc6cfc5bb747cb86ee3f878f5eb4`  
		Last Modified: Sat, 01 Feb 2020 16:46:50 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:3da086c872892b043c6ea0a88d50c735fe704323f6bce2d4cf27869b5f68c1b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54133018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2493b237270ac141d15aec89f28e6b3741884604a2d875debe6f88206f8dec5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:19:35 GMT
ADD file:48cf5f8fcdcc66f1e7fcbca9dff8e2f9c0c423abffe93c54d5c3364c7dceb666 in / 
# Sat, 01 Feb 2020 17:19:40 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:19:48 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7672ed36d18a19abdfb622589d848bf5e86f152ec96a8c45cfee133912d67987`  
		Last Modified: Sat, 01 Feb 2020 17:29:36 GMT  
		Size: 54.1 MB (54132792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd54aeb19cff53b4008b2d33ba9d9493c66f39218b19253c51a2e6da0bda8a1e`  
		Last Modified: Sat, 01 Feb 2020 17:29:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:0ed5c399d48a5929008bf025f1dacc72edf14afb82a82530c1b5b3f85e51b227
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48954765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c69c435d3acc444042a1df9db5c7531445dba573f20e8bade789c1ed20e7b5`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:f1b2c403706afe69d0fa1ffc3352dfb895c5f44e1d96f5f3aeef7e139f00f916 in / 
# Sat, 01 Feb 2020 16:43:22 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 16:43:27 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bf102728221bd20f35cf914630a4f7230b9ed357a1f04b705ac604e45fa97d54`  
		Last Modified: Sat, 01 Feb 2020 16:46:53 GMT  
		Size: 49.0 MB (48954542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee22eb399b0fb952fddcd37a2878900163578cfcbd4e330b5211c06c2ea027a`  
		Last Modified: Sat, 01 Feb 2020 16:47:11 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
