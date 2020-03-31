<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03.0.20200318.1`](#amazonlinux2018030202003181)
-	[`amazonlinux:2018.03.0.20200318.1-with-sources`](#amazonlinux2018030202003181-with-sources)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2.0.20200304.0`](#amazonlinux20202003040)
-	[`amazonlinux:2.0.20200304.0-with-sources`](#amazonlinux20202003040-with-sources)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:e3b8716df6e9b8b0846464aa2c886dc8e12438f5df92980b89997091447e90f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2ab43d6c5e8095784bce3868f225e38f98b9bd05a06c9ac61668dfde7cdefd56
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62034537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f555533483ad7a8ade2bd17f30b5ccef03994adabea93a14a09640c81494710`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 21:19:57 GMT
ADD file:131270c41e49176c5adc4600b4dba09de2714b702f4109c43bfd3dafd421747e in / 
# Thu, 16 Jan 2020 21:19:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:af904c29723d51f4e8a8880c8d9c81277b793aa04cff648cf34959db4f805635`  
		Last Modified: Thu, 16 Jan 2020 21:20:38 GMT  
		Size: 62.0 MB (62034537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:1eb876ad9e2fd0865ec07a0caa3546c97189659565ebbc77f1f995f51195d9ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:948e7877670f729ecaa48147e9d93532694410b3fec4216942b65ccb66881761
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.2 MB (388163218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3258945cc50f1d5dcffb7a41600366c16f10c02a72811119374817a6efdcd1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 21:19:57 GMT
ADD file:131270c41e49176c5adc4600b4dba09de2714b702f4109c43bfd3dafd421747e in / 
# Thu, 16 Jan 2020 21:19:57 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 21:20:17 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-82765bec2ec6aa88fb87dde775c5976db55c2a6f0aeb32fcaaffef420ff75f25.tar.gz"  && echo "2a02207625adf2733571c14cf68bdac4e3d4a481f14620b398c368e14bf0c432  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:af904c29723d51f4e8a8880c8d9c81277b793aa04cff648cf34959db4f805635`  
		Last Modified: Thu, 16 Jan 2020 21:20:38 GMT  
		Size: 62.0 MB (62034537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d458e146b5ee0e1d86be6bce69699664b33a9c6ea4776c15f025a46120ce49`  
		Last Modified: Thu, 16 Jan 2020 21:21:13 GMT  
		Size: 326.1 MB (326128681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:88a720de445a49a039bf9817af06e93c95e36f438bb8d72c15fb5a9bcae86bd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0df02385ce8946ad27fa935b969002302d11dfb13c91c3c4f7c39473a737226b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61669860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484b3aa1f6013f8ca133c20951b1b3b6b74da20cc0958ca474155852ac96b32d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Feb 2020 23:19:52 GMT
ADD file:c43f05fa78d78f998cd8e2e45f089e0572877490c7df425e514d44f15d958fad in / 
# Wed, 19 Feb 2020 23:19:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a7583ef20c9db3e6539d4160e9914383701901b24979656a228000718b0d5bea`  
		Last Modified: Wed, 19 Feb 2020 23:20:55 GMT  
		Size: 61.7 MB (61669860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:d9eb6060c8db3e70dd3452cbb2fca47f35a9e5cfde7ea7f3eeafb36d38dbb47f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63062950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63dbb02acf93525b5be87cc28bcf5cfaa5057ff67047bfd9e5182d3fc3c94fc4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Feb 2020 22:39:49 GMT
ADD file:bf00dcc4d3caeda14a7a6b3afb7f5dca29d64b43fe428f5713b88cec1a82f2a0 in / 
# Wed, 19 Feb 2020 22:39:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7f2fa3024eb129e832d7fd7cee7209fdab8adadbc3dc31675f191ac0414fb93c`  
		Last Modified: Wed, 19 Feb 2020 22:40:47 GMT  
		Size: 63.1 MB (63062950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:e3b8716df6e9b8b0846464aa2c886dc8e12438f5df92980b89997091447e90f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2ab43d6c5e8095784bce3868f225e38f98b9bd05a06c9ac61668dfde7cdefd56
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62034537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f555533483ad7a8ade2bd17f30b5ccef03994adabea93a14a09640c81494710`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 21:19:57 GMT
ADD file:131270c41e49176c5adc4600b4dba09de2714b702f4109c43bfd3dafd421747e in / 
# Thu, 16 Jan 2020 21:19:57 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:af904c29723d51f4e8a8880c8d9c81277b793aa04cff648cf34959db4f805635`  
		Last Modified: Thu, 16 Jan 2020 21:20:38 GMT  
		Size: 62.0 MB (62034537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20200318.1`

```console
$ docker pull amazonlinux@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `amazonlinux:2018.03.0.20200318.1-with-sources`

```console
$ docker pull amazonlinux@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:1eb876ad9e2fd0865ec07a0caa3546c97189659565ebbc77f1f995f51195d9ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:948e7877670f729ecaa48147e9d93532694410b3fec4216942b65ccb66881761
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.2 MB (388163218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3258945cc50f1d5dcffb7a41600366c16f10c02a72811119374817a6efdcd1b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 21:19:57 GMT
ADD file:131270c41e49176c5adc4600b4dba09de2714b702f4109c43bfd3dafd421747e in / 
# Thu, 16 Jan 2020 21:19:57 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 21:20:17 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-82765bec2ec6aa88fb87dde775c5976db55c2a6f0aeb32fcaaffef420ff75f25.tar.gz"  && echo "2a02207625adf2733571c14cf68bdac4e3d4a481f14620b398c368e14bf0c432  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:af904c29723d51f4e8a8880c8d9c81277b793aa04cff648cf34959db4f805635`  
		Last Modified: Thu, 16 Jan 2020 21:20:38 GMT  
		Size: 62.0 MB (62034537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d458e146b5ee0e1d86be6bce69699664b33a9c6ea4776c15f025a46120ce49`  
		Last Modified: Thu, 16 Jan 2020 21:21:13 GMT  
		Size: 326.1 MB (326128681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20200304.0`

```console
$ docker pull amazonlinux@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `amazonlinux:2.0.20200304.0-with-sources`

```console
$ docker pull amazonlinux@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:cb2197f3097f3900a36bf572b2805b3272eff03b617e48cc7fe60f1ab6c763bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:50c28a33157555b4372c1e98cd9c70c161e78e944683322bbfb2b8f44c7729ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476800172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c25bb04918e2ddc50ce74762ffbc0c89b25cd45ba721f2798a172c42234316c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Feb 2020 23:19:52 GMT
ADD file:c43f05fa78d78f998cd8e2e45f089e0572877490c7df425e514d44f15d958fad in / 
# Wed, 19 Feb 2020 23:19:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Feb 2020 23:20:16 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9d577ed8f0e2cbd076b6f144ec0c470c9c81012109b3d19515b8287114f96859.tar.gz"  && echo "88b2385d08e0f3df72a3d6b411c6b418af927ef411549cea48a3dfd887bf0f29  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a7583ef20c9db3e6539d4160e9914383701901b24979656a228000718b0d5bea`  
		Last Modified: Wed, 19 Feb 2020 23:20:55 GMT  
		Size: 61.7 MB (61669860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696d5ea6c170fee8b13d7cc50cf08e8da5934fb7ebec062fbcd1db4171450be`  
		Last Modified: Wed, 19 Feb 2020 23:21:19 GMT  
		Size: 415.1 MB (415130312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:14dbc80a40025e5418a8635a18a5bce9c7337211057ca7626d03d83bda7c7b13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478193302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bacff54cac3e0a26b7b6e3738fd6a9517c85f215b8d05d3202ebee5dd1e81309`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Feb 2020 22:39:49 GMT
ADD file:bf00dcc4d3caeda14a7a6b3afb7f5dca29d64b43fe428f5713b88cec1a82f2a0 in / 
# Wed, 19 Feb 2020 22:39:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Feb 2020 22:40:17 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9d577ed8f0e2cbd076b6f144ec0c470c9c81012109b3d19515b8287114f96859.tar.gz"  && echo "88b2385d08e0f3df72a3d6b411c6b418af927ef411549cea48a3dfd887bf0f29  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7f2fa3024eb129e832d7fd7cee7209fdab8adadbc3dc31675f191ac0414fb93c`  
		Last Modified: Wed, 19 Feb 2020 22:40:47 GMT  
		Size: 63.1 MB (63062950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f38b153acbda095a943079f45ede45d802f3e3d6cfd1cf21c113a65da7d45f6`  
		Last Modified: Wed, 19 Feb 2020 22:41:35 GMT  
		Size: 415.1 MB (415130352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:88a720de445a49a039bf9817af06e93c95e36f438bb8d72c15fb5a9bcae86bd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0df02385ce8946ad27fa935b969002302d11dfb13c91c3c4f7c39473a737226b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61669860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:484b3aa1f6013f8ca133c20951b1b3b6b74da20cc0958ca474155852ac96b32d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Feb 2020 23:19:52 GMT
ADD file:c43f05fa78d78f998cd8e2e45f089e0572877490c7df425e514d44f15d958fad in / 
# Wed, 19 Feb 2020 23:19:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a7583ef20c9db3e6539d4160e9914383701901b24979656a228000718b0d5bea`  
		Last Modified: Wed, 19 Feb 2020 23:20:55 GMT  
		Size: 61.7 MB (61669860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:d9eb6060c8db3e70dd3452cbb2fca47f35a9e5cfde7ea7f3eeafb36d38dbb47f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63062950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63dbb02acf93525b5be87cc28bcf5cfaa5057ff67047bfd9e5182d3fc3c94fc4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Feb 2020 22:39:49 GMT
ADD file:bf00dcc4d3caeda14a7a6b3afb7f5dca29d64b43fe428f5713b88cec1a82f2a0 in / 
# Wed, 19 Feb 2020 22:39:52 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:7f2fa3024eb129e832d7fd7cee7209fdab8adadbc3dc31675f191ac0414fb93c`  
		Last Modified: Wed, 19 Feb 2020 22:40:47 GMT  
		Size: 63.1 MB (63062950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:cb2197f3097f3900a36bf572b2805b3272eff03b617e48cc7fe60f1ab6c763bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:50c28a33157555b4372c1e98cd9c70c161e78e944683322bbfb2b8f44c7729ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476800172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c25bb04918e2ddc50ce74762ffbc0c89b25cd45ba721f2798a172c42234316c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Feb 2020 23:19:52 GMT
ADD file:c43f05fa78d78f998cd8e2e45f089e0572877490c7df425e514d44f15d958fad in / 
# Wed, 19 Feb 2020 23:19:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Feb 2020 23:20:16 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9d577ed8f0e2cbd076b6f144ec0c470c9c81012109b3d19515b8287114f96859.tar.gz"  && echo "88b2385d08e0f3df72a3d6b411c6b418af927ef411549cea48a3dfd887bf0f29  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a7583ef20c9db3e6539d4160e9914383701901b24979656a228000718b0d5bea`  
		Last Modified: Wed, 19 Feb 2020 23:20:55 GMT  
		Size: 61.7 MB (61669860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696d5ea6c170fee8b13d7cc50cf08e8da5934fb7ebec062fbcd1db4171450be`  
		Last Modified: Wed, 19 Feb 2020 23:21:19 GMT  
		Size: 415.1 MB (415130312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:14dbc80a40025e5418a8635a18a5bce9c7337211057ca7626d03d83bda7c7b13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478193302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bacff54cac3e0a26b7b6e3738fd6a9517c85f215b8d05d3202ebee5dd1e81309`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Feb 2020 22:39:49 GMT
ADD file:bf00dcc4d3caeda14a7a6b3afb7f5dca29d64b43fe428f5713b88cec1a82f2a0 in / 
# Wed, 19 Feb 2020 22:39:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Feb 2020 22:40:17 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-9d577ed8f0e2cbd076b6f144ec0c470c9c81012109b3d19515b8287114f96859.tar.gz"  && echo "88b2385d08e0f3df72a3d6b411c6b418af927ef411549cea48a3dfd887bf0f29  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:7f2fa3024eb129e832d7fd7cee7209fdab8adadbc3dc31675f191ac0414fb93c`  
		Last Modified: Wed, 19 Feb 2020 22:40:47 GMT  
		Size: 63.1 MB (63062950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f38b153acbda095a943079f45ede45d802f3e3d6cfd1cf21c113a65da7d45f6`  
		Last Modified: Wed, 19 Feb 2020 22:41:35 GMT  
		Size: 415.1 MB (415130352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
