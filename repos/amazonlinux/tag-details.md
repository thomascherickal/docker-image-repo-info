<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `amazonlinux`

-	[`amazonlinux:1`](#amazonlinux1)
-	[`amazonlinux:1-with-sources`](#amazonlinux1-with-sources)
-	[`amazonlinux:2`](#amazonlinux2)
-	[`amazonlinux:2018.03`](#amazonlinux201803)
-	[`amazonlinux:2018.03.0.20200318.1`](#amazonlinux2018030202003181)
-	[`amazonlinux:2018.03.0.20200318.1-with-sources`](#amazonlinux2018030202003181-with-sources)
-	[`amazonlinux:2018.03-with-sources`](#amazonlinux201803-with-sources)
-	[`amazonlinux:2.0.20200406.0`](#amazonlinux20202004060)
-	[`amazonlinux:2.0.20200406.0-with-sources`](#amazonlinux20202004060-with-sources)
-	[`amazonlinux:2-with-sources`](#amazonlinux2-with-sources)
-	[`amazonlinux:latest`](#amazonlinuxlatest)
-	[`amazonlinux:with-sources`](#amazonlinuxwith-sources)

## `amazonlinux:1`

```console
$ docker pull amazonlinux@sha256:859097367161e0db986971d89e50e38541f9b94a7af95d6c9826ebe545fcd2f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:548e328ccb1bbbad1dbda7f99ffaefd4483824631e5320dbe11f9e49b4761c67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62364391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356215688295370198dee0429295b30026a677f5446c31e7b35cd6d46a47481a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:47:16 GMT
ADD file:4e38236f7bb16fe8537e7b062a1c7dd1bf0e3b3ff96f29709f3347d42002ce93 in / 
# Wed, 01 Apr 2020 06:47:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c107763d15738a6ee301905ccb676bc809201dfd0806984eba9f82e07b99cb79`  
		Last Modified: Wed, 01 Apr 2020 06:48:39 GMT  
		Size: 62.4 MB (62364391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:1-with-sources`

```console
$ docker pull amazonlinux@sha256:cedf10b8eb4977ce42083ee8356c79f569003b167888594e9204d17af7fca85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2eb54dce9209bfc2d447a194931061e65934ead40995052e87d2785d7a7e7959
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.0 MB (451011498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52e5298652a35bfba8d2e89e2cfdcb408241a180d73ef360e5cd1e4899b3506`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:47:16 GMT
ADD file:4e38236f7bb16fe8537e7b062a1c7dd1bf0e3b3ff96f29709f3347d42002ce93 in / 
# Wed, 01 Apr 2020 06:47:16 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 06:47:40 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1f39c46b9f2dee01a647e53170c3c40bed489f7f522519d33d00c5e082eda17a.tar.gz"  && echo "4c7e33ec81dd7b7e9ed483bd8da66073d5d891b96d0836ccbf0e78946014e6f9  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c107763d15738a6ee301905ccb676bc809201dfd0806984eba9f82e07b99cb79`  
		Last Modified: Wed, 01 Apr 2020 06:48:39 GMT  
		Size: 62.4 MB (62364391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc813f620189d5cf8ce0987dcadaa297db6e20ab616e692d1633c6f51f7b08`  
		Last Modified: Wed, 01 Apr 2020 06:49:01 GMT  
		Size: 388.6 MB (388647107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2`

```console
$ docker pull amazonlinux@sha256:436544dbd50a2f1f876390b9c2b09e98d73badb222ba188d69d58e649aa1b6b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:b7f1b202905250e8c51d70d5d0bab048728fb59e73dbf92c694f6c9f13621afc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61619066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f335821efb5e5b95b36541004fa0287732a11f97a4a0ff807cc065746f82538`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:64e35bbe6ac618aef32fc4924b8ab8b576d6085056a285dc311b07ec9138e8c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63079760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39751b5fb90d450e678e5b9f4403d064d2e730da6c334f7ddcc4c4ffb4a4f33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03`

```console
$ docker pull amazonlinux@sha256:859097367161e0db986971d89e50e38541f9b94a7af95d6c9826ebe545fcd2f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03` - linux; amd64

```console
$ docker pull amazonlinux@sha256:548e328ccb1bbbad1dbda7f99ffaefd4483824631e5320dbe11f9e49b4761c67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62364391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356215688295370198dee0429295b30026a677f5446c31e7b35cd6d46a47481a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:47:16 GMT
ADD file:4e38236f7bb16fe8537e7b062a1c7dd1bf0e3b3ff96f29709f3347d42002ce93 in / 
# Wed, 01 Apr 2020 06:47:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c107763d15738a6ee301905ccb676bc809201dfd0806984eba9f82e07b99cb79`  
		Last Modified: Wed, 01 Apr 2020 06:48:39 GMT  
		Size: 62.4 MB (62364391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20200318.1`

```console
$ docker pull amazonlinux@sha256:859097367161e0db986971d89e50e38541f9b94a7af95d6c9826ebe545fcd2f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20200318.1` - linux; amd64

```console
$ docker pull amazonlinux@sha256:548e328ccb1bbbad1dbda7f99ffaefd4483824631e5320dbe11f9e49b4761c67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62364391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:356215688295370198dee0429295b30026a677f5446c31e7b35cd6d46a47481a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:47:16 GMT
ADD file:4e38236f7bb16fe8537e7b062a1c7dd1bf0e3b3ff96f29709f3347d42002ce93 in / 
# Wed, 01 Apr 2020 06:47:16 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:c107763d15738a6ee301905ccb676bc809201dfd0806984eba9f82e07b99cb79`  
		Last Modified: Wed, 01 Apr 2020 06:48:39 GMT  
		Size: 62.4 MB (62364391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03.0.20200318.1-with-sources`

```console
$ docker pull amazonlinux@sha256:cedf10b8eb4977ce42083ee8356c79f569003b167888594e9204d17af7fca85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03.0.20200318.1-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2eb54dce9209bfc2d447a194931061e65934ead40995052e87d2785d7a7e7959
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.0 MB (451011498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52e5298652a35bfba8d2e89e2cfdcb408241a180d73ef360e5cd1e4899b3506`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:47:16 GMT
ADD file:4e38236f7bb16fe8537e7b062a1c7dd1bf0e3b3ff96f29709f3347d42002ce93 in / 
# Wed, 01 Apr 2020 06:47:16 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 06:47:40 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1f39c46b9f2dee01a647e53170c3c40bed489f7f522519d33d00c5e082eda17a.tar.gz"  && echo "4c7e33ec81dd7b7e9ed483bd8da66073d5d891b96d0836ccbf0e78946014e6f9  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c107763d15738a6ee301905ccb676bc809201dfd0806984eba9f82e07b99cb79`  
		Last Modified: Wed, 01 Apr 2020 06:48:39 GMT  
		Size: 62.4 MB (62364391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc813f620189d5cf8ce0987dcadaa297db6e20ab616e692d1633c6f51f7b08`  
		Last Modified: Wed, 01 Apr 2020 06:49:01 GMT  
		Size: 388.6 MB (388647107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2018.03-with-sources`

```console
$ docker pull amazonlinux@sha256:cedf10b8eb4977ce42083ee8356c79f569003b167888594e9204d17af7fca85f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazonlinux:2018.03-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:2eb54dce9209bfc2d447a194931061e65934ead40995052e87d2785d7a7e7959
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.0 MB (451011498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52e5298652a35bfba8d2e89e2cfdcb408241a180d73ef360e5cd1e4899b3506`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:47:16 GMT
ADD file:4e38236f7bb16fe8537e7b062a1c7dd1bf0e3b3ff96f29709f3347d42002ce93 in / 
# Wed, 01 Apr 2020 06:47:16 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 06:47:40 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-1f39c46b9f2dee01a647e53170c3c40bed489f7f522519d33d00c5e082eda17a.tar.gz"  && echo "4c7e33ec81dd7b7e9ed483bd8da66073d5d891b96d0836ccbf0e78946014e6f9  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:c107763d15738a6ee301905ccb676bc809201dfd0806984eba9f82e07b99cb79`  
		Last Modified: Wed, 01 Apr 2020 06:48:39 GMT  
		Size: 62.4 MB (62364391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc813f620189d5cf8ce0987dcadaa297db6e20ab616e692d1633c6f51f7b08`  
		Last Modified: Wed, 01 Apr 2020 06:49:01 GMT  
		Size: 388.6 MB (388647107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20200406.0`

```console
$ docker pull amazonlinux@sha256:436544dbd50a2f1f876390b9c2b09e98d73badb222ba188d69d58e649aa1b6b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20200406.0` - linux; amd64

```console
$ docker pull amazonlinux@sha256:b7f1b202905250e8c51d70d5d0bab048728fb59e73dbf92c694f6c9f13621afc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61619066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f335821efb5e5b95b36541004fa0287732a11f97a4a0ff807cc065746f82538`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20200406.0` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:64e35bbe6ac618aef32fc4924b8ab8b576d6085056a285dc311b07ec9138e8c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63079760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39751b5fb90d450e678e5b9f4403d064d2e730da6c334f7ddcc4c4ffb4a4f33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2.0.20200406.0-with-sources`

```console
$ docker pull amazonlinux@sha256:c49fd49d868b56f1454f7734a3bfdc5b502cdd80963f669458251b146e4b4cd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2.0.20200406.0-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:1070545f3003036660f858836efcf7b089f5f33c9c3da98c664e5d6303957a50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476758547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712d2767ea76ecb265150bae981829b198c60d9ce3fbef60ef2fe247219c0ff3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:23:21 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85b52563080715b3858df242f64ffaa92212a60bfd97b7e9e9bd506b80663b2`  
		Last Modified: Tue, 21 Apr 2020 18:24:16 GMT  
		Size: 415.1 MB (415139481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2.0.20200406.0-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4cbc0732124bed6fdb615eaf60c2d4bb7cc134d957d1f9674dc0066a438ce1bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478219309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca4e24672d702283a87cbf97240f20bed3724d62ff8f8dcfb9a0baed82da19a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:59:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f9d710835018ff01a17ccc9e3b4ce18e9cf9f81a0dc1cf8d455472d9a1d29`  
		Last Modified: Tue, 21 Apr 2020 19:00:52 GMT  
		Size: 415.1 MB (415139549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:c49fd49d868b56f1454f7734a3bfdc5b502cdd80963f669458251b146e4b4cd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:1070545f3003036660f858836efcf7b089f5f33c9c3da98c664e5d6303957a50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476758547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712d2767ea76ecb265150bae981829b198c60d9ce3fbef60ef2fe247219c0ff3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:23:21 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85b52563080715b3858df242f64ffaa92212a60bfd97b7e9e9bd506b80663b2`  
		Last Modified: Tue, 21 Apr 2020 18:24:16 GMT  
		Size: 415.1 MB (415139481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:2-with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4cbc0732124bed6fdb615eaf60c2d4bb7cc134d957d1f9674dc0066a438ce1bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478219309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca4e24672d702283a87cbf97240f20bed3724d62ff8f8dcfb9a0baed82da19a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:59:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f9d710835018ff01a17ccc9e3b4ce18e9cf9f81a0dc1cf8d455472d9a1d29`  
		Last Modified: Tue, 21 Apr 2020 19:00:52 GMT  
		Size: 415.1 MB (415139549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:latest`

```console
$ docker pull amazonlinux@sha256:436544dbd50a2f1f876390b9c2b09e98d73badb222ba188d69d58e649aa1b6b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:b7f1b202905250e8c51d70d5d0bab048728fb59e73dbf92c694f6c9f13621afc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61619066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f335821efb5e5b95b36541004fa0287732a11f97a4a0ff807cc065746f82538`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:latest` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:64e35bbe6ac618aef32fc4924b8ab8b576d6085056a285dc311b07ec9138e8c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63079760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39751b5fb90d450e678e5b9f4403d064d2e730da6c334f7ddcc4c4ffb4a4f33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `amazonlinux:with-sources`

```console
$ docker pull amazonlinux@sha256:c49fd49d868b56f1454f7734a3bfdc5b502cdd80963f669458251b146e4b4cd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:1070545f3003036660f858836efcf7b089f5f33c9c3da98c664e5d6303957a50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476758547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:712d2767ea76ecb265150bae981829b198c60d9ce3fbef60ef2fe247219c0ff3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:23:21 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85b52563080715b3858df242f64ffaa92212a60bfd97b7e9e9bd506b80663b2`  
		Last Modified: Tue, 21 Apr 2020 18:24:16 GMT  
		Size: 415.1 MB (415139481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazonlinux:with-sources` - linux; arm64 variant v8

```console
$ docker pull amazonlinux@sha256:4cbc0732124bed6fdb615eaf60c2d4bb7cc134d957d1f9674dc0066a438ce1bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **478.2 MB (478219309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aca4e24672d702283a87cbf97240f20bed3724d62ff8f8dcfb9a0baed82da19a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:59:09 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-44ab891c498d922bb21e90b6006b12c7f05381ec7e67aba05bb535aae3b261b1.tar.gz"  && echo "a1b70378c6175331c9daa5bee79c8cb36dab14ed1fb0d02bfd33254652f0b846  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f9d710835018ff01a17ccc9e3b4ce18e9cf9f81a0dc1cf8d455472d9a1d29`  
		Last Modified: Tue, 21 Apr 2020 19:00:52 GMT  
		Size: 415.1 MB (415139549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
