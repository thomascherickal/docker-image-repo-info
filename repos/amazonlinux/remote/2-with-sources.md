## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:dfa7380ea0a52bd33be4c1eb397875d8f0ae4266d78876bf7370c5a82b4899c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:50ef3e2e55421c716cf57afc28942eff9e67a5b5a9ea1410ce3c92c0f39953d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.0 MB (486032841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958ec2f24245a7af21fdf7ae9018d22e865f3b4415c53eae3a9777a667360e30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
# Tue, 21 Jun 2022 23:20:03 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-800a7e3918924b4aaf6f75787edd91de54d919ce798c4adbd8190b5dd187eef0.tar.gz"     && echo "ac78714ecd2ea0972b6b72ae2e7ac4b38e0a2d5f5e4751082abe2f4ceee1033d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f238a85b77bd523c86c594598f8dc108f464737b469c8818a79cc26aeae299e8`  
		Last Modified: Tue, 21 Jun 2022 23:21:14 GMT  
		Size: 423.7 MB (423737864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:7b886253583362ee6ebe7f69510a2738cc55ea0a9c1ae8c327e82877b3e88f70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **487.7 MB (487656467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5cbb8d5c004c62b734c7e854b889852efefd7ffd9133d286802fb5277006779`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
# Tue, 21 Jun 2022 23:39:54 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-800a7e3918924b4aaf6f75787edd91de54d919ce798c4adbd8190b5dd187eef0.tar.gz"     && echo "ac78714ecd2ea0972b6b72ae2e7ac4b38e0a2d5f5e4751082abe2f4ceee1033d  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488a72b37e827ac074cd544586f45070542b3658a4623a5da30a6d844f1d79e9`  
		Last Modified: Tue, 21 Jun 2022 23:41:24 GMT  
		Size: 423.7 MB (423737825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
