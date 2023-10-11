## `debian:testing-backports`

```console
$ docker pull debian@sha256:1dca2a4a21d4b644c3612c80239e19431c6e2d16814801a1c85e26a0c9a5e582
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:554c782743a2cbf47b879b87ae60729677270409d1accb6f428c3709ab0abcf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49467887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e32cd42b8c8a0c71cc2ed56db0a7c5691601e241e6f7c8c38a303de06ab5678`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:56 GMT
ADD file:ef0363530acdb66060536a24b4c64786db9f35d1224e1d13645c9e15a1a5a352 in / 
# Wed, 20 Sep 2023 04:57:56 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 04:58:01 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dd55a40fdbce1f8af26c95e5d3ea6a93b913082fb16ba4a530d076e6527a3172`  
		Last Modified: Wed, 20 Sep 2023 05:04:15 GMT  
		Size: 49.5 MB (49467667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59c30b8f8f8a49e55d7635804c318964d4ff6a1f86fa6d16fe13a8d1ca3fe3f`  
		Last Modified: Wed, 20 Sep 2023 05:04:24 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d72bb90f991f449b3fe7a10727bc205db9dd9c2ff126653eeea3a2cbdcb08324
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47166271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f8eedced1e33e1161acf07a413cebc8e9ac724c2d811beb4c1f572faee94bdc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:51 GMT
ADD file:90095ecc4648e585c28161630790e6ddf797a1d5e3c8fa81c0a51144778a29f8 in / 
# Wed, 11 Oct 2023 17:38:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:38:54 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:51b4caaaa9456643ad602841f8e6a2db32f3983c7574e3d83983e5c370cad79a`  
		Last Modified: Wed, 11 Oct 2023 17:43:35 GMT  
		Size: 47.2 MB (47166048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05034ffe2f74d4320bf3a2045e93ab6e5162d2761859fe3ee2a520158f0aeeb0`  
		Last Modified: Wed, 11 Oct 2023 17:43:44 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:d870dcf4c9a86f94231a9468b6b2d26d5035b873626d1d806a3a124630533195
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44954330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422aa8653399e8d755b866c3e9bbc9801b204a0dc68ac22d4e38445b57b60898`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:07 GMT
ADD file:2c0647528c2d5ca3b54a79ac650086051f3f650d781923e2666bdec55af7b027 in / 
# Wed, 11 Oct 2023 17:44:08 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:44:11 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f4f1ce3e449db1b82bae116e4564c1cc5d23a09ed962d4e3783f6eb67e2b3b84`  
		Last Modified: Wed, 11 Oct 2023 17:50:21 GMT  
		Size: 45.0 MB (44954109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86e8e1a8ddefcc793d607c81af6397bd4d8d54751bbdb4b42da38785414457f`  
		Last Modified: Wed, 11 Oct 2023 17:50:30 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:181c8c60a8afbb88aa675d0bfdc76e801ebcd217522368a9cdbd66faf8a262bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49404752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d346454a93ad1829db9182aeef2bdb8b01c2f026f6d6c74226b179bda0710b2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:43 GMT
ADD file:f0c1d15ee705796bc58abf92f15b7a16aa341028b6e099383437710d3694d315 in / 
# Wed, 20 Sep 2023 02:45:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:45:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c80309e0a5bbe8e3c8000103b383c6a60c58a6a84681e6aa5963d565eebe59a6`  
		Last Modified: Wed, 20 Sep 2023 02:51:00 GMT  
		Size: 49.4 MB (49404531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28a7bd6548127d0396a249571cc55f534c820732c903340e6fd755544ceeefe`  
		Last Modified: Wed, 20 Sep 2023 02:51:09 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:e50d27d67bf557a773e1a63413204ce3e5aa152bc67087b163d5b725b3c1b826
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50486074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:553ac2f90775679a7bf846b5f9c5ca3429692a6abbfcc72527fca0b49ca08375`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:59 GMT
ADD file:bfeb3e377b612c7fcb781c1980a81bffebb8cf6326f1150a3e4f046311086965 in / 
# Wed, 11 Oct 2023 17:43:00 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:43:02 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f198a34ff25398acef7fcce11c60c2a1285d11e32f52e1ceda06820ea36253a7`  
		Last Modified: Wed, 11 Oct 2023 17:50:19 GMT  
		Size: 50.5 MB (50485851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df5f0caeb95cbe509d9ef70bd4d2298dbf4292fe461487fddabbb2ff297adc3`  
		Last Modified: Wed, 11 Oct 2023 17:50:29 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:be604f4a48cb3b5a58665d812821ce73a0096fe8c853d1694b4fa5e93809d6e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49301982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8976c5193e0b3609d5ea1cf0b6b783495aabe1617bed81d8b84ea31f9409c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:55:01 GMT
ADD file:82f75dc79ee75c27769804102d2e90c2984ba8bd6d2b0a73b950ec1cbde18dcf in / 
# Wed, 11 Oct 2023 17:55:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:55:19 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9e6f29830ed449161a2082331b9332fb7130a29d7885b43ffc86d2b945010a9e`  
		Last Modified: Wed, 11 Oct 2023 18:06:27 GMT  
		Size: 49.3 MB (49301757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fc65d038748028c18ca6a726671801d312c3f97318e478965c5e9fdad791a4`  
		Last Modified: Wed, 11 Oct 2023 18:06:37 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:65ee705b3024b07dec9da05e332f6fd99daf2a1b9cae8c0dec513bfc6916f0b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53418358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a3720bbb04bfe5a18e5f4abaf40868365a747e4a08acaeaa37746e3dc022413`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:46:50 GMT
ADD file:c877fccf97ee8f77aa2318c5d5fc9deea9905e038d11730ba52d9dd50217738d in / 
# Wed, 11 Oct 2023 17:46:52 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:46:58 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3aaaa4d84036ee17b7ad898e0a13bebade18f92f2c7561f3d407624d1bb0da74`  
		Last Modified: Wed, 11 Oct 2023 17:53:38 GMT  
		Size: 53.4 MB (53418133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f7e2389903519684cfad376c6de72988d3a1a3ad5397105397093ea7c2dc4f`  
		Last Modified: Wed, 11 Oct 2023 17:53:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:119d16b84f373b3b0802d7661208a40f8dac9beb94491b3184014ca3238cadf9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48924564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d2b43e17fc8fb971635218747bf78e58c6b9253e4fcf7810ec9e02a70d38b1f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:52:40 GMT
ADD file:9bdb90e9fc1ff4c63bcf3d994b2211b30b462d560247548fc2e3493704b91c5b in / 
# Wed, 11 Oct 2023 17:52:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:52:50 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:02a6d6b749a80726477cd9a1565b54a7b73acee565b6c727afa20dc76f42a0a7`  
		Last Modified: Wed, 11 Oct 2023 18:00:50 GMT  
		Size: 48.9 MB (48924341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9201e3925d288aab68c6e22c2f34d566db0c968ed7150a12081545394f5daa98`  
		Last Modified: Wed, 11 Oct 2023 18:00:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
