## `debian:testing-backports`

```console
$ docker pull debian@sha256:58638578d4b9be0c0effe238aec8002f2080ebde90c1af1a148cb9dbf6dbf18f
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
$ docker pull debian@sha256:caf7eb6d4d01e0da03c2f5e2584b6f0d5e723d8b4e126a82c4e8087662fa354b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52947837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7443448636ad8531c9687611e48f25bc11452ccce82778dd956541119f62e44c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:22:29 GMT
ADD file:272efeab320060153c6fd77f52b9a9922149739b8f010d93cde516421fde6ce9 in / 
# Sat, 28 May 2022 01:22:30 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:22:32 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:344633e2dec142d10b6e072c2fded693fe7441d6af83d21be68657a30ac0ceaa`  
		Last Modified: Sat, 28 May 2022 01:29:25 GMT  
		Size: 52.9 MB (52947617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be116af98e38fc33d2af4190a3b8ae6e390be60cc4e0e47f8ea2123ce2186281`  
		Last Modified: Sat, 28 May 2022 01:29:34 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:00e270b63d602b8e07db5eaa7a45c6851249f5076a82f32ae9089052aed255e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50737668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2974c48c2c4bbae176be7a26dfd0e5dfef698104042716efd661ea5e4996484`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 00:56:34 GMT
ADD file:335e5d916082436e2ae0ecb67efce63f983ef63c07c914bbe30f28b6978345e1 in / 
# Wed, 11 May 2022 00:56:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 00:56:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:01866b086b60cccf118ed98e37131a03befcd6038523a4965798d5958be62b2d`  
		Last Modified: Wed, 11 May 2022 01:14:30 GMT  
		Size: 50.7 MB (50737447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1245b9c44cf9f29296f26bc7f68ba0f5eda840bb995aebc768da9d7159e21f0d`  
		Last Modified: Wed, 11 May 2022 01:14:41 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:7334196c26083f06c33460cc8e9169d5300470fc9bf4ef1dcb55a83ec561010e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48476635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f7855b424dc327a00f2a1327500fd69decb38caed94ffd316afc0723069664b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:06:23 GMT
ADD file:ec90a19450a4b3174d662c6df3d034488e52773bda79988366e79bf6ac179803 in / 
# Sat, 28 May 2022 01:06:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:06:36 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8e10f53774ef90fce803a05457ec21c9be85884019be903eeed2eba672058603`  
		Last Modified: Sat, 28 May 2022 01:22:58 GMT  
		Size: 48.5 MB (48476410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754c9b025727de20960f9cd09ef91541685dddba7f11ee2f1f1a3d02403b5b1`  
		Last Modified: Sat, 28 May 2022 01:23:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b29176c47112ec1fba9289ab151aba958a6d3e698f1cc88bb285dbc66711a733
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52043058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950a47f33636412fa6a179b1de08a035c7cb5195eb34741cb2abf700bd965d75`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:43:11 GMT
ADD file:936ad327dc97009e77bbb7d1d1874d55f3d251b8a641269356e5caabe860a8cf in / 
# Sat, 28 May 2022 00:43:12 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:43:18 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:75fd77c03641c04273179a599ef54dea600d22da8b30160003b50fa90a397f43`  
		Last Modified: Sat, 28 May 2022 00:52:12 GMT  
		Size: 52.0 MB (52042837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d8952cace7dcdd6d22b67b71e408cb84aa441d311a79d1b659efb863a8a511`  
		Last Modified: Sat, 28 May 2022 00:52:22 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:2ae20ab0c719dd94075e09656f3d4f70c7725c44d3cdb8d5dfdf82fe3f13ed8f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53948783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66072ecee508b09e5ec57f70131493d1f1bda79ce51fe984f99d5336c1b10f3b`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:42:18 GMT
ADD file:ab2acf453e0f28f32503a483bbda0e5e5d09513add50fe39f591bf33810a4be7 in / 
# Sat, 28 May 2022 00:42:19 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:42:24 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fd2231baceb33fbf6629c80839b9f9e3d4d4c20d0adb42b699791bd018f52c4c`  
		Last Modified: Sat, 28 May 2022 00:51:24 GMT  
		Size: 53.9 MB (53948561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e976480a8fa0fa79af4d6edecc9226f5d87d94b720993356bd214da6566c34e`  
		Last Modified: Sat, 28 May 2022 00:51:35 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:10a139b089bcde60f6dea6078e9d280b9b67595ceb4ee65f77229787fd5fc45d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52061751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02cf66d72c11eccbf905331a064453bddab397ba9749d2504aea6948ed12dd6c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:16:20 GMT
ADD file:750180a6aa4a39bf911865e098608b764a75b2c50c00426efecdab074d6108b8 in / 
# Sat, 28 May 2022 01:16:25 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:16:35 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7cb5df6daf04a8d6061a3059f38de0f503140d437089f54459799cd3d1d80736`  
		Last Modified: Sat, 28 May 2022 01:27:18 GMT  
		Size: 52.1 MB (52061526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf5a681f228150ffe7fad4dd9f6867ae147fe99d64651bc317d7caf4218c365`  
		Last Modified: Sat, 28 May 2022 01:27:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:5518506b13061064f86c0cd6efc52467e153897864b9cb91cd5ebb995502336f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57161810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83815a9fe561145424b30cc855571a8ce47f3baf299a5377ec73453fe75cd690`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 01:26:41 GMT
ADD file:c839faac39e30677565fb631dd4f40114392a7a667b8db7f85ca4d8aaeb32ad9 in / 
# Sat, 28 May 2022 01:26:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:26:57 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f5e0403edf3ce1164c65241f62272268585e383702736c781adae79230ef3422`  
		Last Modified: Sat, 28 May 2022 01:36:21 GMT  
		Size: 57.2 MB (57161585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792635adddbd4dc72f42008b9ae6fdf2562c007ff11a1ae6c744cc1cb0fee0a5`  
		Last Modified: Sat, 28 May 2022 01:36:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:b543eb0a4ae55dc75224231cf2452658471b34c9b0a0a93aaa8c2255e424a0d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51490491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ea2b9a1a4faa45af4ccd1fa6dec287de4c597e3f302da04f20edeeadc3f66c`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 May 2022 00:45:48 GMT
ADD file:430aae00218790907570f298b5f5c4e47453d9297090e8d006c5169e5e9ee56f in / 
# Sat, 28 May 2022 00:45:52 GMT
CMD ["bash"]
# Sat, 28 May 2022 00:45:59 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:33ada038def02ed9f3f9762c43feeaf3a66329f979154e6d3dca5e1ac4f04893`  
		Last Modified: Sat, 28 May 2022 00:51:52 GMT  
		Size: 51.5 MB (51490267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1406700fa9997a58c70749575703dc4eb92cff73a6f738556df67a17ae55ca76`  
		Last Modified: Sat, 28 May 2022 00:51:58 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
