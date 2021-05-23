<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20210421.0`](#amazonlinux20202104210)
-	[`amazonlinux:2.0.20210421.0-with-sources`](#amazonlinux20202104210-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20210408.0`](#amazonlinux2018030202104080)
-	[`amazonlinux:2018.03.0.20210408.0-with-sources`](#amazonlinux2018030202104080-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:c8391ce46ca07254a66b160789c68a9eab6b2e8b87c2d2ddc45617ac0f9ef20e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:653ad088c4e1f87ae44b7890a50662f71ccbcec7c3619322bc944533dfcd50b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62226315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368ea5ea3a4b7d53740f298e460f693aa9cda125bda296f6c05e9fd6f3cb848e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:26:27 GMT
ADD file:2d979ed0e9e673272746c2e0a1470a4a1b1d64f4090c95fb32517a37e325d8b1 in / 
# Thu, 29 Apr 2021 22:26:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a9655ddf48b7834722b3efc02c2b73c54f8072f6e379a605978e073e0ac1e16b`  
		Last Modified: Thu, 29 Apr 2021 22:28:23 GMT  
		Size: 62.2 MB (62226315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:8b0f5eeddb4d174f329a1a019037bb61658dd42da2e5a42c52811d8cc5aad049
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0ba375490199e0f44c3adbdeab0649312e57b258ddece02bbd6412a85fa02003
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449089269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6909c494b13338778bf37a69d536375f823ff7634218e1eb3cba228133b328f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:26:27 GMT
ADD file:2d979ed0e9e673272746c2e0a1470a4a1b1d64f4090c95fb32517a37e325d8b1 in / 
# Thu, 29 Apr 2021 22:26:27 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:26:49 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-dc5d92c927a9f79aab7658e5c05df877dd40282d7bf9b4b11a5eb11b225cb7ad.tar.gz"  && echo "03509f1ca8f0593cf761a9fda3dc71baf0f45752a0d8908a04ccd9937bd1ddfc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a9655ddf48b7834722b3efc02c2b73c54f8072f6e379a605978e073e0ac1e16b`  
		Last Modified: Thu, 29 Apr 2021 22:28:23 GMT  
		Size: 62.2 MB (62226315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6639bc772b184db71b1862a37024f43f715383622456477065acea2796de80a4`  
		Last Modified: Thu, 29 Apr 2021 22:28:53 GMT  
		Size: 386.9 MB (386862954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:06b9e2433e4e563e1d75bc8c71d32b76dc49a2841e9253746eefc8ca40b80b5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:930034b169a5d135367a750be2bb7ecf2d6eff2283b74fc7125c22668fad9a92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61947132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53ef897d731f9a5673c083d0e86d7911f85d6e63bb2be2346b17bdbacdc58637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:25:37 GMT
ADD file:47fcf0318dccec16b61a0d21a0f16c45b77dea5abf50ba6604f1ffadcb299d10 in / 
# Thu, 29 Apr 2021 22:25:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3c2c91c7c4311eca863331479504040ee4f45fda9a610947b82886e7bbd5b737`  
		Last Modified: Thu, 29 Apr 2021 22:27:18 GMT  
		Size: 61.9 MB (61947132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:c966229ba3727252b912ba666632b193ac2494f66a943688b23268b3033d077b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63660068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c5a3eb2a399674b6dc35474facec5f1f4531b424579b4b3d09ccd5e86aec048`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:40:32 GMT
ADD file:03605b69274d89b78234df03d53dacc9cac408d68b82b1fb5d63b84c01b69300 in / 
# Thu, 29 Apr 2021 22:40:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:316be4ce82c0add9f71a6ce1face38b99f456abd45232cf7ad96ccac098ef5fe`  
		Last Modified: Thu, 29 Apr 2021 22:41:52 GMT  
		Size: 63.7 MB (63660068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:5c78eec45ee7b16ff81585a58919a3fce701fd95a21f17fc83d61301a5e0516f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:54a81a819385e5ba38b4586b3c960265d106ef7c3924e123dc6848a5b4c8c797
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542818467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4415525a0de6b386eda3d2e8e55c3530698cf3846bd4fda077e8e21743635d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:25:37 GMT
ADD file:47fcf0318dccec16b61a0d21a0f16c45b77dea5abf50ba6604f1ffadcb299d10 in / 
# Thu, 29 Apr 2021 22:25:38 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:26:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d13694054fd2292bc82935f30053f08860d9c7daaaa74d8f5f585dc5be3cc9df.tar.gz"  && echo "532d92b76391e5f08e90ddaac93c1dbf341a2a34550c32e357fdaae61a727917  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3c2c91c7c4311eca863331479504040ee4f45fda9a610947b82886e7bbd5b737`  
		Last Modified: Thu, 29 Apr 2021 22:27:18 GMT  
		Size: 61.9 MB (61947132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa16be21b849cedc18925697d377825ff62903ab864293be050e3af75e2de4`  
		Last Modified: Thu, 29 Apr 2021 22:28:00 GMT  
		Size: 480.9 MB (480871335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:bbad5f4379aaff82f42a053356c5a11a83e909d861070a6d8c22bdf66d2d9b8c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544531400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70b596f0f1df89a10bcd4962777589a56abe72ef2b90ae923f496a67be4eb38c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:40:32 GMT
ADD file:03605b69274d89b78234df03d53dacc9cac408d68b82b1fb5d63b84c01b69300 in / 
# Thu, 29 Apr 2021 22:40:37 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:41:16 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d13694054fd2292bc82935f30053f08860d9c7daaaa74d8f5f585dc5be3cc9df.tar.gz"  && echo "532d92b76391e5f08e90ddaac93c1dbf341a2a34550c32e357fdaae61a727917  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:316be4ce82c0add9f71a6ce1face38b99f456abd45232cf7ad96ccac098ef5fe`  
		Last Modified: Thu, 29 Apr 2021 22:41:52 GMT  
		Size: 63.7 MB (63660068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9964098dcf19d090cdfd0d0a54e9a64b5730888f14669664538953f67272a3e`  
		Last Modified: Thu, 29 Apr 2021 22:42:46 GMT  
		Size: 480.9 MB (480871332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210421.0`

```console
$ docker pull amazonlinux@sha256:06b9e2433e4e563e1d75bc8c71d32b76dc49a2841e9253746eefc8ca40b80b5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210421.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:930034b169a5d135367a750be2bb7ecf2d6eff2283b74fc7125c22668fad9a92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61947132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53ef897d731f9a5673c083d0e86d7911f85d6e63bb2be2346b17bdbacdc58637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:25:37 GMT
ADD file:47fcf0318dccec16b61a0d21a0f16c45b77dea5abf50ba6604f1ffadcb299d10 in / 
# Thu, 29 Apr 2021 22:25:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3c2c91c7c4311eca863331479504040ee4f45fda9a610947b82886e7bbd5b737`  
		Last Modified: Thu, 29 Apr 2021 22:27:18 GMT  
		Size: 61.9 MB (61947132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210421.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:c966229ba3727252b912ba666632b193ac2494f66a943688b23268b3033d077b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63660068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c5a3eb2a399674b6dc35474facec5f1f4531b424579b4b3d09ccd5e86aec048`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:40:32 GMT
ADD file:03605b69274d89b78234df03d53dacc9cac408d68b82b1fb5d63b84c01b69300 in / 
# Thu, 29 Apr 2021 22:40:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:316be4ce82c0add9f71a6ce1face38b99f456abd45232cf7ad96ccac098ef5fe`  
		Last Modified: Thu, 29 Apr 2021 22:41:52 GMT  
		Size: 63.7 MB (63660068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20210421.0-with-sources`

```console
$ docker pull amazonlinux@sha256:5c78eec45ee7b16ff81585a58919a3fce701fd95a21f17fc83d61301a5e0516f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20210421.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:54a81a819385e5ba38b4586b3c960265d106ef7c3924e123dc6848a5b4c8c797
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542818467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4415525a0de6b386eda3d2e8e55c3530698cf3846bd4fda077e8e21743635d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:25:37 GMT
ADD file:47fcf0318dccec16b61a0d21a0f16c45b77dea5abf50ba6604f1ffadcb299d10 in / 
# Thu, 29 Apr 2021 22:25:38 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:26:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d13694054fd2292bc82935f30053f08860d9c7daaaa74d8f5f585dc5be3cc9df.tar.gz"  && echo "532d92b76391e5f08e90ddaac93c1dbf341a2a34550c32e357fdaae61a727917  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3c2c91c7c4311eca863331479504040ee4f45fda9a610947b82886e7bbd5b737`  
		Last Modified: Thu, 29 Apr 2021 22:27:18 GMT  
		Size: 61.9 MB (61947132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa16be21b849cedc18925697d377825ff62903ab864293be050e3af75e2de4`  
		Last Modified: Thu, 29 Apr 2021 22:28:00 GMT  
		Size: 480.9 MB (480871335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20210421.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:bbad5f4379aaff82f42a053356c5a11a83e909d861070a6d8c22bdf66d2d9b8c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544531400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70b596f0f1df89a10bcd4962777589a56abe72ef2b90ae923f496a67be4eb38c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:40:32 GMT
ADD file:03605b69274d89b78234df03d53dacc9cac408d68b82b1fb5d63b84c01b69300 in / 
# Thu, 29 Apr 2021 22:40:37 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:41:16 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d13694054fd2292bc82935f30053f08860d9c7daaaa74d8f5f585dc5be3cc9df.tar.gz"  && echo "532d92b76391e5f08e90ddaac93c1dbf341a2a34550c32e357fdaae61a727917  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:316be4ce82c0add9f71a6ce1face38b99f456abd45232cf7ad96ccac098ef5fe`  
		Last Modified: Thu, 29 Apr 2021 22:41:52 GMT  
		Size: 63.7 MB (63660068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9964098dcf19d090cdfd0d0a54e9a64b5730888f14669664538953f67272a3e`  
		Last Modified: Thu, 29 Apr 2021 22:42:46 GMT  
		Size: 480.9 MB (480871332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:c8391ce46ca07254a66b160789c68a9eab6b2e8b87c2d2ddc45617ac0f9ef20e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:653ad088c4e1f87ae44b7890a50662f71ccbcec7c3619322bc944533dfcd50b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62226315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368ea5ea3a4b7d53740f298e460f693aa9cda125bda296f6c05e9fd6f3cb848e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:26:27 GMT
ADD file:2d979ed0e9e673272746c2e0a1470a4a1b1d64f4090c95fb32517a37e325d8b1 in / 
# Thu, 29 Apr 2021 22:26:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a9655ddf48b7834722b3efc02c2b73c54f8072f6e379a605978e073e0ac1e16b`  
		Last Modified: Thu, 29 Apr 2021 22:28:23 GMT  
		Size: 62.2 MB (62226315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:8b0f5eeddb4d174f329a1a019037bb61658dd42da2e5a42c52811d8cc5aad049
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0ba375490199e0f44c3adbdeab0649312e57b258ddece02bbd6412a85fa02003
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449089269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6909c494b13338778bf37a69d536375f823ff7634218e1eb3cba228133b328f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:26:27 GMT
ADD file:2d979ed0e9e673272746c2e0a1470a4a1b1d64f4090c95fb32517a37e325d8b1 in / 
# Thu, 29 Apr 2021 22:26:27 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:26:49 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-dc5d92c927a9f79aab7658e5c05df877dd40282d7bf9b4b11a5eb11b225cb7ad.tar.gz"  && echo "03509f1ca8f0593cf761a9fda3dc71baf0f45752a0d8908a04ccd9937bd1ddfc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a9655ddf48b7834722b3efc02c2b73c54f8072f6e379a605978e073e0ac1e16b`  
		Last Modified: Thu, 29 Apr 2021 22:28:23 GMT  
		Size: 62.2 MB (62226315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6639bc772b184db71b1862a37024f43f715383622456477065acea2796de80a4`  
		Last Modified: Thu, 29 Apr 2021 22:28:53 GMT  
		Size: 386.9 MB (386862954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210408.0`

```console
$ docker pull amazonlinux@sha256:c8391ce46ca07254a66b160789c68a9eab6b2e8b87c2d2ddc45617ac0f9ef20e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20210408.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:653ad088c4e1f87ae44b7890a50662f71ccbcec7c3619322bc944533dfcd50b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62226315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368ea5ea3a4b7d53740f298e460f693aa9cda125bda296f6c05e9fd6f3cb848e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:26:27 GMT
ADD file:2d979ed0e9e673272746c2e0a1470a4a1b1d64f4090c95fb32517a37e325d8b1 in / 
# Thu, 29 Apr 2021 22:26:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a9655ddf48b7834722b3efc02c2b73c54f8072f6e379a605978e073e0ac1e16b`  
		Last Modified: Thu, 29 Apr 2021 22:28:23 GMT  
		Size: 62.2 MB (62226315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20210408.0-with-sources`

```console
$ docker pull amazonlinux@sha256:8b0f5eeddb4d174f329a1a019037bb61658dd42da2e5a42c52811d8cc5aad049
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20210408.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0ba375490199e0f44c3adbdeab0649312e57b258ddece02bbd6412a85fa02003
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.1 MB (449089269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6909c494b13338778bf37a69d536375f823ff7634218e1eb3cba228133b328f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:26:27 GMT
ADD file:2d979ed0e9e673272746c2e0a1470a4a1b1d64f4090c95fb32517a37e325d8b1 in / 
# Thu, 29 Apr 2021 22:26:27 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:26:49 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-dc5d92c927a9f79aab7658e5c05df877dd40282d7bf9b4b11a5eb11b225cb7ad.tar.gz"  && echo "03509f1ca8f0593cf761a9fda3dc71baf0f45752a0d8908a04ccd9937bd1ddfc  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a9655ddf48b7834722b3efc02c2b73c54f8072f6e379a605978e073e0ac1e16b`  
		Last Modified: Thu, 29 Apr 2021 22:28:23 GMT  
		Size: 62.2 MB (62226315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6639bc772b184db71b1862a37024f43f715383622456477065acea2796de80a4`  
		Last Modified: Thu, 29 Apr 2021 22:28:53 GMT  
		Size: 386.9 MB (386862954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:06b9e2433e4e563e1d75bc8c71d32b76dc49a2841e9253746eefc8ca40b80b5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:930034b169a5d135367a750be2bb7ecf2d6eff2283b74fc7125c22668fad9a92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.9 MB (61947132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53ef897d731f9a5673c083d0e86d7911f85d6e63bb2be2346b17bdbacdc58637`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:25:37 GMT
ADD file:47fcf0318dccec16b61a0d21a0f16c45b77dea5abf50ba6604f1ffadcb299d10 in / 
# Thu, 29 Apr 2021 22:25:38 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:3c2c91c7c4311eca863331479504040ee4f45fda9a610947b82886e7bbd5b737`  
		Last Modified: Thu, 29 Apr 2021 22:27:18 GMT  
		Size: 61.9 MB (61947132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:c966229ba3727252b912ba666632b193ac2494f66a943688b23268b3033d077b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63660068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c5a3eb2a399674b6dc35474facec5f1f4531b424579b4b3d09ccd5e86aec048`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:40:32 GMT
ADD file:03605b69274d89b78234df03d53dacc9cac408d68b82b1fb5d63b84c01b69300 in / 
# Thu, 29 Apr 2021 22:40:37 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:316be4ce82c0add9f71a6ce1face38b99f456abd45232cf7ad96ccac098ef5fe`  
		Last Modified: Thu, 29 Apr 2021 22:41:52 GMT  
		Size: 63.7 MB (63660068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:5c78eec45ee7b16ff81585a58919a3fce701fd95a21f17fc83d61301a5e0516f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:54a81a819385e5ba38b4586b3c960265d106ef7c3924e123dc6848a5b4c8c797
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542818467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4415525a0de6b386eda3d2e8e55c3530698cf3846bd4fda077e8e21743635d2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:25:37 GMT
ADD file:47fcf0318dccec16b61a0d21a0f16c45b77dea5abf50ba6604f1ffadcb299d10 in / 
# Thu, 29 Apr 2021 22:25:38 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:26:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d13694054fd2292bc82935f30053f08860d9c7daaaa74d8f5f585dc5be3cc9df.tar.gz"  && echo "532d92b76391e5f08e90ddaac93c1dbf341a2a34550c32e357fdaae61a727917  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:3c2c91c7c4311eca863331479504040ee4f45fda9a610947b82886e7bbd5b737`  
		Last Modified: Thu, 29 Apr 2021 22:27:18 GMT  
		Size: 61.9 MB (61947132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59aa16be21b849cedc18925697d377825ff62903ab864293be050e3af75e2de4`  
		Last Modified: Thu, 29 Apr 2021 22:28:00 GMT  
		Size: 480.9 MB (480871335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:bbad5f4379aaff82f42a053356c5a11a83e909d861070a6d8c22bdf66d2d9b8c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.5 MB (544531400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70b596f0f1df89a10bcd4962777589a56abe72ef2b90ae923f496a67be4eb38c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:40:32 GMT
ADD file:03605b69274d89b78234df03d53dacc9cac408d68b82b1fb5d63b84c01b69300 in / 
# Thu, 29 Apr 2021 22:40:37 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:41:16 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-d13694054fd2292bc82935f30053f08860d9c7daaaa74d8f5f585dc5be3cc9df.tar.gz"  && echo "532d92b76391e5f08e90ddaac93c1dbf341a2a34550c32e357fdaae61a727917  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:316be4ce82c0add9f71a6ce1face38b99f456abd45232cf7ad96ccac098ef5fe`  
		Last Modified: Thu, 29 Apr 2021 22:41:52 GMT  
		Size: 63.7 MB (63660068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9964098dcf19d090cdfd0d0a54e9a64b5730888f14669664538953f67272a3e`  
		Last Modified: Thu, 29 Apr 2021 22:42:46 GMT  
		Size: 480.9 MB (480871332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
