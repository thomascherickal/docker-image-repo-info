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
$ docker pull amazonlinux@sha256:deadcaae52851831a2f579185eceb9e86c824d67c25334fbd5ef2ee75cf525a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2` - linux; amd64

```console
$ docker pull amazonlinux@sha256:49b6d61fd3efc7ec126eddbb9a9c692fe89678d12f69aa96bf834ab10c30c762
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61655014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2d92bc1c0c25b0e15c00cfaa44320d84af71ab3fe97280d53a7b769cd96c19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:46:32 GMT
ADD file:119ae574c5d5b6e59e83ecadbe4c8dc4e7b535508e63704e74939df696c9b9a1 in / 
# Wed, 01 Apr 2020 06:46:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a8d577519c9fb37ef239a77026a16c019d20cce14b25867f57a44459b3bbf387`  
		Last Modified: Wed, 01 Apr 2020 06:48:00 GMT  
		Size: 61.7 MB (61655014 bytes)  
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

**does not exist** (yet?)

## `amazonlinux:2.0.20200406.0-with-sources`

**does not exist** (yet?)

## `amazonlinux:2-with-sources`

```console
$ docker pull amazonlinux@sha256:1c2ff16aec2969b471271d267c5d3458c3a99fc8f584c410464de5e56a29d060
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:2-with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ae9a60bb771a5d7bae7d2b72be76465aa0fbba01798369693da7118683e76f8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476793057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4edff84f869f5f2809dbcac4472a16c86a631e32be729065f187f37796636caf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:46:32 GMT
ADD file:119ae574c5d5b6e59e83ecadbe4c8dc4e7b535508e63704e74939df696c9b9a1 in / 
# Wed, 01 Apr 2020 06:46:33 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 06:47:00 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-4cda1b0d98865d12f61886af2ff052cf2cb4a48734bded0ac84d2664a0361220.tar.gz"  && echo "c53ef45b008bcb392f9ecbd229a6fa38f69cfe536d630560a8e1a8daaa8b68e6  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a8d577519c9fb37ef239a77026a16c019d20cce14b25867f57a44459b3bbf387`  
		Last Modified: Wed, 01 Apr 2020 06:48:00 GMT  
		Size: 61.7 MB (61655014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639485fb25df7e0bf5f7dfa45a2d1bf8980e990acd57646e3a7904ddbfd99ba3`  
		Last Modified: Wed, 01 Apr 2020 06:48:23 GMT  
		Size: 415.1 MB (415138043 bytes)  
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
$ docker pull amazonlinux@sha256:deadcaae52851831a2f579185eceb9e86c824d67c25334fbd5ef2ee75cf525a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:latest` - linux; amd64

```console
$ docker pull amazonlinux@sha256:49b6d61fd3efc7ec126eddbb9a9c692fe89678d12f69aa96bf834ab10c30c762
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61655014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2d92bc1c0c25b0e15c00cfaa44320d84af71ab3fe97280d53a7b769cd96c19`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:46:32 GMT
ADD file:119ae574c5d5b6e59e83ecadbe4c8dc4e7b535508e63704e74939df696c9b9a1 in / 
# Wed, 01 Apr 2020 06:46:33 GMT
CMD ["/bin/bash"]
```

-	Layers:
	-	`sha256:a8d577519c9fb37ef239a77026a16c019d20cce14b25867f57a44459b3bbf387`  
		Last Modified: Wed, 01 Apr 2020 06:48:00 GMT  
		Size: 61.7 MB (61655014 bytes)  
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
$ docker pull amazonlinux@sha256:1c2ff16aec2969b471271d267c5d3458c3a99fc8f584c410464de5e56a29d060
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazonlinux:with-sources` - linux; amd64

```console
$ docker pull amazonlinux@sha256:ae9a60bb771a5d7bae7d2b72be76465aa0fbba01798369693da7118683e76f8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **476.8 MB (476793057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4edff84f869f5f2809dbcac4472a16c86a631e32be729065f187f37796636caf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 01 Apr 2020 06:46:32 GMT
ADD file:119ae574c5d5b6e59e83ecadbe4c8dc4e7b535508e63704e74939df696c9b9a1 in / 
# Wed, 01 Apr 2020 06:46:33 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 06:47:00 GMT
RUN mkdir /usr/src/srpm  && curl -o /usr/src/srpm/srpm-bundle.tar.gz "https://amazon-linux-docker-sources.s3-accelerate.amazonaws.com/srpm-bundle-4cda1b0d98865d12f61886af2ff052cf2cb4a48734bded0ac84d2664a0361220.tar.gz"  && echo "c53ef45b008bcb392f9ecbd229a6fa38f69cfe536d630560a8e1a8daaa8b68e6  /usr/src/srpm/srpm-bundle.tar.gz" | sha256sum -c -
```

-	Layers:
	-	`sha256:a8d577519c9fb37ef239a77026a16c019d20cce14b25867f57a44459b3bbf387`  
		Last Modified: Wed, 01 Apr 2020 06:48:00 GMT  
		Size: 61.7 MB (61655014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639485fb25df7e0bf5f7dfa45a2d1bf8980e990acd57646e3a7904ddbfd99ba3`  
		Last Modified: Wed, 01 Apr 2020 06:48:23 GMT  
		Size: 415.1 MB (415138043 bytes)  
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
