## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:648b87b1606615ecc29c3235ddd93e2f7728ac960e8363181c907f80906ceca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:cc966d558163b2c444e75b9f98f82b9ff3937ebb3197e77783e9e929bc373136
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50447986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524292ee0b4e17fa1f18838b052d0c780295ce929da220ec105ceda9703913b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:21 GMT
ADD file:326adf2063d8d292211a8c3f1b0ed03faeac6ac47a2bf31c02c22df04e81a3eb in / 
# Tue, 25 Oct 2022 01:44:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 01:44:25 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5c3cab76daeb46f383600922bdc00d7e2095afa471338147c1901af943ba4792`  
		Last Modified: Tue, 25 Oct 2022 01:49:00 GMT  
		Size: 50.4 MB (50447761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888e60dc9add3193c2ae715a89e232822346e2a800d7cd75e237f4fc26fe4bbd`  
		Last Modified: Tue, 25 Oct 2022 01:49:16 GMT  
		Size: 225.0 B  
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
