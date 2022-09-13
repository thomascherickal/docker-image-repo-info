## `debian:oldstable-backports`

```console
$ docker pull debian@sha256:1dba6d06c98af3a58bfd0cdbfe710df25e6f820772e081db0a3fab7a8cd4a278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:oldstable-backports` - linux; amd64

```console
$ docker pull debian@sha256:950f772a83d9b163308a2cf34f1a9804b324e968a46152969da43832f20e68fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50440602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a741669898e8a2911e2674b401ac93bb880b33810826a03b6ac13844aa827357`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:57 GMT
ADD file:ee981dd66a540953de72a5a2eedad3dd86c907140a949981cf8f3a879584bee6 in / 
# Tue, 13 Sep 2022 00:56:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:57:01 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:26cf2e88423366fb12dd62fce8e546f7debcd8109023d26952a00572917dd10e`  
		Last Modified: Tue, 13 Sep 2022 01:01:36 GMT  
		Size: 50.4 MB (50440379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039790036087637f4795fd922b4b4cd7bc1db5169cf3746b9c35b26379d8bff7`  
		Last Modified: Tue, 13 Sep 2022 01:01:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:54516bf9019321d534e6b3f86db5132181ed323c5234ee9c2792eff7f0213f3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45915198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3a8e67e45eacd806a20b68a30fefba41f464069e091dc565f98c12e9d77765f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:55 GMT
ADD file:b0aff8d83a8a3da12cb618c8b48a31499970722aa53e2a3d079b900406a7415a in / 
# Tue, 23 Aug 2022 01:43:55 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:44:01 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3e0404797f1b5f037fd0b5cc761f5c658a141dee1981c872264000da8ea611ea`  
		Last Modified: Tue, 23 Aug 2022 01:51:25 GMT  
		Size: 45.9 MB (45914974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4589b52e62f4527cbbaac6f43be8174e36547ff65cd03334aa275418c756a45d`  
		Last Modified: Tue, 23 Aug 2022 01:51:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:a024d95d810e67d89c895e6e84672350ed8fb3747f7ec90c62fb4dd9b875d42b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49228288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:859fd10c72ce1386387828daae987b7ccad0b31f1904a2a17fa45119d3f927b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:09 GMT
ADD file:f835872a7a5100d5ef97d0f21ca6d1f2fd1b49dba8d54f3c4c66b649e9801d1f in / 
# Tue, 23 Aug 2022 01:53:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:53:16 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0d621ff8dc2eb254f381e58ad811795387ae8515b65377fe95a86e086047bcc5`  
		Last Modified: Tue, 23 Aug 2022 01:59:13 GMT  
		Size: 49.2 MB (49228065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b34bcef51040adee397f1b8b21614e94f112d2ce2c1f3123e6928af736742bd`  
		Last Modified: Tue, 23 Aug 2022 01:59:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:oldstable-backports` - linux; 386

```console
$ docker pull debian@sha256:40a51774ceb752c7f8bc80a96cf2183d75ec13093913128d7497e1f3b4955e9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51203167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b93947afc8f985479b1fe9b1a1db907a51ace8c937c0ccc7c99cb1909df24c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:18 GMT
ADD file:655a5a9db78e729514b5c9540a63e455f7f7155368767dcf27ea88f9770fd8e9 in / 
# Tue, 23 Aug 2022 01:03:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:03:25 GMT
RUN echo 'deb http://deb.debian.org/debian oldstable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ab1e70384b9110068c85ecac341ed1f98cc3efbd0cd1bc812fb9d9cd9bca4813`  
		Last Modified: Tue, 23 Aug 2022 01:09:44 GMT  
		Size: 51.2 MB (51202943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412fc271903a041b4bc83778538b9240f2255fdc11a1b80de49a18e0d1b3c0dc`  
		Last Modified: Tue, 23 Aug 2022 01:09:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
