## `debian:rc-buggy`

```console
$ docker pull debian@sha256:b165ba01c0ab950cf4dbe10a9649642b1121133397651e5d364cad62d622d6f8
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:111e6e92397717f1da103aa944e5df696cf7c4920a5556e9f478281df8b00914
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55702309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bcfd9574ccbe8ab4ea0e5f4d33a650cf552e8b7f8497f573a1fc7fd0361f938`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:24:18 GMT
ADD file:43a49c0ac74573bd560d191480bb30b2950f21ec76e9b3bdffdf73eb74628c50 in / 
# Tue, 28 Sep 2021 01:24:19 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:26:35 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e3fead4ded84f6449ee17b9deabf1e9144512edf86da02e0f93fbf81df3fd6fb`  
		Last Modified: Tue, 28 Sep 2021 01:31:21 GMT  
		Size: 55.7 MB (55702084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da498e7dba01af8f0739170de21db5d14f88e820a5ffcf875f6c3655933e4b64`  
		Last Modified: Tue, 28 Sep 2021 01:34:23 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:06f4bac1d309d2e597300ff8f07eead2e9834ebcaacad7c26f6baf5226c888f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53207981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745fec711c40f032b7516c875226224e1374d46d32eda9784760d9728689e243`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:54:15 GMT
ADD file:bcd1f002a3a38be54eed5da9d7a2e3822ecdf63ba82a59931124557d1f97007b in / 
# Tue, 28 Sep 2021 01:54:16 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:59:00 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:4bd09bbbe96b85664474243c833d73be517c92e7172b8d740101438ee21d5561`  
		Last Modified: Tue, 28 Sep 2021 02:11:21 GMT  
		Size: 53.2 MB (53207754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78897525622bfbc06e7186b781a71d2ca727ad7d8ec551876800532ca5402cef`  
		Last Modified: Tue, 28 Sep 2021 02:17:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:0382bf7f6d519c5a366aeced634254b2ec776ff54919c2ff626b4eabd0189446
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50822661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ece0ae76113c354498ae97f41a14cca3a092ee134db3232cfd4deba449e7da`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:06:54 GMT
ADD file:d9a8e8032b2f681adb1be7e9dfacdf1838167068f97e052c3173223cb1d2c303 in / 
# Thu, 30 Sep 2021 18:06:55 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 18:12:02 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:90a9a2564a394330c4b6320f33e007b55c6f40a9006b85fe17fa2ed9fe260cee`  
		Last Modified: Thu, 30 Sep 2021 18:23:58 GMT  
		Size: 50.8 MB (50822436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7971753a91d151d9d6e9431af64dc7b3f78ccfdf417d501f6793bdd5f03b36`  
		Last Modified: Thu, 30 Sep 2021 18:29:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:45fde50e6b76c1ee375922f48b82a6e143acd30300ff69b00be9024fec545836
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54725527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb4e911cb0225c8356831278817a4a28bf551a74cc1edfb59f66f3703f4b10d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:20 GMT
ADD file:714781c9fce1c450e5f9cc5529167eaa33fdff089ab48a1dcac0a813d768be30 in / 
# Tue, 28 Sep 2021 01:42:20 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:44:29 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:bd53cd90ab526d30a2e414c3951333db1b1b814fe009621017a07b5eea3cad0f`  
		Last Modified: Tue, 28 Sep 2021 01:51:10 GMT  
		Size: 54.7 MB (54725302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236a68a66e98200b3cb5d14660ec7bd11f989f811b802bc35c2db90cb28f992f`  
		Last Modified: Tue, 28 Sep 2021 01:54:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:83e9a21fa9a08c48eeefbf186803658a110d42b6895b360664a4fd6106a6e3b7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56733552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:749d061a019a4435e2b67bd12b7cda453d5cf00c573652122da27f52627dd44b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:17 GMT
ADD file:07dfd2960f3649fbe7a701ad0b551f48b4815ff5eabaefe7aaf62e770435e5f2 in / 
# Tue, 28 Sep 2021 01:42:18 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:44:58 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:e7ed4b6e2f624e3ac187bdfdafce616f76387ede25afbec70c204c9d6300d2e0`  
		Last Modified: Tue, 28 Sep 2021 01:52:05 GMT  
		Size: 56.7 MB (56733325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77eea00cda077e450d053d5e5a43393be10803a8e55feb6516fb7fba19f29bc`  
		Last Modified: Tue, 28 Sep 2021 01:55:59 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:82204a540062e6fe06fd10074ff79e53ec41741f1530850f2a1f5e00d1205e29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54326378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484ba97b4c3ffdde09fccd698d63ef22e3482260f906a2ef64c7eab64508aca9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:13:16 GMT
ADD file:37c840854d981a81a27b6080ead6db0f2ffb138c53ef4f592543a73b0d0d2d20 in / 
# Tue, 28 Sep 2021 02:13:17 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:17:11 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:48db6be5b154d5ac1d5fca89bea59293f6bbd71d0b6e918bec46cbfa79afc0cb`  
		Last Modified: Tue, 28 Sep 2021 02:24:08 GMT  
		Size: 54.3 MB (54326151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587bb4ec95c2caeb130025bdccc9def985870825bb9e43c6c9a862f0a630bcec`  
		Last Modified: Tue, 28 Sep 2021 02:28:45 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:bf02f52b0cef37c5dd890d9caa2cc859d5e0c197806b43db1ebe6ebdb26a22a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59534299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49da3929aacc93abff8f77a8ee15827c1aaa987292cf8781aacb8f76e67addfe`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:26:09 GMT
ADD file:eb825a05756409572b414e35fa1f7f58986be1d8d7b4251cf7ea2eab299ccbd4 in / 
# Fri, 03 Sep 2021 01:26:18 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:30:39 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:eeb3edf1a6fea1725c5b8863036bbeeab17fd1ba2d09e50f1a016800ecc239a4`  
		Last Modified: Fri, 03 Sep 2021 01:42:46 GMT  
		Size: 59.5 MB (59534072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c055d4d6c20555e40f6f325ce64682784d28fded349f4a0863224dd64d114e`  
		Last Modified: Fri, 03 Sep 2021 01:50:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:56771dfc1ba65be5694075eab3607a77c90917e1082e768a245ae8edbc00a4a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (53954062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3c2c9337fc1b167c9442d42180b7194d1ff4e2c09f3858092fa4f9e1ab91bf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:44:11 GMT
ADD file:797f09f7e25e9194e8845d5783ab9078062d7caad45c75201a4ad699145b1305 in / 
# Tue, 28 Sep 2021 01:44:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:46:04 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8463103c03054c6dd4bf0a387d658bdf4d12ddbb0d87ce07eaa15b2b13f1d733`  
		Last Modified: Tue, 28 Sep 2021 01:50:20 GMT  
		Size: 54.0 MB (53953837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f7550321dad7ba75cbd554ca6a6d470378d9189f8f59788bc35885eb06512e`  
		Last Modified: Tue, 28 Sep 2021 01:52:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
