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
$ docker pull amazonlinux@sha256:45a9caadc960d8345066ffe74f1b13f5a6e713e4b91d8a86cc7c331e47bedc9a
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
$ docker pull amazonlinux@sha256:13b345bea4a238e53966ef3f2e0c2586e6c12ecc1dc73155c2538befa4d03276
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63072580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e46d9cf7e04cc6828bbcc8acec3828b5b3aeb2c6b37d78549e26ac882dac0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
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
$ docker pull amazonlinux@sha256:1b51d90dc3ef35a03e35a5af28629d4bf9a31ff5fb5561bb31e09760c07a4d7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20200304.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:13b345bea4a238e53966ef3f2e0c2586e6c12ecc1dc73155c2538befa4d03276
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63072580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e46d9cf7e04cc6828bbcc8acec3828b5b3aeb2c6b37d78549e26ac882dac0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20200304.0-with-sources`

```console
$ docker pull amazonlinux@sha256:0ad4b6fbc378de3842366242e0c8b43a3f895790fbf7530b398446c7bf486ebe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20200304.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:20b1a9fe34ca33f2c1aacc4343fa97b0771d30ca2205167addab44c976fd726c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478210702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e2dcdd719c4bfad05508a36c20f7d8100b941816a39367f4b3b4cedb6d39431`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 05:23:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-4cda1b0d98865d12f61886af2ff052cf2cb4a48734bded0ac84d2664a0361220.tar.gz"  && echo "c53ef45b008bcb392f9ecbd229a6fa38f69cfe536d630560a8e1a8daaa8b68e6  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f5263e197d28b470047a0d5a85c7de9ceb69e2107bcc4eba8d080aef3bfa95`  
		Last Modified: Wed, 01 Apr 2020 05:24:46 GMT  
		Size: 415.1 MB (415138122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:26c08e4d8fcf09bfad0c3c35f1608e8acfb07cbef8d5ac87c111ce10579d11d0
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
$ docker pull amazonlinux@sha256:20b1a9fe34ca33f2c1aacc4343fa97b0771d30ca2205167addab44c976fd726c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478210702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e2dcdd719c4bfad05508a36c20f7d8100b941816a39367f4b3b4cedb6d39431`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 05:23:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-4cda1b0d98865d12f61886af2ff052cf2cb4a48734bded0ac84d2664a0361220.tar.gz"  && echo "c53ef45b008bcb392f9ecbd229a6fa38f69cfe536d630560a8e1a8daaa8b68e6  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f5263e197d28b470047a0d5a85c7de9ceb69e2107bcc4eba8d080aef3bfa95`  
		Last Modified: Wed, 01 Apr 2020 05:24:46 GMT  
		Size: 415.1 MB (415138122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:45a9caadc960d8345066ffe74f1b13f5a6e713e4b91d8a86cc7c331e47bedc9a
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
$ docker pull amazonlinux@sha256:13b345bea4a238e53966ef3f2e0c2586e6c12ecc1dc73155c2538befa4d03276
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63072580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e46d9cf7e04cc6828bbcc8acec3828b5b3aeb2c6b37d78549e26ac882dac0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:26c08e4d8fcf09bfad0c3c35f1608e8acfb07cbef8d5ac87c111ce10579d11d0
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
$ docker pull amazonlinux@sha256:20b1a9fe34ca33f2c1aacc4343fa97b0771d30ca2205167addab44c976fd726c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478210702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e2dcdd719c4bfad05508a36c20f7d8100b941816a39367f4b3b4cedb6d39431`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 05:23:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-4cda1b0d98865d12f61886af2ff052cf2cb4a48734bded0ac84d2664a0361220.tar.gz"  && echo "c53ef45b008bcb392f9ecbd229a6fa38f69cfe536d630560a8e1a8daaa8b68e6  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f5263e197d28b470047a0d5a85c7de9ceb69e2107bcc4eba8d080aef3bfa95`  
		Last Modified: Wed, 01 Apr 2020 05:24:46 GMT  
		Size: 415.1 MB (415138122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
