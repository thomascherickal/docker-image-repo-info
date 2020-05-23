## `photon:latest`

```console
$ docker pull photon@sha256:fbdae32f534858727fa855af8d548dfa5d98872ef81f466790f7c302a46e8384
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `photon:latest` - linux; amd64

```console
$ docker pull photon@sha256:9a86b203ed75e5439fb770473e94fda6aaa5ac9d103b0b52ad700f8ab6475818
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15167752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0135244847f59a2a8cbb62b2d11bb759a976381952c4999bd110e6b521bbc21e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 23 May 2020 01:30:10 GMT
ADD file:0d11f538a785fef422a09a6576a7da9c315f0e6b608b8ac67b927038da2514fe in / 
# Sat, 23 May 2020 01:30:10 GMT
LABEL name=Photon OS x86_64/3.0 Base Image vendor=VMware build-date=20200522
# Sat, 23 May 2020 01:30:10 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:868db15bb2ca68416408afa1b6e00b73d030f4255494933d63ad6ed2e2044004`  
		Last Modified: Sat, 23 May 2020 01:30:27 GMT  
		Size: 15.2 MB (15167752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `photon:latest` - linux; arm64 variant v8

```console
$ docker pull photon@sha256:87bdb08bc4384f7c5471a7cc826b6779bbc194eddb0684cf6304bf2f5046c934
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12962444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c1251dbe75c0c7f1402e566256f658348ace07d771d9842efac21b60fcaa53`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 23 May 2020 00:52:00 GMT
ADD file:311d79925173a4dc58fde9a967d094e79f318c51937586dc9298a2e4b0a9e3bc in / 
# Sat, 23 May 2020 00:52:03 GMT
LABEL name=Photon OS aarch64/3.0 Base Image vendor=VMware build-date=20200522
# Sat, 23 May 2020 00:52:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4f8c382308ca72c53d44246ee3746dd73f50a2eba6a1da7fea53dc963f0743d3`  
		Last Modified: Sat, 23 May 2020 00:52:30 GMT  
		Size: 13.0 MB (12962444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
