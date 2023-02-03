<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20230119.1`](#amazonlinux20202301191)
-	[`amazonlinux:2.0.20230119.1-with-sources`](#amazonlinux20202301191-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20230124.1`](#amazonlinux2018030202301241)
-	[`amazonlinux:2018.03.0.20230124.1-with-sources`](#amazonlinux2018030202301241-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20230118.3`](#amazonlinux20220202301183)
-	[`amazonlinux:2022.0.20230118.3-with-sources`](#amazonlinux20220202301183-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:3a31e03432ef61ce54faac0cdcedf44d1cd93bab1f927c55587626ac729a352d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:70dda6dc87f1b3279393af31709f5a9a1dfd83a8c32f1c84c378c700a2870770
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62255374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a1fb356be0b186bcc23105e5869f2581fcaee8e4deaabca5b9354d70a191a9c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 05:17:05 GMT
ADD file:165da0f747d5bb8a5b24aeec2a50d25873475dd1c4e2552a0ab59ffc9af2488c in / 
# Wed, 01 Feb 2023 05:17:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3e051ffffb66f948f07ba2db2e3360f6a4343f61c5575d7b569fc1c94775cbf5`  
		Last Modified: Wed, 01 Feb 2023 05:18:09 GMT  
		Size: 62.3 MB (62255374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:9503466ae911d6d77ac747764f6464fbf2b728c59fb14324e2766ae6f9280c1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:616a099584c9a4ed315ce962208814ca53212cf67985aebf8b5206a53125f382
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (514989737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10744eddd6741de6ffab97ff9f68b81f59fc7844510c0f57794411f6dd2c655d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 05:17:05 GMT
ADD file:165da0f747d5bb8a5b24aeec2a50d25873475dd1c4e2552a0ab59ffc9af2488c in / 
# Wed, 01 Feb 2023 05:17:05 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 05:17:29 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2ed4106e01cfeb1719871304503f68d7fb9b69a826163f974f641b609b98e3f8.tar.gz"     && echo "9183fb7e1c04cd92db6be2c006030b8cbddf8e42bdb9cd0e31e06d89fd79ca60  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3e051ffffb66f948f07ba2db2e3360f6a4343f61c5575d7b569fc1c94775cbf5`  
		Last Modified: Wed, 01 Feb 2023 05:18:09 GMT  
		Size: 62.3 MB (62255374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1333bc317469bfd8da3894f3a10ebba3bd13fc2946a199b16b4dc205688571aa`  
		Last Modified: Wed, 01 Feb 2023 05:18:37 GMT  
		Size: 452.7 MB (452734363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:66d22a2b8749283aa0764e6983fbb8bf8c143511cf16c9773598acca2a1cd6d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:db0bf55c548efbbb167c60ced2eb0ca60769de293667d18b92c0c089b8038279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62341068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92310fbb9f4cb6ae7cbbfc7fdb22d61f35279bd4ceae30d7cf7dcddb9e5b2e41`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:20:04 GMT
ADD file:6ebab25a4f1aa82238dbf1a48f38d22c6421052d0d158cf88cbc1a4d01b5c5c1 in / 
# Thu, 26 Jan 2023 22:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1e78b99dd1fd1031c6513834c4b5f594fa3cec5d06cdeb4b65ee104180bc0d4c`  
		Last Modified: Thu, 26 Jan 2023 20:44:53 GMT  
		Size: 62.3 MB (62341068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:edfe6cc6ed773f9fafef779b8fe925b127c3e811e46367b3a851536a48d6613b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (63964642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa2bfcf82b27a574cd54b7a50d459fa2cacc70b68410e0f46cafa32f1319c65`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:39:30 GMT
ADD file:1b056f516caefc99e89cee1ffa2d3b98a54ec5756d3c54b0b1c75c6ddfa9e1ae in / 
# Thu, 26 Jan 2023 22:39:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f211bebb41ee40fd8a6c26d9c71d47a936d9684219f14a2679e8f57c07bb49b6`  
		Last Modified: Thu, 26 Jan 2023 22:40:24 GMT  
		Size: 64.0 MB (63964642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:62b13a9eaba6c742134ffc4fd47fa4074441831519ae4076a3b4b2adbd197448
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2d38587453f08b16b63169a66451ee34d0934db2399ee95c2614e86a5a7dae1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.5 MB (492531606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad43da7b8649e85abd2f228c42dfa04e55336f23d3af0f78794e4307de8d545f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:20:04 GMT
ADD file:6ebab25a4f1aa82238dbf1a48f38d22c6421052d0d158cf88cbc1a4d01b5c5c1 in / 
# Thu, 26 Jan 2023 22:20:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Jan 2023 22:20:30 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5f290fbb01ed6cae6ec9436094897096f0cd61aa0fb90afb412045f989363faa.tar.gz"     && echo "a2345704122103f0cf035d1ae3d4fa863db8c73c0f08e6f8656f5ac9274b0eba  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:1e78b99dd1fd1031c6513834c4b5f594fa3cec5d06cdeb4b65ee104180bc0d4c`  
		Last Modified: Thu, 26 Jan 2023 20:44:53 GMT  
		Size: 62.3 MB (62341068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9c62719ce9a736ff6f49a8d84be8316820a6035ab43ac69eaafb9ec7975bcd`  
		Last Modified: Thu, 26 Jan 2023 22:21:33 GMT  
		Size: 430.2 MB (430190538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:abcef3933194055013b7b02644b7ab3ca2ac28625e48190cfeda61595fffe67f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **494.2 MB (494155176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0726baa057a47e2e49ea7a98d3a8206bde79fd1225f738ccfc73ba0fd69eef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:39:30 GMT
ADD file:1b056f516caefc99e89cee1ffa2d3b98a54ec5756d3c54b0b1c75c6ddfa9e1ae in / 
# Thu, 26 Jan 2023 22:39:31 GMT
CMD ["/bin/bash"]
# Thu, 26 Jan 2023 22:39:53 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5f290fbb01ed6cae6ec9436094897096f0cd61aa0fb90afb412045f989363faa.tar.gz"     && echo "a2345704122103f0cf035d1ae3d4fa863db8c73c0f08e6f8656f5ac9274b0eba  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f211bebb41ee40fd8a6c26d9c71d47a936d9684219f14a2679e8f57c07bb49b6`  
		Last Modified: Thu, 26 Jan 2023 22:40:24 GMT  
		Size: 64.0 MB (63964642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9850613c66f695c4d0de595f9359ad654f83678bbe4f57664bf76827b8ca00`  
		Last Modified: Thu, 26 Jan 2023 22:40:47 GMT  
		Size: 430.2 MB (430190534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20230119.1`

```console
$ docker pull amazonlinux@sha256:66d22a2b8749283aa0764e6983fbb8bf8c143511cf16c9773598acca2a1cd6d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20230119.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:db0bf55c548efbbb167c60ced2eb0ca60769de293667d18b92c0c089b8038279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62341068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92310fbb9f4cb6ae7cbbfc7fdb22d61f35279bd4ceae30d7cf7dcddb9e5b2e41`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:20:04 GMT
ADD file:6ebab25a4f1aa82238dbf1a48f38d22c6421052d0d158cf88cbc1a4d01b5c5c1 in / 
# Thu, 26 Jan 2023 22:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1e78b99dd1fd1031c6513834c4b5f594fa3cec5d06cdeb4b65ee104180bc0d4c`  
		Last Modified: Thu, 26 Jan 2023 20:44:53 GMT  
		Size: 62.3 MB (62341068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20230119.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:edfe6cc6ed773f9fafef779b8fe925b127c3e811e46367b3a851536a48d6613b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (63964642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa2bfcf82b27a574cd54b7a50d459fa2cacc70b68410e0f46cafa32f1319c65`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:39:30 GMT
ADD file:1b056f516caefc99e89cee1ffa2d3b98a54ec5756d3c54b0b1c75c6ddfa9e1ae in / 
# Thu, 26 Jan 2023 22:39:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f211bebb41ee40fd8a6c26d9c71d47a936d9684219f14a2679e8f57c07bb49b6`  
		Last Modified: Thu, 26 Jan 2023 22:40:24 GMT  
		Size: 64.0 MB (63964642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20230119.1-with-sources`

```console
$ docker pull amazonlinux@sha256:62b13a9eaba6c742134ffc4fd47fa4074441831519ae4076a3b4b2adbd197448
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20230119.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2d38587453f08b16b63169a66451ee34d0934db2399ee95c2614e86a5a7dae1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.5 MB (492531606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad43da7b8649e85abd2f228c42dfa04e55336f23d3af0f78794e4307de8d545f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:20:04 GMT
ADD file:6ebab25a4f1aa82238dbf1a48f38d22c6421052d0d158cf88cbc1a4d01b5c5c1 in / 
# Thu, 26 Jan 2023 22:20:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Jan 2023 22:20:30 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5f290fbb01ed6cae6ec9436094897096f0cd61aa0fb90afb412045f989363faa.tar.gz"     && echo "a2345704122103f0cf035d1ae3d4fa863db8c73c0f08e6f8656f5ac9274b0eba  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:1e78b99dd1fd1031c6513834c4b5f594fa3cec5d06cdeb4b65ee104180bc0d4c`  
		Last Modified: Thu, 26 Jan 2023 20:44:53 GMT  
		Size: 62.3 MB (62341068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9c62719ce9a736ff6f49a8d84be8316820a6035ab43ac69eaafb9ec7975bcd`  
		Last Modified: Thu, 26 Jan 2023 22:21:33 GMT  
		Size: 430.2 MB (430190538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20230119.1-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:abcef3933194055013b7b02644b7ab3ca2ac28625e48190cfeda61595fffe67f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **494.2 MB (494155176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0726baa057a47e2e49ea7a98d3a8206bde79fd1225f738ccfc73ba0fd69eef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:39:30 GMT
ADD file:1b056f516caefc99e89cee1ffa2d3b98a54ec5756d3c54b0b1c75c6ddfa9e1ae in / 
# Thu, 26 Jan 2023 22:39:31 GMT
CMD ["/bin/bash"]
# Thu, 26 Jan 2023 22:39:53 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5f290fbb01ed6cae6ec9436094897096f0cd61aa0fb90afb412045f989363faa.tar.gz"     && echo "a2345704122103f0cf035d1ae3d4fa863db8c73c0f08e6f8656f5ac9274b0eba  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f211bebb41ee40fd8a6c26d9c71d47a936d9684219f14a2679e8f57c07bb49b6`  
		Last Modified: Thu, 26 Jan 2023 22:40:24 GMT  
		Size: 64.0 MB (63964642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9850613c66f695c4d0de595f9359ad654f83678bbe4f57664bf76827b8ca00`  
		Last Modified: Thu, 26 Jan 2023 22:40:47 GMT  
		Size: 430.2 MB (430190534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:3a31e03432ef61ce54faac0cdcedf44d1cd93bab1f927c55587626ac729a352d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:70dda6dc87f1b3279393af31709f5a9a1dfd83a8c32f1c84c378c700a2870770
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62255374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a1fb356be0b186bcc23105e5869f2581fcaee8e4deaabca5b9354d70a191a9c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 05:17:05 GMT
ADD file:165da0f747d5bb8a5b24aeec2a50d25873475dd1c4e2552a0ab59ffc9af2488c in / 
# Wed, 01 Feb 2023 05:17:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3e051ffffb66f948f07ba2db2e3360f6a4343f61c5575d7b569fc1c94775cbf5`  
		Last Modified: Wed, 01 Feb 2023 05:18:09 GMT  
		Size: 62.3 MB (62255374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:9503466ae911d6d77ac747764f6464fbf2b728c59fb14324e2766ae6f9280c1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:616a099584c9a4ed315ce962208814ca53212cf67985aebf8b5206a53125f382
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (514989737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10744eddd6741de6ffab97ff9f68b81f59fc7844510c0f57794411f6dd2c655d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 05:17:05 GMT
ADD file:165da0f747d5bb8a5b24aeec2a50d25873475dd1c4e2552a0ab59ffc9af2488c in / 
# Wed, 01 Feb 2023 05:17:05 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 05:17:29 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2ed4106e01cfeb1719871304503f68d7fb9b69a826163f974f641b609b98e3f8.tar.gz"     && echo "9183fb7e1c04cd92db6be2c006030b8cbddf8e42bdb9cd0e31e06d89fd79ca60  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3e051ffffb66f948f07ba2db2e3360f6a4343f61c5575d7b569fc1c94775cbf5`  
		Last Modified: Wed, 01 Feb 2023 05:18:09 GMT  
		Size: 62.3 MB (62255374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1333bc317469bfd8da3894f3a10ebba3bd13fc2946a199b16b4dc205688571aa`  
		Last Modified: Wed, 01 Feb 2023 05:18:37 GMT  
		Size: 452.7 MB (452734363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20230124.1`

```console
$ docker pull amazonlinux@sha256:3a31e03432ef61ce54faac0cdcedf44d1cd93bab1f927c55587626ac729a352d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20230124.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:70dda6dc87f1b3279393af31709f5a9a1dfd83a8c32f1c84c378c700a2870770
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62255374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a1fb356be0b186bcc23105e5869f2581fcaee8e4deaabca5b9354d70a191a9c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 05:17:05 GMT
ADD file:165da0f747d5bb8a5b24aeec2a50d25873475dd1c4e2552a0ab59ffc9af2488c in / 
# Wed, 01 Feb 2023 05:17:05 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3e051ffffb66f948f07ba2db2e3360f6a4343f61c5575d7b569fc1c94775cbf5`  
		Last Modified: Wed, 01 Feb 2023 05:18:09 GMT  
		Size: 62.3 MB (62255374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20230124.1-with-sources`

```console
$ docker pull amazonlinux@sha256:9503466ae911d6d77ac747764f6464fbf2b728c59fb14324e2766ae6f9280c1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03.0.20230124.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:616a099584c9a4ed315ce962208814ca53212cf67985aebf8b5206a53125f382
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (514989737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10744eddd6741de6ffab97ff9f68b81f59fc7844510c0f57794411f6dd2c655d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Feb 2023 05:17:05 GMT
ADD file:165da0f747d5bb8a5b24aeec2a50d25873475dd1c4e2552a0ab59ffc9af2488c in / 
# Wed, 01 Feb 2023 05:17:05 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 05:17:29 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-2ed4106e01cfeb1719871304503f68d7fb9b69a826163f974f641b609b98e3f8.tar.gz"     && echo "9183fb7e1c04cd92db6be2c006030b8cbddf8e42bdb9cd0e31e06d89fd79ca60  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3e051ffffb66f948f07ba2db2e3360f6a4343f61c5575d7b569fc1c94775cbf5`  
		Last Modified: Wed, 01 Feb 2023 05:18:09 GMT  
		Size: 62.3 MB (62255374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1333bc317469bfd8da3894f3a10ebba3bd13fc2946a199b16b4dc205688571aa`  
		Last Modified: Wed, 01 Feb 2023 05:18:37 GMT  
		Size: 452.7 MB (452734363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:52a0dc20e07b3a70a9aca4b8f3690ab3383819c1e0ec0508e7f5a18279bc0873
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c09be3439eb2f0aa95355fbf59f6c33753f77022ac06e71f9a10507099dd2cde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57916237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2748fd231f3d65fea95fa89d239d40006782a4e865ab98ff4eadead624915d7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:19:36 GMT
ADD file:98ef92cdf32a39d761092e3dbc916e083179c438c365e21a2ea68b801a3f595d in / 
# Thu, 02 Feb 2023 20:19:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:044c2e2e5f7c74ee29fba14bd0c17aba2da682d4bb1f235b6efaeb7365c09814`  
		Last Modified: Thu, 02 Feb 2023 20:20:38 GMT  
		Size: 57.9 MB (57916237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:66dec6cf6570aeb14bfaf4a1e4f294a82dfc403d86a9b375caf06301211f030d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56810570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ac05fbc302afa4b33f0f00fdb304bd40f34b1deb9f2335b93d004aa232be0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:39:44 GMT
ADD file:9f05ba021fffd82beb2a9d0ea647b83648b1bfd0e607557faab2356c813fb362 in / 
# Thu, 02 Feb 2023 20:39:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:838e33db41c437b283f45c5b41cf3cfe56026082e5c47e55eed49ec433af394c`  
		Last Modified: Tue, 31 Jan 2023 12:25:16 GMT  
		Size: 56.8 MB (56810570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:37d568a1e8e46481763223db859dae55eedd4aa86ece9de6f0da7d38e7d6d2a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:12ecc5ecdbe5395b1515094ad80bdaa720034caefb3d09f69c49ad7f28babcb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.0 MB (392016191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53819a0095a6146d5cbcd2ea2874c210e83cd0ef869a9539c08f245089f75a9d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:19:36 GMT
ADD file:98ef92cdf32a39d761092e3dbc916e083179c438c365e21a2ea68b801a3f595d in / 
# Thu, 02 Feb 2023 20:19:37 GMT
CMD ["/bin/bash"]
# Thu, 02 Feb 2023 20:19:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1b0dd271d54be9dbb3fcfa0b37f2c0ec0cee4279b55d596ff37915e26ad6a533.tar.gz"     && echo "6a05192a5bdf55ee6b82715c027521a534bef1cc3b45b3b9b07fda0700fb583f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:044c2e2e5f7c74ee29fba14bd0c17aba2da682d4bb1f235b6efaeb7365c09814`  
		Last Modified: Thu, 02 Feb 2023 20:20:38 GMT  
		Size: 57.9 MB (57916237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a290d90a538e5f8c06ed51ada1dcf0fa26fe3322bf1917b55769086b8ec613a0`  
		Last Modified: Thu, 02 Feb 2023 20:21:02 GMT  
		Size: 334.1 MB (334099954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2ae114e4c7fc0532d78268efaa7116b3da72cf053843068ac6e2da54c098f592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.9 MB (390910524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:576e65a2c6d2c6a6d838569b1c09d4f95e3f1459e67179429429b373fe2a9425`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:39:44 GMT
ADD file:9f05ba021fffd82beb2a9d0ea647b83648b1bfd0e607557faab2356c813fb362 in / 
# Thu, 02 Feb 2023 20:39:44 GMT
CMD ["/bin/bash"]
# Thu, 02 Feb 2023 20:40:07 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1b0dd271d54be9dbb3fcfa0b37f2c0ec0cee4279b55d596ff37915e26ad6a533.tar.gz"     && echo "6a05192a5bdf55ee6b82715c027521a534bef1cc3b45b3b9b07fda0700fb583f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:838e33db41c437b283f45c5b41cf3cfe56026082e5c47e55eed49ec433af394c`  
		Last Modified: Tue, 31 Jan 2023 12:25:16 GMT  
		Size: 56.8 MB (56810570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a25acb53d1cf2874625ad374a8810cd2ada6730cc44f0118c43cbf60382fd6`  
		Last Modified: Thu, 02 Feb 2023 20:41:01 GMT  
		Size: 334.1 MB (334099954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20230118.3`

```console
$ docker pull amazonlinux@sha256:52a0dc20e07b3a70a9aca4b8f3690ab3383819c1e0ec0508e7f5a18279bc0873
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20230118.3` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c09be3439eb2f0aa95355fbf59f6c33753f77022ac06e71f9a10507099dd2cde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57916237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2748fd231f3d65fea95fa89d239d40006782a4e865ab98ff4eadead624915d7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:19:36 GMT
ADD file:98ef92cdf32a39d761092e3dbc916e083179c438c365e21a2ea68b801a3f595d in / 
# Thu, 02 Feb 2023 20:19:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:044c2e2e5f7c74ee29fba14bd0c17aba2da682d4bb1f235b6efaeb7365c09814`  
		Last Modified: Thu, 02 Feb 2023 20:20:38 GMT  
		Size: 57.9 MB (57916237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20230118.3` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:66dec6cf6570aeb14bfaf4a1e4f294a82dfc403d86a9b375caf06301211f030d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56810570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ac05fbc302afa4b33f0f00fdb304bd40f34b1deb9f2335b93d004aa232be0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:39:44 GMT
ADD file:9f05ba021fffd82beb2a9d0ea647b83648b1bfd0e607557faab2356c813fb362 in / 
# Thu, 02 Feb 2023 20:39:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:838e33db41c437b283f45c5b41cf3cfe56026082e5c47e55eed49ec433af394c`  
		Last Modified: Tue, 31 Jan 2023 12:25:16 GMT  
		Size: 56.8 MB (56810570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20230118.3-with-sources`

```console
$ docker pull amazonlinux@sha256:37d568a1e8e46481763223db859dae55eedd4aa86ece9de6f0da7d38e7d6d2a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20230118.3-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:12ecc5ecdbe5395b1515094ad80bdaa720034caefb3d09f69c49ad7f28babcb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.0 MB (392016191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53819a0095a6146d5cbcd2ea2874c210e83cd0ef869a9539c08f245089f75a9d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:19:36 GMT
ADD file:98ef92cdf32a39d761092e3dbc916e083179c438c365e21a2ea68b801a3f595d in / 
# Thu, 02 Feb 2023 20:19:37 GMT
CMD ["/bin/bash"]
# Thu, 02 Feb 2023 20:19:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1b0dd271d54be9dbb3fcfa0b37f2c0ec0cee4279b55d596ff37915e26ad6a533.tar.gz"     && echo "6a05192a5bdf55ee6b82715c027521a534bef1cc3b45b3b9b07fda0700fb583f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:044c2e2e5f7c74ee29fba14bd0c17aba2da682d4bb1f235b6efaeb7365c09814`  
		Last Modified: Thu, 02 Feb 2023 20:20:38 GMT  
		Size: 57.9 MB (57916237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a290d90a538e5f8c06ed51ada1dcf0fa26fe3322bf1917b55769086b8ec613a0`  
		Last Modified: Thu, 02 Feb 2023 20:21:02 GMT  
		Size: 334.1 MB (334099954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20230118.3-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2ae114e4c7fc0532d78268efaa7116b3da72cf053843068ac6e2da54c098f592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.9 MB (390910524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:576e65a2c6d2c6a6d838569b1c09d4f95e3f1459e67179429429b373fe2a9425`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:39:44 GMT
ADD file:9f05ba021fffd82beb2a9d0ea647b83648b1bfd0e607557faab2356c813fb362 in / 
# Thu, 02 Feb 2023 20:39:44 GMT
CMD ["/bin/bash"]
# Thu, 02 Feb 2023 20:40:07 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1b0dd271d54be9dbb3fcfa0b37f2c0ec0cee4279b55d596ff37915e26ad6a533.tar.gz"     && echo "6a05192a5bdf55ee6b82715c027521a534bef1cc3b45b3b9b07fda0700fb583f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:838e33db41c437b283f45c5b41cf3cfe56026082e5c47e55eed49ec433af394c`  
		Last Modified: Tue, 31 Jan 2023 12:25:16 GMT  
		Size: 56.8 MB (56810570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a25acb53d1cf2874625ad374a8810cd2ada6730cc44f0118c43cbf60382fd6`  
		Last Modified: Thu, 02 Feb 2023 20:41:01 GMT  
		Size: 334.1 MB (334099954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:52a0dc20e07b3a70a9aca4b8f3690ab3383819c1e0ec0508e7f5a18279bc0873
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c09be3439eb2f0aa95355fbf59f6c33753f77022ac06e71f9a10507099dd2cde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57916237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2748fd231f3d65fea95fa89d239d40006782a4e865ab98ff4eadead624915d7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:19:36 GMT
ADD file:98ef92cdf32a39d761092e3dbc916e083179c438c365e21a2ea68b801a3f595d in / 
# Thu, 02 Feb 2023 20:19:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:044c2e2e5f7c74ee29fba14bd0c17aba2da682d4bb1f235b6efaeb7365c09814`  
		Last Modified: Thu, 02 Feb 2023 20:20:38 GMT  
		Size: 57.9 MB (57916237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:66dec6cf6570aeb14bfaf4a1e4f294a82dfc403d86a9b375caf06301211f030d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56810570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ac05fbc302afa4b33f0f00fdb304bd40f34b1deb9f2335b93d004aa232be0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:39:44 GMT
ADD file:9f05ba021fffd82beb2a9d0ea647b83648b1bfd0e607557faab2356c813fb362 in / 
# Thu, 02 Feb 2023 20:39:44 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:838e33db41c437b283f45c5b41cf3cfe56026082e5c47e55eed49ec433af394c`  
		Last Modified: Tue, 31 Jan 2023 12:25:16 GMT  
		Size: 56.8 MB (56810570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:37d568a1e8e46481763223db859dae55eedd4aa86ece9de6f0da7d38e7d6d2a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:12ecc5ecdbe5395b1515094ad80bdaa720034caefb3d09f69c49ad7f28babcb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.0 MB (392016191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53819a0095a6146d5cbcd2ea2874c210e83cd0ef869a9539c08f245089f75a9d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:19:36 GMT
ADD file:98ef92cdf32a39d761092e3dbc916e083179c438c365e21a2ea68b801a3f595d in / 
# Thu, 02 Feb 2023 20:19:37 GMT
CMD ["/bin/bash"]
# Thu, 02 Feb 2023 20:19:59 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1b0dd271d54be9dbb3fcfa0b37f2c0ec0cee4279b55d596ff37915e26ad6a533.tar.gz"     && echo "6a05192a5bdf55ee6b82715c027521a534bef1cc3b45b3b9b07fda0700fb583f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:044c2e2e5f7c74ee29fba14bd0c17aba2da682d4bb1f235b6efaeb7365c09814`  
		Last Modified: Thu, 02 Feb 2023 20:20:38 GMT  
		Size: 57.9 MB (57916237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a290d90a538e5f8c06ed51ada1dcf0fa26fe3322bf1917b55769086b8ec613a0`  
		Last Modified: Thu, 02 Feb 2023 20:21:02 GMT  
		Size: 334.1 MB (334099954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:2ae114e4c7fc0532d78268efaa7116b3da72cf053843068ac6e2da54c098f592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.9 MB (390910524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:576e65a2c6d2c6a6d838569b1c09d4f95e3f1459e67179429429b373fe2a9425`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 02 Feb 2023 20:39:44 GMT
ADD file:9f05ba021fffd82beb2a9d0ea647b83648b1bfd0e607557faab2356c813fb362 in / 
# Thu, 02 Feb 2023 20:39:44 GMT
CMD ["/bin/bash"]
# Thu, 02 Feb 2023 20:40:07 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1b0dd271d54be9dbb3fcfa0b37f2c0ec0cee4279b55d596ff37915e26ad6a533.tar.gz"     && echo "6a05192a5bdf55ee6b82715c027521a534bef1cc3b45b3b9b07fda0700fb583f  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:838e33db41c437b283f45c5b41cf3cfe56026082e5c47e55eed49ec433af394c`  
		Last Modified: Tue, 31 Jan 2023 12:25:16 GMT  
		Size: 56.8 MB (56810570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a25acb53d1cf2874625ad374a8810cd2ada6730cc44f0118c43cbf60382fd6`  
		Last Modified: Thu, 02 Feb 2023 20:41:01 GMT  
		Size: 334.1 MB (334099954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:66d22a2b8749283aa0764e6983fbb8bf8c143511cf16c9773598acca2a1cd6d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:db0bf55c548efbbb167c60ced2eb0ca60769de293667d18b92c0c089b8038279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62341068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92310fbb9f4cb6ae7cbbfc7fdb22d61f35279bd4ceae30d7cf7dcddb9e5b2e41`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:20:04 GMT
ADD file:6ebab25a4f1aa82238dbf1a48f38d22c6421052d0d158cf88cbc1a4d01b5c5c1 in / 
# Thu, 26 Jan 2023 22:20:04 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:1e78b99dd1fd1031c6513834c4b5f594fa3cec5d06cdeb4b65ee104180bc0d4c`  
		Last Modified: Thu, 26 Jan 2023 20:44:53 GMT  
		Size: 62.3 MB (62341068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:edfe6cc6ed773f9fafef779b8fe925b127c3e811e46367b3a851536a48d6613b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.0 MB (63964642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa2bfcf82b27a574cd54b7a50d459fa2cacc70b68410e0f46cafa32f1319c65`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:39:30 GMT
ADD file:1b056f516caefc99e89cee1ffa2d3b98a54ec5756d3c54b0b1c75c6ddfa9e1ae in / 
# Thu, 26 Jan 2023 22:39:31 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f211bebb41ee40fd8a6c26d9c71d47a936d9684219f14a2679e8f57c07bb49b6`  
		Last Modified: Thu, 26 Jan 2023 22:40:24 GMT  
		Size: 64.0 MB (63964642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:62b13a9eaba6c742134ffc4fd47fa4074441831519ae4076a3b4b2adbd197448
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2d38587453f08b16b63169a66451ee34d0934db2399ee95c2614e86a5a7dae1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.5 MB (492531606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad43da7b8649e85abd2f228c42dfa04e55336f23d3af0f78794e4307de8d545f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:20:04 GMT
ADD file:6ebab25a4f1aa82238dbf1a48f38d22c6421052d0d158cf88cbc1a4d01b5c5c1 in / 
# Thu, 26 Jan 2023 22:20:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Jan 2023 22:20:30 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5f290fbb01ed6cae6ec9436094897096f0cd61aa0fb90afb412045f989363faa.tar.gz"     && echo "a2345704122103f0cf035d1ae3d4fa863db8c73c0f08e6f8656f5ac9274b0eba  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:1e78b99dd1fd1031c6513834c4b5f594fa3cec5d06cdeb4b65ee104180bc0d4c`  
		Last Modified: Thu, 26 Jan 2023 20:44:53 GMT  
		Size: 62.3 MB (62341068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9c62719ce9a736ff6f49a8d84be8316820a6035ab43ac69eaafb9ec7975bcd`  
		Last Modified: Thu, 26 Jan 2023 22:21:33 GMT  
		Size: 430.2 MB (430190538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:abcef3933194055013b7b02644b7ab3ca2ac28625e48190cfeda61595fffe67f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **494.2 MB (494155176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0726baa057a47e2e49ea7a98d3a8206bde79fd1225f738ccfc73ba0fd69eef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 26 Jan 2023 22:39:30 GMT
ADD file:1b056f516caefc99e89cee1ffa2d3b98a54ec5756d3c54b0b1c75c6ddfa9e1ae in / 
# Thu, 26 Jan 2023 22:39:31 GMT
CMD ["/bin/bash"]
# Thu, 26 Jan 2023 22:39:53 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-5f290fbb01ed6cae6ec9436094897096f0cd61aa0fb90afb412045f989363faa.tar.gz"     && echo "a2345704122103f0cf035d1ae3d4fa863db8c73c0f08e6f8656f5ac9274b0eba  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f211bebb41ee40fd8a6c26d9c71d47a936d9684219f14a2679e8f57c07bb49b6`  
		Last Modified: Thu, 26 Jan 2023 22:40:24 GMT  
		Size: 64.0 MB (63964642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9850613c66f695c4d0de595f9359ad654f83678bbe4f57664bf76827b8ca00`  
		Last Modified: Thu, 26 Jan 2023 22:40:47 GMT  
		Size: 430.2 MB (430190534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
