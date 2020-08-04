## `debian:stable-backports`

```console
$ docker pull debian@sha256:c2ae6d04a4a5dcd77ab37540fd5e089cd1792c0e23ff5453790def12fda04432
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:36332bb99256ec6435b20a917ba1492e1027a0b3879160e638a7bf4cbf2bc6e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50390548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0c3c786009f99b16a52b82e7d6f8f653c4d34339b15729f356ba34c34019cb8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:06:11 GMT
ADD file:e452c7756111c96e712dc2b42a59e87ebc8dfebeeff03939c62773d73c7ff71e in / 
# Wed, 22 Jul 2020 02:06:11 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:06:16 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3c77d565f42d8558a327c2abef361d045d9394c2bfacc64d8397fc382ff59f16`  
		Last Modified: Wed, 22 Jul 2020 02:11:49 GMT  
		Size: 50.4 MB (50390327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422792c8b6247385dfc23bc92c06e21ea0af03658b93b64489d074d84875bcf`  
		Last Modified: Wed, 22 Jul 2020 02:11:54 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:51e43fa71179af844a09fda18c53d4d99df19934bbcdda906a0f2db34e5bc7c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48108991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53d37bcd0d369763ad82f27556c9e0dbaac8e2cf9d9d2d4f94944556c0b4c229`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:21:26 GMT
ADD file:e304ffd272441dcbda0bc6091bb2424e494c376a8195e849b1c47e607e9238a1 in / 
# Tue, 04 Aug 2020 03:21:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:22:25 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:944323055e270bddfb919a22d90c31ab18917c182e34026afc5766874c7c1b4b`  
		Last Modified: Tue, 04 Aug 2020 03:37:41 GMT  
		Size: 48.1 MB (48108765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551784342112a5166f2c950dcd52c229a2ac4abdf16e5c21bdc7a3c8d99698c1`  
		Last Modified: Tue, 04 Aug 2020 03:37:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:9dd0444be6655ecf3dcdb7040d454ed58f06963a7a68baae5f169df0097a702c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45869475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc00362b2408b40ea228cee50045835bd98b0d9ca11e5f5273ae79c670a6656`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 05:00:11 GMT
ADD file:9b724e6f699cca258831a52859ce296717d0788630c8140c7dd277e0662205f0 in / 
# Tue, 04 Aug 2020 05:00:13 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 05:00:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:18fe0ed5c8b551a294aa9862bc05b92f8219a16b1e6cf8dcbf7c22706efd15fe`  
		Last Modified: Tue, 04 Aug 2020 05:08:04 GMT  
		Size: 45.9 MB (45869249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1596175bc07921883f6d42472b5ad79f74d4b4071c90a37527f140a4df2b3ea0`  
		Last Modified: Tue, 04 Aug 2020 05:08:11 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ae01f33d291f015bf1376b5d341c88060bcfdad0a58b98c1781d3c10e321fa11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49175693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ef613da7ba5691dce4dafbf5763eab2f23b0026e5f14a096d1af10e4e95c0cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:58:59 GMT
ADD file:e5eb4282b024f00bd592dd40d77a1e379590a30b287d64bf3bb9b82cb03e8d1b in / 
# Tue, 04 Aug 2020 06:59:02 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:59:10 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fa512392f2f38838ec5375baaadeb62ffcb80d4054684dc451e0dbc6464b89de`  
		Last Modified: Tue, 04 Aug 2020 07:05:37 GMT  
		Size: 49.2 MB (49175468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b0d57823362138586ca04d715607c6fe93ee651265efece79f4f718cc10583`  
		Last Modified: Tue, 04 Aug 2020 07:05:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:2e9563f36225b71a9439f73fafef5034042be3128a163bdcdad9126e8436f7b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51159072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23965c6818260479fd89cc10d9e3165c6f59c287be10092f1522670999e264b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:39:30 GMT
ADD file:20ea544484dd374a932f29445494a69a7b16d34b878c9e5926435f1f14218a63 in / 
# Tue, 04 Aug 2020 03:39:30 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:39:35 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:276a6e41eeeafeb66510d48c737e70ac7bda34dfbf1ba0846a1668ecd715be98`  
		Last Modified: Tue, 04 Aug 2020 03:44:43 GMT  
		Size: 51.2 MB (51158847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6382254da76be301cb428cee97c20860878e6bc5633a8d95665f73f88fcb8e2`  
		Last Modified: Tue, 04 Aug 2020 03:44:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:9bb04d30a111d3e859bd96188b75d514eda1d047e9ac8e5337f238c85a03174c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49017427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ab7fa2aca881391136acd2b69e164ce372f7ee66a18f851e877c4b4c18e4f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:43:32 GMT
ADD file:247bc212623a9a8b4c529b2009a59f5814dea432abd9c1bf7a740350438c5746 in / 
# Tue, 04 Aug 2020 06:43:33 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:43:39 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2437a5e79d3b12c528aa02859445b77947c4f28645d91dfe13cef840707eafe8`  
		Last Modified: Tue, 04 Aug 2020 06:50:46 GMT  
		Size: 49.0 MB (49017201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bace872dca909d7f47cb820a928d67cd0315e239d73f5f975832198338dc7d82`  
		Last Modified: Tue, 04 Aug 2020 06:50:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:75fa41879a8e85a2e031bf81524e0b31020db91e50736f16bc3e3851b8480cdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54142804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d28e2222733a224c1e55e7ac9a13afea3131ade986adf8804f56c728fdde8601`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:46:37 GMT
ADD file:cfb76d5b6760d4c98deb64521bcd3ee7aaca5f2d698a15ca7879be7671789c77 in / 
# Tue, 04 Aug 2020 04:46:42 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 04:46:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:00b89b02ac721b8d2474facfdd34ceadef210c1c970e4e9e9d69efbe2ddc4ce3`  
		Last Modified: Tue, 04 Aug 2020 04:54:30 GMT  
		Size: 54.1 MB (54142578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90139b2a191e2b99d9a2f8dc99d4294414e3df565f6571c6d4cc836511c38bbd`  
		Last Modified: Tue, 04 Aug 2020 04:54:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:765507cc3cbc4817334f1da7487aae987ada3354b0b891e73ee3e70ce0562002
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48966467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1b0106fe52227536506aae5edd81dbaf17e8bfac92f335ab446625f1aeac08`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:45 GMT
ADD file:e19ac56c8d91014cbfc90c6c3578c2c1a34a2e76c757da7d2d8f40ff3380f9e9 in / 
# Tue, 04 Aug 2020 01:17:47 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 01:17:52 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:08465fa67606b957d9c84fd1983bc0b0a74b36ae57921bc497155e7f9e06910e`  
		Last Modified: Tue, 04 Aug 2020 01:20:37 GMT  
		Size: 49.0 MB (48966240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188da64e7c466d5a4032aa747cd0014ed41f46c8097e1515ecded5221901c7c4`  
		Last Modified: Tue, 04 Aug 2020 01:20:43 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
