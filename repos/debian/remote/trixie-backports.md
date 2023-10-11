## `debian:trixie-backports`

```console
$ docker pull debian@sha256:33ae8a0f0191a331fa82b04cef6a3423f1fe5a530d4415865fee0b6f26404535
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

### `debian:trixie-backports` - linux; amd64

```console
$ docker pull debian@sha256:d4d8474fd05db07592da3171579a6f559d74fbff3c9797989bd379f3c5490800
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49467891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6385a8cec330c29c1f437defd666b1fc7894d03d731a283fde4d1ba4cfe9ddf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:58:17 GMT
ADD file:cd33732baf7a8215a9cb532ae6f2fe0be64d030adb1f3e0085e461cf4f22ec4d in / 
# Wed, 20 Sep 2023 04:58:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 04:58:21 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3954180d94025620e480192adbba35d582d59582f662e17f992f954d83539feb`  
		Last Modified: Wed, 20 Sep 2023 05:04:48 GMT  
		Size: 49.5 MB (49467670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4584eea246440188150b069ce8e544a63936f951d6d80dce0400ab2407128b0a`  
		Last Modified: Wed, 20 Sep 2023 05:04:57 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:b38203096c3e1e93846688612747dc8ae660469d9e6bf3be4fd8730db504bdc4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47166269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:359b2b54427027ec1a459956df283694446fa4c021de6cc5b4b6cf754113349b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:06 GMT
ADD file:a7de42b73a4591d75c2ea2f44cdd15d34ce24fa78ca8e57ac62e4fd3ffe2019d in / 
# Wed, 11 Oct 2023 17:39:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:39:10 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5a100e11229dc40f9cdcd25e779cd1f10bb500c44c5b9ae24abec0b01f4b26b1`  
		Last Modified: Wed, 11 Oct 2023 17:44:09 GMT  
		Size: 47.2 MB (47166046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4b05cdca4135066ecb9ed2e2648c8cf35a1623f9bc434452872626046cf2bb`  
		Last Modified: Wed, 11 Oct 2023 17:44:19 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:11cf178df019141ab938005b4e662d95e05e2c515ee2c353c0281409b58f8ee2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44954313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf037ac1194dd544fb4ed3c4840bcc0a6d07a82e48381a165a93513a69852f0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:26 GMT
ADD file:69ac67070b211f2a7980ec82da00c1d97d41dc6fe979f892e741ce9b7c566a85 in / 
# Wed, 11 Oct 2023 17:44:26 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:44:29 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:53634a2dc8fdfb2e0bde3647302a9fd6183101ae18e9a9c89ec4d54909761e25`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 45.0 MB (44954093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217d82b41aa5f71309c0a6e360c5f825297956b9f5483b7e89d966fd8582f2fe`  
		Last Modified: Wed, 11 Oct 2023 17:51:05 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:0a4920e0ae737125747f8d0ba6feb8baf957137c17cb26a790a7cd237e525625
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49404723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dacc26ecfc7bd73e1212c9d1770f92debaa64c92afb4154f54a57f6ba522e67e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:58 GMT
ADD file:dc9be3a1e3e1904a1eb81053b568b583a58307e861fc56fb1b7ce9349d2faa18 in / 
# Wed, 20 Sep 2023 02:45:59 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:46:01 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4d433462e04ded836d58eebb0fee68803768bcf3c9f92338a2cdda77bf7bef8d`  
		Last Modified: Wed, 20 Sep 2023 02:51:30 GMT  
		Size: 49.4 MB (49404499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2971bd829e6d4cab6e239fae43246325496a884c068e59a494f1d8c31c6f3b2c`  
		Last Modified: Wed, 20 Sep 2023 02:51:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; 386

```console
$ docker pull debian@sha256:b81c6435230ba46243a7163e971626fe6494d79fc86aa5f82408a4a1b016a0f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50486073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0b3d8ff6edd8b6430aa8881074d81f96bda88cc8cd83316b2b50a76b808d30`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:20 GMT
ADD file:ad97acda5f74778001aece2a9e280f0e58d2953cf8fdbd4740a049c4a595a225 in / 
# Wed, 11 Oct 2023 17:43:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:43:24 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ce8ed34eaeffdeb7ac49225c6093f421b0005558aedb2b9c429731032d156621`  
		Last Modified: Wed, 11 Oct 2023 17:50:59 GMT  
		Size: 50.5 MB (50485846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c4a71932ae7c6a851db412ad9b5bd196b7d6495e0208ba569f8318e1f418c4`  
		Last Modified: Wed, 11 Oct 2023 17:51:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; mips64le

```console
$ docker pull debian@sha256:17cd63c9a77283bfa4a96d506589f6ac3f718e1a483a394dfcc9045ea68ff198
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49301956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0cf97ee24e9422bb9c076ea211cbc03a4bacdce908bd8cecce345434d1bbc8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:56:15 GMT
ADD file:29bed270e296c5a95f2141f114580e0f25c1040c03609fa632757a8e48ec43fd in / 
# Wed, 11 Oct 2023 17:56:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:56:34 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f0d54eafe706e7144ea10a18a0abaa975cb4f7f92fd40e292f388c2b1321a794`  
		Last Modified: Wed, 11 Oct 2023 18:07:41 GMT  
		Size: 49.3 MB (49301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de76dd5ed09e00af07f232282664be7090f11d87d9961bf1e3cd8805bd0fedef`  
		Last Modified: Wed, 11 Oct 2023 18:07:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:f530fa4aedd7ba3f722e80b6250e1c1d2dc960241dd898feb71d860f804ef42b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53418361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068aefaaa095b4d93c737339b42d7cd6064a5e6201721b58560a44f00e0761ed`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:47:23 GMT
ADD file:24d4df221ce118a8059e0559a8bb2d715512fa6f5b15cd1397dbc177ceaa1bfd in / 
# Wed, 11 Oct 2023 17:47:26 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:47:31 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:93b578febbe769059c90eaa91e9dc027d172e6088856c2c52dc3e26dfdf01d4c`  
		Last Modified: Wed, 11 Oct 2023 17:54:24 GMT  
		Size: 53.4 MB (53418134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec77a0be9807ec1d702d27eec6a1c3fae135f6a722ac6684ae2cea2e8067c0d`  
		Last Modified: Wed, 11 Oct 2023 17:54:34 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:trixie-backports` - linux; s390x

```console
$ docker pull debian@sha256:1071bf29df9d0b1172d23a924ee93683c5e78467d34d6c5f13e6d4860ecf00e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48924570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79cf055af48824e812057a42342112a51f5ea027826cb24fb6106f3a1b0bc193`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:11 GMT
ADD file:7f7d0fe596110ed400f2bbc2fe6edf5716a5a62332062c86009df0df0cc0a257 in / 
# Wed, 11 Oct 2023 17:53:14 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:53:22 GMT
RUN echo 'deb http://deb.debian.org/debian trixie-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3f47ccc9a5d62eac06dcd9bcbdf51b3bf5f494156a2c21d58d93d11f5261baf4`  
		Last Modified: Wed, 11 Oct 2023 18:01:45 GMT  
		Size: 48.9 MB (48924346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db50facd80bff41c859ed7a93e81d9da412301a354329ad447672e7eff392ad2`  
		Last Modified: Wed, 11 Oct 2023 18:02:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
