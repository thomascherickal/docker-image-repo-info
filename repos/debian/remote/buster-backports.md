## `debian:buster-backports`

```console
$ docker pull debian@sha256:c6c760d11a20cc0dd5a4db46dc442e423be46a1edda1cc1b3d832a73162e506a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:19b57f3c28b7bf5881244cac08971c3c68ca9345173efcd10b1afaee40e73bc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50440597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20db46d819c66f4131ef33f59cddacb0e267bcc1fd6bbecbab928cbd5a1263c5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:38 GMT
ADD file:4649a893b2859f2ff51182a13c9c8eeaeaea866161b3f4a1c4f0bb48bc01d007 in / 
# Tue, 13 Sep 2022 00:56:38 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:56:42 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:86467c57892b6bb48d563cb5940c68b69c431b2e79c3547df60d1c761c21c156`  
		Last Modified: Tue, 13 Sep 2022 01:00:51 GMT  
		Size: 50.4 MB (50440374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde92056eabda90361e2ba789480d2522d5a66be24614cb17532dec10fbb1352`  
		Last Modified: Tue, 13 Sep 2022 01:01:05 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:9cdd4514104e9229bbcb03d4614c184b499e6a85dc8bcda04920db93dbf832fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45915162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40a1a6a79cbfa54e1946028f5b1a7e34f8d48356bc0a0b74b49f3c4693c0f165`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:18 GMT
ADD file:f02e7759ba5d55ff457d421191df7d2973666205453bbb6755214288b1c5527b in / 
# Tue, 23 Aug 2022 01:43:19 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:43:26 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e43c24e08caa0d5875ad9b74a9503702850e39637c5dfe8cf2b231adfb60322c`  
		Last Modified: Tue, 23 Aug 2022 01:50:31 GMT  
		Size: 45.9 MB (45914940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ef2aca6c2446a83d1560f96c63eca229a7619dd47b60210b3c562ded0303db`  
		Last Modified: Tue, 23 Aug 2022 01:50:48 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:1b7101656e10699813b6b0f450827567460790c3e66a8c9fbe34600467f26443
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49228290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55333d7611fe01df5357bdd35cf6a93b010b587496fd3b132f63e348fe064461`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:43 GMT
ADD file:a3ba1802e6680a14c605fbe754f9fb56a642f0799f51ce0010d253cb66c9691f in / 
# Tue, 23 Aug 2022 01:52:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:51 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3332e5c67ba650c61dbca801cf2739a1f5b6faac33f7b0543f97f4ab1165fe69`  
		Last Modified: Tue, 23 Aug 2022 01:58:23 GMT  
		Size: 49.2 MB (49228066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0610e83ae1ee34ad5cdd950d17d92a2fccaa4da9589a73a114d463ce6f2101e2`  
		Last Modified: Tue, 23 Aug 2022 01:58:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:3f2714f51b0706a2f1b2364433f9e50c5b706030dff77e2b249b62061416e429
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51203156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7bb47641f113a3c016d084942457b96f72c33195801432fbe11cbef60d70036`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:51 GMT
ADD file:7ad537f8110f70df174d79a50cbe08fc480933797f0717e94529061bbfd00759 in / 
# Tue, 23 Aug 2022 01:02:52 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:02:59 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f73bf17b8a4e28cf438c1af60c558d4943ab3fea50a934b856e19e18b2cefc70`  
		Last Modified: Tue, 23 Aug 2022 01:08:52 GMT  
		Size: 51.2 MB (51202934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e67396ae923eb2ec5769b79e9f8bb7d9d9544f972ba7c9c8350116be5c6e86`  
		Last Modified: Tue, 23 Aug 2022 01:09:08 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
