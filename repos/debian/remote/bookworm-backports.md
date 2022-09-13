## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:43f3ce8cbd5a492770d678e4b8b13b47e03f11a5c19cb648355bc5cc679b08c2
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:9af5b53b6f5524d8940f34d785b4c139f17009ce04152c63c7cfacbce824b0ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52983836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f20a0bf770ed055921cb80566f987e2b44171da90a662aab932cad3755168d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:55:59 GMT
ADD file:3b3b943815afcac58f0e8a49af9b3ab289e32cdd69d4c6bb0c64665439c8619d in / 
# Tue, 13 Sep 2022 00:56:00 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:56:03 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:97357bf36a88b062ffcf42d1d32358484d7f104afddf68a27fc780d5e4b35747`  
		Last Modified: Tue, 13 Sep 2022 00:59:24 GMT  
		Size: 53.0 MB (52983612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b8c76f392ce2428816319f1a73aac900a2f46825c08e9957c1a1ac3e9584c0`  
		Last Modified: Tue, 13 Sep 2022 00:59:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:452fb96912ae9d536ffceba237d340fdb6df659d945b8c9f45782bb824fba381
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52122766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18c5f9813646fb6f77f6a1100dd2c6d3266fa13ad6c88981864bfa720ccfff59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:52:16 GMT
ADD file:fafc9bc142e136ee85605d8e97e30de6b77737818f595795657169b6296c2106 in / 
# Tue, 13 Sep 2022 00:52:16 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:52:24 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7ac1aef77561a09b4a507bdfee90352851c4c589691168642e1962feeb17f470`  
		Last Modified: Tue, 13 Sep 2022 00:59:23 GMT  
		Size: 52.1 MB (52122539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd577085d4fc2867ef390534184ca3693f7977930392b8a5a3563035d93670a8`  
		Last Modified: Tue, 13 Sep 2022 00:59:37 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:bf883eab8c0ae068335982b699ba236d03dfc5a04e88a550bb5661f5396ed1c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49555317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aa6d9c9222cf43f22e3e6d4ba26e6a22765f05e46d9b5a059e5505b46022ebb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:14 GMT
ADD file:590ff1916ed8a15a7a205153d20c2823a242c228573a1868134df4bdd95f10d8 in / 
# Tue, 23 Aug 2022 01:42:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:42:22 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b4a2cf95b2637a1520aeb527ca7569456a3bcf1d740f72cc418357cbe490704d`  
		Last Modified: Tue, 23 Aug 2022 01:48:45 GMT  
		Size: 49.6 MB (49555090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1915b01a40b5fa0a6d70fbbe851c9a3a6d79632d5880f4f6d4349d613c8b8294`  
		Last Modified: Tue, 23 Aug 2022 01:48:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:72794a193365f746305aa344eee1c275109b6662c7913441d09287d260e6df24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53117790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97820cba02c5a46bb226141ee8a37105f389599db6a8fe2a25e02c8f5e8db7d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:51:53 GMT
ADD file:f94a576f262c4fcf5112164145c04850c826787b299878e7e126754d1211a51c in / 
# Tue, 23 Aug 2022 01:51:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:51:59 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7dd208a8a7339c037c691e6ace1cd3f94803ee4c17a3211b9ccadf01d1ff2ca9`  
		Last Modified: Tue, 23 Aug 2022 01:56:50 GMT  
		Size: 53.1 MB (53117563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e50667678c3bc818bf4491880eca873f36d1eda574b45d21c34d25ebda6637`  
		Last Modified: Tue, 23 Aug 2022 01:57:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:ebf728c02291865c130d4d8e793f26242f107192f6e1a2462c3b278bb6742668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54097163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1a9e464985766d6cc435b152f3f46ae2250e7b2bbe87d78c9feff0c9f392dd7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:01:59 GMT
ADD file:1c8ebe8b69a2d3c236c8a947162fab2e579f4bf01bff01695a3c46557f6c73f4 in / 
# Tue, 23 Aug 2022 01:02:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:02:06 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:29bf8f676853094720e43096224f2ec8a31ffa3752cf7a1e52fb9e72ae069480`  
		Last Modified: Tue, 23 Aug 2022 01:07:13 GMT  
		Size: 54.1 MB (54096938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a1f14bf6d32c514540083e07e1d8512a2532b49fd43d6efdfc4633ea932833`  
		Last Modified: Tue, 23 Aug 2022 01:07:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:88a92685f8588e036311c9e1396eb8658be3a205e1c3249a36e74613d6c5e663
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53119576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afe2ac5ad32ed3e283a9692d8afa222a7d9366148c7a92dd71a4aad1dac1ffc7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:09:18 GMT
ADD file:2b4a878ee82590d9ee2da01a2501742d21f6d050a0002f9bd484a4d7c8620d2e in / 
# Tue, 23 Aug 2022 00:09:23 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:09:42 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4b18e364c6342ca1244071a2f94edf42b92a5b7997d16df3b26467139f3f0603`  
		Last Modified: Tue, 23 Aug 2022 00:17:33 GMT  
		Size: 53.1 MB (53119349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dd7949df62368fe8995f95aaefbb19714f16174623c9a7e62352db95b7d53f`  
		Last Modified: Tue, 23 Aug 2022 00:17:43 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:39a3cd3fb1cd9159584cae2feda4d2b63e6772eb80644b997f5fc881256bcbaf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57290094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cc160c48535921230dd425b13def27152d315f20b5dd3f982bbe278afcb6959`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:23:48 GMT
ADD file:92444ce23c3227ef88446469c37fc41decda1ba975ddfb1be3e1ebb1e694471b in / 
# Tue, 23 Aug 2022 01:23:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:24:00 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a2d2f2c5b4e64eabb8a7632609e67883239433d932129bf478f7614059a9aabe`  
		Last Modified: Tue, 23 Aug 2022 01:29:05 GMT  
		Size: 57.3 MB (57289866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860a9e529b4934b84efffa7e325339ec53cc8207eef318d7e3262eda4c87e3f6`  
		Last Modified: Tue, 23 Aug 2022 01:29:16 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:a2c63f586d8bf640ce02fc71973543b7a62eb43762d70c0d479206409d5319e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51793961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c05a821067f2f9f5194546712b8cd36b35457bec95f605406057b79ee1e2bd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:47:18 GMT
ADD file:b7771dfd52d59914f02d6a960a15a002d38a4ce20bcf17ccc9e77d105dcc970f in / 
# Tue, 13 Sep 2022 00:47:21 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:47:27 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7aeb98a659275cb80ecf5c5010e17e1f9dbaeb66dc78b0b9547e7d2cef3ccbed`  
		Last Modified: Tue, 13 Sep 2022 00:51:49 GMT  
		Size: 51.8 MB (51793736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947cfdd569edb2e6807c07964af3f63cdd2f0706430ed865c2d5898145e10bc`  
		Last Modified: Tue, 13 Sep 2022 00:51:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
