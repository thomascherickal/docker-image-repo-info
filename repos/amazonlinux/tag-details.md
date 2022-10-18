<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:2.0.20220912.1`](#amazonlinux20202209121)
-	[`amazonlinux:2.0.20220912.1-with-sources`](#amazonlinux20202209121-with-sources)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2018.03.0.20220907.3`](#amazonlinux2018030202209073)
-	[`amazonlinux:2018.03.0.20220907.3-with-sources`](#amazonlinux2018030202209073-with-sources)
-	[`amazonlinux:2022`](#amazonlinux2022)
-	[`amazonlinux:2022-with-sources`](#amazonlinux2022-with-sources)
-	[`amazonlinux:2022.0.20221012.0`](#amazonlinux20220202210120)
-	[`amazonlinux:2022.0.20221012.0-with-sources`](#amazonlinux20220202210120-with-sources)
-	[`amazonlinux:devel`](#amazonlinuxdevel)
-	[`amazonlinux:devel-with-sources`](#amazonlinuxdevel-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:cc88d1da2efe66faa3b86ef71e70e8b7b52822f1bebdd1dd7b56c7f0e3cbc978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ba0ec71b51f66eeb3c2a808f463fa79dffa362de472e3e6c1650b0953471b227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62346886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80a9b43a329751b9a765fb6d1e788afb43419119cb4946c578832fb43fb8a84`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:4cc664bb668e2e073fb39df0fee7e85317f34850ac7b117fb832a1a3c7b47e06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e904f4b8c4ac1bd2ee165c00d8c0854558b9a799a31c0a265433f1ed453c2970
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515034753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232eb238b33b7e870dd055314fe8ca6e936ad5f353e199a4f203ec82ca7fe5de`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
# Thu, 25 Aug 2022 18:20:10 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-77f3d99b447b0774a1bbba85498486869e097db4118c05994ac137d64f0f07bb.tar.gz"     && echo "c428ed82c12be347f1150a419dc16d997020583bda0f076e10a0f34b88df6363  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb07ac98d11436de390efdab7fd63c37b7afabc8b88176ca190a39ba9a6cb12`  
		Last Modified: Thu, 25 Aug 2022 18:21:18 GMT  
		Size: 452.7 MB (452687867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:b393108d01e77ff923d602f837fabb1aa545e8b913fbb1f7130d2ca30bde3c54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c5e654f04302f2f88bdc5fe9644b7a096405205432a3738fc2ca6d4b766b6037
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62303269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01bdb519be2070a170aee5940166344f2a871e7d22887366c0a30406094727bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:19:21 GMT
ADD file:99847692b0f2dee43b50f306ad92fbc13ccb0541af21c6d3040f72d3184aabac in / 
# Thu, 22 Sep 2022 19:19:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e80285ff599e329e689e4689be05885456823b7f6233486aa419541ae8e98c62`  
		Last Modified: Wed, 21 Sep 2022 22:07:12 GMT  
		Size: 62.3 MB (62303269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:10c927b25ed56533d46fc4f2ac0085bc5f8839527c83ee5ea395753b019d899f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63912418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c44e7db5ae05cce1a4890c4507b657d00a595765e478417de6cbe69d4d4eb01`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:39:26 GMT
ADD file:cd0852de8cdfb2b7efdaa53ad4827a33302d895b10306b540e7df9d8c7f00637 in / 
# Thu, 22 Sep 2022 19:39:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f5371f42f94d8ba2c9559448b8e36de82d246f179760ec911f594632d3545611`  
		Last Modified: Wed, 21 Sep 2022 22:07:11 GMT  
		Size: 63.9 MB (63912418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:a4a7095f6cae0281cf3a5f357eda5174a0e2ee3fb1f584858f2740c0958a7eae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:f1c531eaf600c693158c1d1ebbead9146809d78fab280d8bb9fa3b255b8c5af0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486378202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1900d5d0b057d3ad0be96c67ba2666b4016b5a9e87c34e4442e61d12d4002336`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:19:21 GMT
ADD file:99847692b0f2dee43b50f306ad92fbc13ccb0541af21c6d3040f72d3184aabac in / 
# Thu, 22 Sep 2022 19:19:21 GMT
CMD ["/bin/bash"]
# Thu, 22 Sep 2022 19:19:40 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e805f912bcb0541240fd70fe7e7f23e3b79a2c5ce3c273054b3efc087e0cc6a1.tar.gz"     && echo "726894e6d2bbc0a7301d9a191b1197b554ad07319a01e726c537d27e73953785  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e80285ff599e329e689e4689be05885456823b7f6233486aa419541ae8e98c62`  
		Last Modified: Wed, 21 Sep 2022 22:07:12 GMT  
		Size: 62.3 MB (62303269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d7c2b2aa50fe3ff7023a3909084d659b7f234ce37cb2b8a54bc449bb682a27`  
		Last Modified: Thu, 22 Sep 2022 19:20:48 GMT  
		Size: 424.1 MB (424074933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:c64709a723326277e8bd139dee26c099248a5cfdc15af39276fdab5bfab370e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487987310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e561a7921606d2497a6dd0c931d14e2c4efc3c741a9a665cef47c145e63222`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:39:26 GMT
ADD file:cd0852de8cdfb2b7efdaa53ad4827a33302d895b10306b540e7df9d8c7f00637 in / 
# Thu, 22 Sep 2022 19:39:27 GMT
CMD ["/bin/bash"]
# Thu, 22 Sep 2022 19:39:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e805f912bcb0541240fd70fe7e7f23e3b79a2c5ce3c273054b3efc087e0cc6a1.tar.gz"     && echo "726894e6d2bbc0a7301d9a191b1197b554ad07319a01e726c537d27e73953785  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f5371f42f94d8ba2c9559448b8e36de82d246f179760ec911f594632d3545611`  
		Last Modified: Wed, 21 Sep 2022 22:07:11 GMT  
		Size: 63.9 MB (63912418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366907dea1a523b535578b50385542ee460f0d786719b57a5b8a57f84d86c59c`  
		Last Modified: Thu, 22 Sep 2022 19:41:14 GMT  
		Size: 424.1 MB (424074892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220912.1`

```console
$ docker pull amazonlinux@sha256:b393108d01e77ff923d602f837fabb1aa545e8b913fbb1f7130d2ca30bde3c54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220912.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c5e654f04302f2f88bdc5fe9644b7a096405205432a3738fc2ca6d4b766b6037
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62303269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01bdb519be2070a170aee5940166344f2a871e7d22887366c0a30406094727bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:19:21 GMT
ADD file:99847692b0f2dee43b50f306ad92fbc13ccb0541af21c6d3040f72d3184aabac in / 
# Thu, 22 Sep 2022 19:19:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e80285ff599e329e689e4689be05885456823b7f6233486aa419541ae8e98c62`  
		Last Modified: Wed, 21 Sep 2022 22:07:12 GMT  
		Size: 62.3 MB (62303269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220912.1` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:10c927b25ed56533d46fc4f2ac0085bc5f8839527c83ee5ea395753b019d899f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63912418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c44e7db5ae05cce1a4890c4507b657d00a595765e478417de6cbe69d4d4eb01`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:39:26 GMT
ADD file:cd0852de8cdfb2b7efdaa53ad4827a33302d895b10306b540e7df9d8c7f00637 in / 
# Thu, 22 Sep 2022 19:39:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f5371f42f94d8ba2c9559448b8e36de82d246f179760ec911f594632d3545611`  
		Last Modified: Wed, 21 Sep 2022 22:07:11 GMT  
		Size: 63.9 MB (63912418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20220912.1-with-sources`

```console
$ docker pull amazonlinux@sha256:a4a7095f6cae0281cf3a5f357eda5174a0e2ee3fb1f584858f2740c0958a7eae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20220912.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:f1c531eaf600c693158c1d1ebbead9146809d78fab280d8bb9fa3b255b8c5af0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486378202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1900d5d0b057d3ad0be96c67ba2666b4016b5a9e87c34e4442e61d12d4002336`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:19:21 GMT
ADD file:99847692b0f2dee43b50f306ad92fbc13ccb0541af21c6d3040f72d3184aabac in / 
# Thu, 22 Sep 2022 19:19:21 GMT
CMD ["/bin/bash"]
# Thu, 22 Sep 2022 19:19:40 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e805f912bcb0541240fd70fe7e7f23e3b79a2c5ce3c273054b3efc087e0cc6a1.tar.gz"     && echo "726894e6d2bbc0a7301d9a191b1197b554ad07319a01e726c537d27e73953785  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e80285ff599e329e689e4689be05885456823b7f6233486aa419541ae8e98c62`  
		Last Modified: Wed, 21 Sep 2022 22:07:12 GMT  
		Size: 62.3 MB (62303269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d7c2b2aa50fe3ff7023a3909084d659b7f234ce37cb2b8a54bc449bb682a27`  
		Last Modified: Thu, 22 Sep 2022 19:20:48 GMT  
		Size: 424.1 MB (424074933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20220912.1-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:c64709a723326277e8bd139dee26c099248a5cfdc15af39276fdab5bfab370e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487987310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e561a7921606d2497a6dd0c931d14e2c4efc3c741a9a665cef47c145e63222`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:39:26 GMT
ADD file:cd0852de8cdfb2b7efdaa53ad4827a33302d895b10306b540e7df9d8c7f00637 in / 
# Thu, 22 Sep 2022 19:39:27 GMT
CMD ["/bin/bash"]
# Thu, 22 Sep 2022 19:39:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e805f912bcb0541240fd70fe7e7f23e3b79a2c5ce3c273054b3efc087e0cc6a1.tar.gz"     && echo "726894e6d2bbc0a7301d9a191b1197b554ad07319a01e726c537d27e73953785  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f5371f42f94d8ba2c9559448b8e36de82d246f179760ec911f594632d3545611`  
		Last Modified: Wed, 21 Sep 2022 22:07:11 GMT  
		Size: 63.9 MB (63912418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366907dea1a523b535578b50385542ee460f0d786719b57a5b8a57f84d86c59c`  
		Last Modified: Thu, 22 Sep 2022 19:41:14 GMT  
		Size: 424.1 MB (424074892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:cc88d1da2efe66faa3b86ef71e70e8b7b52822f1bebdd1dd7b56c7f0e3cbc978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ba0ec71b51f66eeb3c2a808f463fa79dffa362de472e3e6c1650b0953471b227
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62346886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80a9b43a329751b9a765fb6d1e788afb43419119cb4946c578832fb43fb8a84`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:4cc664bb668e2e073fb39df0fee7e85317f34850ac7b117fb832a1a3c7b47e06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:e904f4b8c4ac1bd2ee165c00d8c0854558b9a799a31c0a265433f1ed453c2970
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.0 MB (515034753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232eb238b33b7e870dd055314fe8ca6e936ad5f353e199a4f203ec82ca7fe5de`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 25 Aug 2022 18:19:48 GMT
ADD file:9e8cce1e42cea635edfdd37709f35ae6c2245a7083686c2943b7d13dea774f7d in / 
# Thu, 25 Aug 2022 18:19:49 GMT
CMD ["/bin/bash"]
# Thu, 25 Aug 2022 18:20:10 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-77f3d99b447b0774a1bbba85498486869e097db4118c05994ac137d64f0f07bb.tar.gz"     && echo "c428ed82c12be347f1150a419dc16d997020583bda0f076e10a0f34b88df6363  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f08ecab7f1156b852159d72973eed2aacf858af0dbc76980151a20d8a80c0d30`  
		Last Modified: Thu, 25 Aug 2022 18:20:49 GMT  
		Size: 62.3 MB (62346886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb07ac98d11436de390efdab7fd63c37b7afabc8b88176ca190a39ba9a6cb12`  
		Last Modified: Thu, 25 Aug 2022 18:21:18 GMT  
		Size: 452.7 MB (452687867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20220907.3`

**does not exist** (yet?)

## `amazonlinux:2018.03.0.20220907.3-with-sources`

**does not exist** (yet?)

## `amazonlinux:2022`

```console
$ docker pull amazonlinux@sha256:9a8f402248e675582fc7a85b5571cfe930c4304350cebca34d4d7f4447f99319
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9be478e5302e819b22748b02cef9100fbe1d94fb2f686992bb1fe342e2f13617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57657755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff592f394353087fc68ed2ca76c2e93ef0530352e529cf4e24408fd19e50e0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f27d0cadf3b206e09b18623f6818f0956d878ab29fa00028c565e9f83b028eeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56481754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866f138fb6f3eef9cf1c6f7e3f9a6e139ed594eb1128b1599b0137b6d6e7ff5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022-with-sources`

```console
$ docker pull amazonlinux@sha256:215c755f3dd70ebd198d5750e92052deb39debf83d3d365e95633bb01f1d9957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0595983489ba3b0fff0f7099f2b64174d8792d7863dc1a5a8eadaf779bc48e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.7 MB (386739246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5dbe9498109f5c7575eef6c4776278d4c5ea3c83f9ed55211873a5c38c1410`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:20:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f62047bb148ea45f7f34dc9e1bffbd74fa083fd7b6784e0dbed1685f6eb339`  
		Last Modified: Tue, 18 Oct 2022 00:21:06 GMT  
		Size: 329.1 MB (329081491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6b5dade9f05691b289fbbcd0e203d6e44ac7bc4c9a7bd8049e26e13e0a7b57c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.6 MB (385563209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77e861f60a2da3e2c3af5d4dcb8cd19a11a1862fa9b80ddccb0c168e8e3ec9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:40:04 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f3324e83ad5f6d382027fcf8d3c3b31785ddb076e0ccee7669e38742e29ce2`  
		Last Modified: Tue, 18 Oct 2022 00:41:16 GMT  
		Size: 329.1 MB (329081455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20221012.0`

```console
$ docker pull amazonlinux@sha256:9a8f402248e675582fc7a85b5571cfe930c4304350cebca34d4d7f4447f99319
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20221012.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9be478e5302e819b22748b02cef9100fbe1d94fb2f686992bb1fe342e2f13617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57657755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff592f394353087fc68ed2ca76c2e93ef0530352e529cf4e24408fd19e50e0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20221012.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f27d0cadf3b206e09b18623f6818f0956d878ab29fa00028c565e9f83b028eeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56481754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866f138fb6f3eef9cf1c6f7e3f9a6e139ed594eb1128b1599b0137b6d6e7ff5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2022.0.20221012.0-with-sources`

```console
$ docker pull amazonlinux@sha256:215c755f3dd70ebd198d5750e92052deb39debf83d3d365e95633bb01f1d9957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2022.0.20221012.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0595983489ba3b0fff0f7099f2b64174d8792d7863dc1a5a8eadaf779bc48e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.7 MB (386739246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5dbe9498109f5c7575eef6c4776278d4c5ea3c83f9ed55211873a5c38c1410`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:20:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f62047bb148ea45f7f34dc9e1bffbd74fa083fd7b6784e0dbed1685f6eb339`  
		Last Modified: Tue, 18 Oct 2022 00:21:06 GMT  
		Size: 329.1 MB (329081491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2022.0.20221012.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6b5dade9f05691b289fbbcd0e203d6e44ac7bc4c9a7bd8049e26e13e0a7b57c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.6 MB (385563209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77e861f60a2da3e2c3af5d4dcb8cd19a11a1862fa9b80ddccb0c168e8e3ec9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:40:04 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f3324e83ad5f6d382027fcf8d3c3b31785ddb076e0ccee7669e38742e29ce2`  
		Last Modified: Tue, 18 Oct 2022 00:41:16 GMT  
		Size: 329.1 MB (329081455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel`

```console
$ docker pull amazonlinux@sha256:9a8f402248e675582fc7a85b5571cfe930c4304350cebca34d4d7f4447f99319
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel` - linux; amd64

```console
$ docker pull amazonlinux@sha256:9be478e5302e819b22748b02cef9100fbe1d94fb2f686992bb1fe342e2f13617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57657755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff592f394353087fc68ed2ca76c2e93ef0530352e529cf4e24408fd19e50e0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:f27d0cadf3b206e09b18623f6818f0956d878ab29fa00028c565e9f83b028eeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56481754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866f138fb6f3eef9cf1c6f7e3f9a6e139ed594eb1128b1599b0137b6d6e7ff5d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:devel-with-sources`

```console
$ docker pull amazonlinux@sha256:215c755f3dd70ebd198d5750e92052deb39debf83d3d365e95633bb01f1d9957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:devel-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:0595983489ba3b0fff0f7099f2b64174d8792d7863dc1a5a8eadaf779bc48e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.7 MB (386739246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef5dbe9498109f5c7575eef6c4776278d4c5ea3c83f9ed55211873a5c38c1410`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:19:39 GMT
ADD file:8860392494bed2aec97f656f86966610382a6b489c2ad5c38026fe1d8d863f61 in / 
# Tue, 18 Oct 2022 00:19:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:20:00 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ec0bebc99e942c435ad72a66150b1af95996b96a131aa75a0d963df9e53487b3`  
		Last Modified: Sat, 15 Oct 2022 04:05:55 GMT  
		Size: 57.7 MB (57657755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f62047bb148ea45f7f34dc9e1bffbd74fa083fd7b6784e0dbed1685f6eb339`  
		Last Modified: Tue, 18 Oct 2022 00:21:06 GMT  
		Size: 329.1 MB (329081491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:devel-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:6b5dade9f05691b289fbbcd0e203d6e44ac7bc4c9a7bd8049e26e13e0a7b57c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.6 MB (385563209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b77e861f60a2da3e2c3af5d4dcb8cd19a11a1862fa9b80ddccb0c168e8e3ec9f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 18 Oct 2022 00:39:41 GMT
ADD file:a2aadf3cc267a952a6497ccfe5fd0447ab2279d5a88739bf90af1e60794933ce in / 
# Tue, 18 Oct 2022 00:39:42 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 00:40:04 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-7d9a61be4e4c4c426d147ee8e001d0fc0ee22e31883c1aa4a6e093a70e79f0a9.tar.gz"     && echo "93f9eb8517f6f82afa0a927f6edf8d11199d40cdf454b8099ef820e79ac7908b  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:ee9406179427e6b6af08f2294110b752ddd93a1ca950b1572d22e517a92a46a2`  
		Last Modified: Tue, 18 Oct 2022 00:40:45 GMT  
		Size: 56.5 MB (56481754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f3324e83ad5f6d382027fcf8d3c3b31785ddb076e0ccee7669e38742e29ce2`  
		Last Modified: Tue, 18 Oct 2022 00:41:16 GMT  
		Size: 329.1 MB (329081455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:b393108d01e77ff923d602f837fabb1aa545e8b913fbb1f7130d2ca30bde3c54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:c5e654f04302f2f88bdc5fe9644b7a096405205432a3738fc2ca6d4b766b6037
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62303269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01bdb519be2070a170aee5940166344f2a871e7d22887366c0a30406094727bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:19:21 GMT
ADD file:99847692b0f2dee43b50f306ad92fbc13ccb0541af21c6d3040f72d3184aabac in / 
# Thu, 22 Sep 2022 19:19:21 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:e80285ff599e329e689e4689be05885456823b7f6233486aa419541ae8e98c62`  
		Last Modified: Wed, 21 Sep 2022 22:07:12 GMT  
		Size: 62.3 MB (62303269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:10c927b25ed56533d46fc4f2ac0085bc5f8839527c83ee5ea395753b019d899f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63912418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c44e7db5ae05cce1a4890c4507b657d00a595765e478417de6cbe69d4d4eb01`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:39:26 GMT
ADD file:cd0852de8cdfb2b7efdaa53ad4827a33302d895b10306b540e7df9d8c7f00637 in / 
# Thu, 22 Sep 2022 19:39:27 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:f5371f42f94d8ba2c9559448b8e36de82d246f179760ec911f594632d3545611`  
		Last Modified: Wed, 21 Sep 2022 22:07:11 GMT  
		Size: 63.9 MB (63912418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:a4a7095f6cae0281cf3a5f357eda5174a0e2ee3fb1f584858f2740c0958a7eae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:f1c531eaf600c693158c1d1ebbead9146809d78fab280d8bb9fa3b255b8c5af0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486378202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1900d5d0b057d3ad0be96c67ba2666b4016b5a9e87c34e4442e61d12d4002336`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:19:21 GMT
ADD file:99847692b0f2dee43b50f306ad92fbc13ccb0541af21c6d3040f72d3184aabac in / 
# Thu, 22 Sep 2022 19:19:21 GMT
CMD ["/bin/bash"]
# Thu, 22 Sep 2022 19:19:40 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e805f912bcb0541240fd70fe7e7f23e3b79a2c5ce3c273054b3efc087e0cc6a1.tar.gz"     && echo "726894e6d2bbc0a7301d9a191b1197b554ad07319a01e726c537d27e73953785  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:e80285ff599e329e689e4689be05885456823b7f6233486aa419541ae8e98c62`  
		Last Modified: Wed, 21 Sep 2022 22:07:12 GMT  
		Size: 62.3 MB (62303269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d7c2b2aa50fe3ff7023a3909084d659b7f234ce37cb2b8a54bc449bb682a27`  
		Last Modified: Thu, 22 Sep 2022 19:20:48 GMT  
		Size: 424.1 MB (424074933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:c64709a723326277e8bd139dee26c099248a5cfdc15af39276fdab5bfab370e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.0 MB (487987310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e561a7921606d2497a6dd0c931d14e2c4efc3c741a9a665cef47c145e63222`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 22 Sep 2022 19:39:26 GMT
ADD file:cd0852de8cdfb2b7efdaa53ad4827a33302d895b10306b540e7df9d8c7f00637 in / 
# Thu, 22 Sep 2022 19:39:27 GMT
CMD ["/bin/bash"]
# Thu, 22 Sep 2022 19:39:47 GMT
RUN mkdir /usr/src/srpm     && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-e805f912bcb0541240fd70fe7e7f23e3b79a2c5ce3c273054b3efc087e0cc6a1.tar.gz"     && echo "726894e6d2bbc0a7301d9a191b1197b554ad07319a01e726c537d27e73953785  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:f5371f42f94d8ba2c9559448b8e36de82d246f179760ec911f594632d3545611`  
		Last Modified: Wed, 21 Sep 2022 22:07:11 GMT  
		Size: 63.9 MB (63912418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366907dea1a523b535578b50385542ee460f0d786719b57a5b8a57f84d86c59c`  
		Last Modified: Thu, 22 Sep 2022 19:41:14 GMT  
		Size: 424.1 MB (424074892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
