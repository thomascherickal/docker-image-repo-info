<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03.0.20201209.1`](#amazonlinux2018030202012091)
-	[`amazonlinux:2018.03.0.20201209.1-with-sources`](#amazonlinux2018030202012091-with-sources)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2.0.20201218.1`](#amazonlinux20202012181)
-	[`amazonlinux:2.0.20201218.1-with-sources`](#amazonlinux20202012181-with-sources)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:99cd0e8755feee09c253bc0ffa9a2785cdd5c2de929859fd424944883a3777d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c575dbda82e056425a0bd1e3bed0f592bc5cd309e41ab69d1e37b8b7ed1e78ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62391497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a6f913fa957e59bf5aab7754b83474a8d0c8e42985d6352151a21ce0c360b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:50 GMT
ADD file:fad21d2914f8429ddebb886e5d03ca48b4cb36eccac1e691bb6ed0f9cb7a6f03 in / 
# Wed, 23 Dec 2020 20:20:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0d94e7de59b4b27051eda77847a3e1fc846797f408beefa97271f541420516c3`  
		Last Modified: Wed, 23 Dec 2020 20:22:43 GMT  
		Size: 62.4 MB (62391497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:728fe610c29c4b3d89fbd2447cbacf5e0861e813474b903bce48d54a0b95d9b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ff807c30a818c92b6c322b8f8a9cda7642253c632f7f7deb3e28968fea38bd7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.3 MB (449256394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38785f24e771e397d1d05b265eb5cb9eb1cb94e223d4aeb075b78df1d94e38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:50 GMT
ADD file:fad21d2914f8429ddebb886e5d03ca48b4cb36eccac1e691bb6ed0f9cb7a6f03 in / 
# Wed, 23 Dec 2020 20:20:50 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 20:21:13 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-8332ab379854aecfcd3ddf9c79744dfabb59c3b3aace63aaa61c9a99d8632bf1.tar.gz"  && echo "02b8c67f01479983152192070a10d4b669597d506849684e48c32d9b4b66ffde  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0d94e7de59b4b27051eda77847a3e1fc846797f408beefa97271f541420516c3`  
		Last Modified: Wed, 23 Dec 2020 20:22:43 GMT  
		Size: 62.4 MB (62391497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92833f5796ed72fcb599787b27e5758e69fb5fba474a57eff8f180868e6ac4f`  
		Last Modified: Wed, 23 Dec 2020 20:23:07 GMT  
		Size: 386.9 MB (386864897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:420a6503505c73ea05e1254acd4d1a5e73305dab8ec3fa70833e112cc6980624
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:1c5213077930ebbd35b51bece063ffb31f47df9c6fb71b7248944785c77ba772
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62007428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9917dfe117ca1e8affbea6d819c0d94918524ae1882fe69746a8217aec4c4053`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:d4e6ef65af9890813147ffac08f349a0d0c1edbe840d3fd0430723f63f73a78c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63707914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e29a7714b76a8ac87a5634269fb63b50c709bc940cc096d773d565d67218c29`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:99cd0e8755feee09c253bc0ffa9a2785cdd5c2de929859fd424944883a3777d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c575dbda82e056425a0bd1e3bed0f592bc5cd309e41ab69d1e37b8b7ed1e78ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62391497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a6f913fa957e59bf5aab7754b83474a8d0c8e42985d6352151a21ce0c360b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:50 GMT
ADD file:fad21d2914f8429ddebb886e5d03ca48b4cb36eccac1e691bb6ed0f9cb7a6f03 in / 
# Wed, 23 Dec 2020 20:20:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0d94e7de59b4b27051eda77847a3e1fc846797f408beefa97271f541420516c3`  
		Last Modified: Wed, 23 Dec 2020 20:22:43 GMT  
		Size: 62.4 MB (62391497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20201209.1`

```console
$ docker pull amazonlinux@sha256:99cd0e8755feee09c253bc0ffa9a2785cdd5c2de929859fd424944883a3777d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20201209.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c575dbda82e056425a0bd1e3bed0f592bc5cd309e41ab69d1e37b8b7ed1e78ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62391497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3a6f913fa957e59bf5aab7754b83474a8d0c8e42985d6352151a21ce0c360b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:50 GMT
ADD file:fad21d2914f8429ddebb886e5d03ca48b4cb36eccac1e691bb6ed0f9cb7a6f03 in / 
# Wed, 23 Dec 2020 20:20:50 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0d94e7de59b4b27051eda77847a3e1fc846797f408beefa97271f541420516c3`  
		Last Modified: Wed, 23 Dec 2020 20:22:43 GMT  
		Size: 62.4 MB (62391497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20201209.1-with-sources`

```console
$ docker pull amazonlinux@sha256:728fe610c29c4b3d89fbd2447cbacf5e0861e813474b903bce48d54a0b95d9b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20201209.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ff807c30a818c92b6c322b8f8a9cda7642253c632f7f7deb3e28968fea38bd7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.3 MB (449256394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38785f24e771e397d1d05b265eb5cb9eb1cb94e223d4aeb075b78df1d94e38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:50 GMT
ADD file:fad21d2914f8429ddebb886e5d03ca48b4cb36eccac1e691bb6ed0f9cb7a6f03 in / 
# Wed, 23 Dec 2020 20:20:50 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 20:21:13 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-8332ab379854aecfcd3ddf9c79744dfabb59c3b3aace63aaa61c9a99d8632bf1.tar.gz"  && echo "02b8c67f01479983152192070a10d4b669597d506849684e48c32d9b4b66ffde  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0d94e7de59b4b27051eda77847a3e1fc846797f408beefa97271f541420516c3`  
		Last Modified: Wed, 23 Dec 2020 20:22:43 GMT  
		Size: 62.4 MB (62391497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92833f5796ed72fcb599787b27e5758e69fb5fba474a57eff8f180868e6ac4f`  
		Last Modified: Wed, 23 Dec 2020 20:23:07 GMT  
		Size: 386.9 MB (386864897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:728fe610c29c4b3d89fbd2447cbacf5e0861e813474b903bce48d54a0b95d9b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ff807c30a818c92b6c322b8f8a9cda7642253c632f7f7deb3e28968fea38bd7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.3 MB (449256394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a38785f24e771e397d1d05b265eb5cb9eb1cb94e223d4aeb075b78df1d94e38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:50 GMT
ADD file:fad21d2914f8429ddebb886e5d03ca48b4cb36eccac1e691bb6ed0f9cb7a6f03 in / 
# Wed, 23 Dec 2020 20:20:50 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 20:21:13 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-8332ab379854aecfcd3ddf9c79744dfabb59c3b3aace63aaa61c9a99d8632bf1.tar.gz"  && echo "02b8c67f01479983152192070a10d4b669597d506849684e48c32d9b4b66ffde  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0d94e7de59b4b27051eda77847a3e1fc846797f408beefa97271f541420516c3`  
		Last Modified: Wed, 23 Dec 2020 20:22:43 GMT  
		Size: 62.4 MB (62391497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92833f5796ed72fcb599787b27e5758e69fb5fba474a57eff8f180868e6ac4f`  
		Last Modified: Wed, 23 Dec 2020 20:23:07 GMT  
		Size: 386.9 MB (386864897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20201218.1`

```console
$ docker pull amazonlinux@sha256:420a6503505c73ea05e1254acd4d1a5e73305dab8ec3fa70833e112cc6980624
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20201218.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:1c5213077930ebbd35b51bece063ffb31f47df9c6fb71b7248944785c77ba772
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62007428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9917dfe117ca1e8affbea6d819c0d94918524ae1882fe69746a8217aec4c4053`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20201218.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:d4e6ef65af9890813147ffac08f349a0d0c1edbe840d3fd0430723f63f73a78c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63707914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e29a7714b76a8ac87a5634269fb63b50c709bc940cc096d773d565d67218c29`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20201218.1-with-sources`

```console
$ docker pull amazonlinux@sha256:60eaad1a680f611c9cf9fd4f2a1ddad0c299a28a7688ca2875c2631036b1ff7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20201218.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ec8b116cbc8e5f39d32cc46ab9d1823d413862a07e85ddb4dc3b9ac054bb98c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542851989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba507121a17fcae383da7f3fc6481ee5707835c3e67b7fd68edc64698d31b44b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 20:20:34 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-826e231a97252a5034e63006e69224de2364211252782ce0d9eab6a50c799006.tar.gz"  && echo "3d237536b5aa360bd744e30abd284cdd42eb182e390f3d4c2abc4655f7a048a2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3130bba24cdc0c903b6d6eb23f3cb5fcc362f36af331045a285d5ccb0c74bc45`  
		Last Modified: Wed, 23 Dec 2020 20:22:24 GMT  
		Size: 480.8 MB (480844561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20201218.1-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9c7588150eff1d7928416c7fafd35edaa4f1d03d663f0c7fdac8ac62de67c8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.6 MB (544552541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d28578129bba32d0a61dcb4c5ce73ca3365c60abcae712f3c4d2edd3009ae7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 19:40:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-826e231a97252a5034e63006e69224de2364211252782ce0d9eab6a50c799006.tar.gz"  && echo "3d237536b5aa360bd744e30abd284cdd42eb182e390f3d4c2abc4655f7a048a2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3431b17c8d2c281dfa9b3b9f9880a6159a978452bed73137b8af89f04586250c`  
		Last Modified: Wed, 23 Dec 2020 19:41:41 GMT  
		Size: 480.8 MB (480844627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:60eaad1a680f611c9cf9fd4f2a1ddad0c299a28a7688ca2875c2631036b1ff7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ec8b116cbc8e5f39d32cc46ab9d1823d413862a07e85ddb4dc3b9ac054bb98c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542851989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba507121a17fcae383da7f3fc6481ee5707835c3e67b7fd68edc64698d31b44b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 20:20:34 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-826e231a97252a5034e63006e69224de2364211252782ce0d9eab6a50c799006.tar.gz"  && echo "3d237536b5aa360bd744e30abd284cdd42eb182e390f3d4c2abc4655f7a048a2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3130bba24cdc0c903b6d6eb23f3cb5fcc362f36af331045a285d5ccb0c74bc45`  
		Last Modified: Wed, 23 Dec 2020 20:22:24 GMT  
		Size: 480.8 MB (480844561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9c7588150eff1d7928416c7fafd35edaa4f1d03d663f0c7fdac8ac62de67c8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.6 MB (544552541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d28578129bba32d0a61dcb4c5ce73ca3365c60abcae712f3c4d2edd3009ae7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 19:40:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-826e231a97252a5034e63006e69224de2364211252782ce0d9eab6a50c799006.tar.gz"  && echo "3d237536b5aa360bd744e30abd284cdd42eb182e390f3d4c2abc4655f7a048a2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3431b17c8d2c281dfa9b3b9f9880a6159a978452bed73137b8af89f04586250c`  
		Last Modified: Wed, 23 Dec 2020 19:41:41 GMT  
		Size: 480.8 MB (480844627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:420a6503505c73ea05e1254acd4d1a5e73305dab8ec3fa70833e112cc6980624
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:1c5213077930ebbd35b51bece063ffb31f47df9c6fb71b7248944785c77ba772
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62007428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9917dfe117ca1e8affbea6d819c0d94918524ae1882fe69746a8217aec4c4053`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:d4e6ef65af9890813147ffac08f349a0d0c1edbe840d3fd0430723f63f73a78c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63707914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e29a7714b76a8ac87a5634269fb63b50c709bc940cc096d773d565d67218c29`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:60eaad1a680f611c9cf9fd4f2a1ddad0c299a28a7688ca2875c2631036b1ff7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ec8b116cbc8e5f39d32cc46ab9d1823d413862a07e85ddb4dc3b9ac054bb98c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.9 MB (542851989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba507121a17fcae383da7f3fc6481ee5707835c3e67b7fd68edc64698d31b44b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 20:20:09 GMT
ADD file:15991ffbefc01e13f134972ce0eabc6b7901ea9ab4d56347bee5057302cf4848 in / 
# Wed, 23 Dec 2020 20:20:09 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 20:20:34 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-826e231a97252a5034e63006e69224de2364211252782ce0d9eab6a50c799006.tar.gz"  && echo "3d237536b5aa360bd744e30abd284cdd42eb182e390f3d4c2abc4655f7a048a2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:4232b9ee675bb1f9a32337ec3f266a570b75c54c3c3f173b1abb998e9984ad8c`  
		Last Modified: Wed, 23 Dec 2020 20:21:42 GMT  
		Size: 62.0 MB (62007428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3130bba24cdc0c903b6d6eb23f3cb5fcc362f36af331045a285d5ccb0c74bc45`  
		Last Modified: Wed, 23 Dec 2020 20:22:24 GMT  
		Size: 480.8 MB (480844561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:9c7588150eff1d7928416c7fafd35edaa4f1d03d663f0c7fdac8ac62de67c8a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.6 MB (544552541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d28578129bba32d0a61dcb4c5ce73ca3365c60abcae712f3c4d2edd3009ae7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 23 Dec 2020 19:39:59 GMT
ADD file:d991483ad4376be5e4327b3789511ab9266db8b87fc4b5327f0cabd1016ba00a in / 
# Wed, 23 Dec 2020 19:40:02 GMT
CMD ["/bin/bash"]
# Wed, 23 Dec 2020 19:40:28 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-826e231a97252a5034e63006e69224de2364211252782ce0d9eab6a50c799006.tar.gz"  && echo "3d237536b5aa360bd744e30abd284cdd42eb182e390f3d4c2abc4655f7a048a2  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3307d2ab2034125075f0b058dcc32d6bf3e2c0595f1306de08d9e4a0287ddd76`  
		Last Modified: Wed, 23 Dec 2020 19:40:59 GMT  
		Size: 63.7 MB (63707914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3431b17c8d2c281dfa9b3b9f9880a6159a978452bed73137b8af89f04586250c`  
		Last Modified: Wed, 23 Dec 2020 19:41:41 GMT  
		Size: 480.8 MB (480844627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
