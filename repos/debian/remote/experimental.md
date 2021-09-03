## `debian:experimental`

```console
$ docker pull debian@sha256:48a203cd50aa7d40b5a91ff46d01b1ef20af999496c3b453aacfe0eb0d62266f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:cfe1329c2d8a03a08401c718cd75f14aed9b444a027860c4f849eae18151af34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55493613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:873aa48b37d5e7e421e2f1f1442a07965c596693e1a5a219204e4280d25470db`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:24:24 GMT
ADD file:950698d1761eced134cc40a827634eaf3a41bc5f0d4912347d5241448077afc1 in / 
# Fri, 03 Sep 2021 01:24:25 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:24:41 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:40420c2d03cc54fbad3be21a2561d1f604527779c58487a247b003b9e54a8b53`  
		Last Modified: Fri, 03 Sep 2021 01:33:14 GMT  
		Size: 55.5 MB (55493390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70bfacc355168474324653eaffe320feb3e2b06d0d4f02b1de26a2a2604487f`  
		Last Modified: Fri, 03 Sep 2021 01:33:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:0a80e5feaef869d9e80bbf4cd7abf710f2a2d7987dbcfc6cf396a1bb18f2f104
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52980345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47db9d8f2ce1034d197cbff322fc3b69b0e1b92a3a6708ce678ac37099a4fa4`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:57:16 GMT
ADD file:35aeefda7cbfe52bd922da8352d6d36205e453c6a01b4910ead51a57fefcf7d3 in / 
# Fri, 03 Sep 2021 00:57:17 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:57:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ca8098013e2d6d0f3902fecf5766117cb6127aaf3e4a072165bec0be91496740`  
		Last Modified: Fri, 03 Sep 2021 01:16:21 GMT  
		Size: 53.0 MB (52980122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef4f643165173ebb806bcc9a93f77dc42b48272a6a7e22ac5dc3f89bda3647d`  
		Last Modified: Fri, 03 Sep 2021 01:17:08 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:c7df2064f560eb970d0a6e538a367a2f4913d749dc1d61775c46610c8c6bce49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50638101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a980063ea4a9aee6776f6336034ae5cb0985e08c9e660417502a6f9525d6c995`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:06:44 GMT
ADD file:bf59d647308e39808e127bfb478b359d6955717fa6a97c2c7a25d4bff031bb36 in / 
# Fri, 03 Sep 2021 01:06:45 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:07:17 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:48cda209034c6e805739dd1344fd37380f55e395e8cbcfb88881d7e80cce0cd1`  
		Last Modified: Fri, 03 Sep 2021 01:24:44 GMT  
		Size: 50.6 MB (50637878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55c00440b3dc92ccad515e84738d786919790de7d2fc4471bca6abb677c7301`  
		Last Modified: Fri, 03 Sep 2021 01:25:25 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:82570506403fd4dcd58ff6a3bedea1eb11ec82252b529047c233c0f261edeff2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54529344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943540cc3b93744bafad592f2400f40b75a06a3f3227835ad4ffb0797a556959`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:22 GMT
ADD file:4a5fc16e07f48a7bcaee26c8506d7ee46ae6fc1b1d041dde1505916210b9ef1c in / 
# Fri, 03 Sep 2021 00:43:23 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:43:37 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d722e834fa0a0a055247562f40e9205cba88a0611d6576bee62a4a2823a4f93c`  
		Last Modified: Fri, 03 Sep 2021 00:54:36 GMT  
		Size: 54.5 MB (54529125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e5c6a57e181facd8e4a375c7aa06c55ee875044742f094ac1dfe23d9faaf60`  
		Last Modified: Fri, 03 Sep 2021 00:55:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:fbafb68a1afbb83386f6674ac096b0d86f0a3045aca13f4cb6923f1d4c77d0d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56525539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8342648ef9819566b937597e8cc4b02089710ce7b50e3e602ae878e9eeeefaaa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:32 GMT
ADD file:819a543f28fdb3c78df21d78aa7ebe8bbd9c5bbe8260844fb608349c98b5e469 in / 
# Fri, 03 Sep 2021 00:43:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:43:49 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9905ffc78aa155ec4132d8e271c7a3d74e19790dd9358c6c80dd4f1f45f53165`  
		Last Modified: Fri, 03 Sep 2021 00:54:38 GMT  
		Size: 56.5 MB (56525320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec838ee17240992019100199f6cca2669a7bb9cc6db88598847b0cf155617ed`  
		Last Modified: Fri, 03 Sep 2021 00:55:08 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:2ed22c2d5401836f139b991a8854a9c7c57ff3f53e3a5663bd1983a1722cc4d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54135244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d40ccd1286730ae8eb176aa590538c011b64aecba3e3557d03e998cd5607da80`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:14:31 GMT
ADD file:06b8e6c7631dd03ee95286f60728e93dfb5305af071b2a1de415e3b00f0b7566 in / 
# Fri, 03 Sep 2021 01:14:32 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:14:55 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f9d6f94c6fc458ecc22830abf12c00aa2f763c4a38fae527558ce527081e5c41`  
		Last Modified: Fri, 03 Sep 2021 01:25:51 GMT  
		Size: 54.1 MB (54135022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0386d5291c708d9029e7e1f150f8ea82b06ae79c9f56e0587640cdee75f44d`  
		Last Modified: Fri, 03 Sep 2021 01:26:34 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:b77effeb230813d98019e468976c35c32cdae47c34288ca3c3f9f824f041bfdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59534260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be868c8b2b7500d0ce91a7f829a42609e6d7298d8816f5aff36eea4a7316d879`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:29:00 GMT
ADD file:8a51a1c37e3e8707357ea465cbeb661f779abe15dd78177b507df7c4f379c897 in / 
# Fri, 03 Sep 2021 01:29:09 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:29:58 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7997061ae42bdeebd52a682046b07a537363cce99bbd8e1a5a956bfd26232482`  
		Last Modified: Fri, 03 Sep 2021 01:49:26 GMT  
		Size: 59.5 MB (59534039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5d123292116ecb7c8730a465d5ee07226ec12d896df03e1497f7e1ef75c084`  
		Last Modified: Fri, 03 Sep 2021 01:50:22 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:2f9e2910e97f2f8bf6bcf98353c63a690b487472f8194a39725b6f39729fbc55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51289309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44045f90bf5edd1432148a0f26dc9b197541a2dc4705c25d039c28905bfdc67d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:19:47 GMT
ADD file:3c786ac2e98158e7a24470ce33dfb8df0e24a7ab1702ac34cbb800f320c8744e in / 
# Fri, 03 Sep 2021 01:19:50 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:22:59 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f8fb8038fd63561c7012487a4a41109b5b2414eef638d69d26175cb04362653c`  
		Last Modified: Fri, 03 Sep 2021 01:36:05 GMT  
		Size: 51.3 MB (51289081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d9a67317214661414bc8708ec3c18456cf229ff064caa4fc6b48383c2532eb`  
		Last Modified: Fri, 03 Sep 2021 01:38:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:785b10a6bfaf45fa698fc85954d428d551717f4d79323b9bce66b0f279d02f51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53772329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24918f356bcd5e8deb1f8d43173cf7e9fd81a3599216b196da9cfc6d668ce787`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:48:40 GMT
ADD file:9b4c0f03543a9f640bb4b4227cafcdfde8ed6ee17d8c745c0397e759c0800867 in / 
# Fri, 03 Sep 2021 00:48:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:49:16 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:85bc6421e22ceda228fb019ee19eba91b0c9eba555c9c8f9b89de3d9a5bf59ab`  
		Last Modified: Fri, 03 Sep 2021 00:56:12 GMT  
		Size: 53.8 MB (53772110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3a16a5e178309acaa94e16651ea4a2ea8d143dd75d7c8099a27f2f4c794a29`  
		Last Modified: Fri, 03 Sep 2021 00:56:33 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
