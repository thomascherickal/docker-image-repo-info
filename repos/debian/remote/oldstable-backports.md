## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:c6ffe338594f6d7abf6d9553a82e23284f4ccf0f219504b1051dd5e2aa6a3018
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:d32ca74a09f416c806bd224e56429bb8c12699ff778999c30de50b2f2846824c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50441340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:decdac11e91c9a8880624f290791840224d4eb182b3c1fa4d0416fb6bb1976be`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:11 GMT
ADD file:3d94e1c36b68699eb36acdde63a56bc6f9aed18856780b55a6c8f1edbbe47997 in / 
# Tue, 04 Oct 2022 23:27:11 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:27:14 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ebb5c831d3e09c6e4f69e2abf7358677daed502a3473128d7b5d96e209279e2c`  
		Last Modified: Tue, 04 Oct 2022 23:31:58 GMT  
		Size: 50.4 MB (50441113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c13568f5746e73b7d4dc10943557b27c64487c0261c95769136600314b6541`  
		Last Modified: Tue, 04 Oct 2022 23:32:07 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:d43ab4b57345d432c3233f70a07a5859f9267fba028e9c8ca1dbb717ca120814
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45915174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6fa838f8fcfac9554ad7a98b1ce6608fac6a7e658212edae4fe0f835c230111`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:32 GMT
ADD file:b4a6d01562e23ba618ef6fd98895784f112241404069c1b0e47faa8a21e46f5f in / 
# Tue, 04 Oct 2022 23:59:32 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:59:38 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7409878a6e8072e252dcee5620a4a01e7cb0ff5db6b8d336bf20e960085ead33`  
		Last Modified: Wed, 05 Oct 2022 00:06:28 GMT  
		Size: 45.9 MB (45914950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911593a89ae4e5627e354d1946264a29788cc7a5ba49ccf7bdd8a3b5945c253c`  
		Last Modified: Wed, 05 Oct 2022 00:06:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ac8fa46e9ac5d85d16b8e1a78456cefebb9944b4f519ca3e0121915f62faef63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49229088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76127c128d286fc847d4c4c0a832081440dc74c78b412d1ff3e9517fa90e7492`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:22 GMT
ADD file:b52dee81f9bddca289cf47aea9d4a4e29e685894c8c75b997e507862c36da52f in / 
# Tue, 04 Oct 2022 23:45:22 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:45:28 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5de3e49ea1c1676df95c2f1e0df1cedc8b8eedf184a3aa0b5afcf188e6043da2`  
		Last Modified: Tue, 04 Oct 2022 23:51:37 GMT  
		Size: 49.2 MB (49228863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5846890602b8cb6c6748989552b97a4cf57188ecc57d431d87c1dcfad50e55fc`  
		Last Modified: Tue, 04 Oct 2022 23:51:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:b317ce21a2bf192a38d32d9799dac4797765886fc1c520099c3d4c9548cf72c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51203041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:481051ae4a4040f3edc1e05825c45cf8ca6023dea05f557865c1e828fe850a4e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:21 GMT
ADD file:d11a78d8074261391716b872b4dc5973bec57eb307b0216de066efd2c11fd04c in / 
# Tue, 04 Oct 2022 23:40:22 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:40:28 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:eb59cd87b868fc239d88ffd2373d583422d34572ed5a958cd78614077a9a50dc`  
		Last Modified: Tue, 04 Oct 2022 23:46:49 GMT  
		Size: 51.2 MB (51202816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464b3481ebc0acf58292d05b56a69f9ce9b603282bd03196c9008dd7ed6b136f`  
		Last Modified: Tue, 04 Oct 2022 23:47:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
