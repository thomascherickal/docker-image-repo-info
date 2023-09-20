## `debian:rc-buggy`

```console
$ docker pull debian@sha256:6d892063c7f7d4d9927571ff46dc4216a84570e895ee70af12915b4fb0bf9faa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:c75151fb1cfc072c3c7d217b33fe707405e2328212e38a04a757293935d17b20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49492552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:862ceba2c06948531099780ec3f5dc82df5bb40ccb499b46a8a4aa10063747fa`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:22:27 GMT
ADD file:bd8ad5ff1bfae3fed182d348486f9719820be43c8b6b13ad4385f6cc6a15ce87 in / 
# Thu, 07 Sep 2023 00:22:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:24:04 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6c36f0cb17f99a82a25600b41f67d97eba8474b1cc58f325f0d1307303171b68`  
		Last Modified: Thu, 07 Sep 2023 00:28:36 GMT  
		Size: 49.5 MB (49492324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7215c599af5fba780e6183c0ae74d3a337be48d6ff6c7ad3302779edca2c0b6e`  
		Last Modified: Thu, 07 Sep 2023 00:31:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:4f7ce6d0d652b1487d9b618d38c61360383c47a8a036f8111bda223ba3ae4fa2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47166112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd7c79e21ca55bb1956da3fed152891d52dcf8ef38007f7d616182bb778b2512`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:51:01 GMT
ADD file:4c775ca1c9a8c87b9e1d380ae08f73f13d6c554601a5b87aef7f73b399316a50 in / 
# Wed, 20 Sep 2023 00:51:02 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:53:07 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:af64b4d6568f99d4aba6c0cd1799711a18174e7c92ab564f1783b1b859742070`  
		Last Modified: Wed, 20 Sep 2023 00:56:46 GMT  
		Size: 47.2 MB (47165885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef5ee7f1773b1180abf295093ffe99722c416b7817855dddff569b108ba3ab1`  
		Last Modified: Wed, 20 Sep 2023 01:00:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:12d39fd4ea7f9a79a410e6866613485acafbd17b75045f8ba57c0392fc9d7f3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44983470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f31aa6ecf0e6332a841ba821421ee9a722e4c369a1bdd1adccf10c182aaed8e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:59:28 GMT
ADD file:48b9003b5f16cca577ade266eaa0f16a82c1470540f591ca5b3478846402f252 in / 
# Thu, 07 Sep 2023 00:59:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:01:01 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d85f55a7a6c774695f75c1a7ec0bc0caeb915349d9250d2f4e6737e12fcc92fc`  
		Last Modified: Thu, 07 Sep 2023 01:05:21 GMT  
		Size: 45.0 MB (44983245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605e9adc328599a497771357e30d70633b648ec7d759b652a4c78c49cf9e36c1`  
		Last Modified: Thu, 07 Sep 2023 01:07:55 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:85e2564f5b21e054c934e406e5e33d820c323496bd166c1cfecfd390f4e593fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49450716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d133d098236a20aa09484102a2808aa91e01a011f45e27fef4507a981a6324`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:16 GMT
ADD file:3493f4ad2710629ee9ad4c981682b2afcc1d9964cb5034de77189556f0c0e810 in / 
# Wed, 20 Sep 2023 02:45:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:46:23 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d83e3b52cf7f7a250777a05d8d2d7960fd6dba8a6438beed3879ff3c389bb01b`  
		Last Modified: Wed, 20 Sep 2023 02:50:04 GMT  
		Size: 49.5 MB (49450488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb5191978a2e1433d7d932ed3bf3fb213113be6f09dca5a12e1a588f5c6ee7a`  
		Last Modified: Wed, 20 Sep 2023 02:52:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:6ce469c68e21c916aa9632af587b836f67d137866735be08be9cfb73c4d09f37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50483353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dabfd2a8f4bfcbf3090fe8144287dc60f26e249972cfcf447c867ad64bb67ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:43:36 GMT
ADD file:89a1cfdf26e23095cc168a8c054aaa8afe0cb7f1b748f0dbca755e9aad935ce8 in / 
# Wed, 20 Sep 2023 00:43:37 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 00:45:14 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a77a25e288eca9c35f0aeada81ba65e2f4beb3d0b739a139eb41bdd87309a97b`  
		Last Modified: Wed, 20 Sep 2023 00:50:06 GMT  
		Size: 50.5 MB (50483129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65acddf67d2eb98450a115639d2bcc9e755c36d058420daf8f24b08474f60324`  
		Last Modified: Wed, 20 Sep 2023 00:53:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:9166a08987ff23de27f2a3c84b6c5662e9a70559ca1cd3fd57c07cdd77c42ae1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49338165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d848c74a60a576865e64bce227bea97fc71671f461480df817230efcc5678ab`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:12:16 GMT
ADD file:a0f62fb4629026abfbc8955434580788fb6798315ec2cbb9fff3b490cae4ae5f in / 
# Thu, 07 Sep 2023 01:12:22 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:18:10 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:fbf3aa413814601f6b34fe509eeee19b8570d10547318d9e50b786a1305da8f5`  
		Last Modified: Thu, 07 Sep 2023 01:23:38 GMT  
		Size: 49.3 MB (49337937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397a379ebd061cee838e1abd438e7cbba4b82450ee334b4c381356b712e8974a`  
		Last Modified: Thu, 07 Sep 2023 01:29:16 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:0b201c53e85c1c31c1a52046f5e5f70b548da766227954cec93c5ec3507265de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53430051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02446067c4091cd97ebb6d00a8b124c0adca0e12d8b871f6e17180a9bd243ff`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:19:03 GMT
ADD file:0a03052b027b835521a56eb544f68d37afd082caf6b0f2a86d36ba3a4df23574 in / 
# Thu, 07 Sep 2023 00:19:07 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:21:56 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:61513ad4f292fbcfceaab5e01ed63b82ba881a99736b2ffd97579f96947c0829`  
		Last Modified: Thu, 07 Sep 2023 00:25:38 GMT  
		Size: 53.4 MB (53429824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fa69f9835a1f2c348460f80fe08b5f8f18414aeb954120e6a1429c38022615`  
		Last Modified: Thu, 07 Sep 2023 00:29:13 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; riscv64

```console
$ docker pull debian@sha256:46abc0df6f9937cc7588360f715b1a3e81a56250938955792f058dc913409cc0
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47886231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90508f15e429e4b3f1811cb12897631267f4fc757bfa892661080b4501cbc60b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 01:10:40 GMT
ADD file:1f642efb72cdde4ae806c2daa6011fc8bf9064f9ca1495c204a2329c8224085e in / 
# Wed, 20 Sep 2023 01:10:42 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 01:12:28 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:dd92315c0266263460bbfc9a32f8e00d31dd51aaf5819be923d34de88ddf3545`  
		Last Modified: Wed, 20 Sep 2023 01:13:31 GMT  
		Size: 47.9 MB (47886004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bddbdd63848c4d04b14caf62c39cd997a14cdfe2add8c16bb4d882d36ee490`  
		Last Modified: Wed, 20 Sep 2023 01:15:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:1bf9fc9393923b6ebd6e46c9e6c88b29dbdfd561957f95c503e943492e9d7141
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48852906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f1786d5c9cc070e471cda8507660e8eff63ecb24483b02205c37bd364f2423`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:55:43 GMT
ADD file:aeb19ed2c9b92cbe76bb1e733b04de5bcb32489c00c1c06504aef79cd36c3c3f in / 
# Wed, 20 Sep 2023 02:55:50 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:58:28 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b1b4950b21705690e4b15e5257a0efcf7d334776307aaa893216166a5c37f2c0`  
		Last Modified: Wed, 20 Sep 2023 03:01:02 GMT  
		Size: 48.9 MB (48852678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbb598bcea03e6abf06908bd3a806ca2c446227b541282a7fc316d35d6f5b8c`  
		Last Modified: Wed, 20 Sep 2023 03:03:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
