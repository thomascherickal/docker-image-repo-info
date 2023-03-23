## `debian:rc-buggy`

```console
$ docker pull debian@sha256:1e277b753afe6e273b18a169fe868c64b96e1d38ffa00f923a17bf2873eb0830
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

### `debian:rc-buggy` - linux; amd64

```console
$ docker pull debian@sha256:232b5fd011b12453068c8e006967f2a52e2b7b79fba99933ee72c1266cd74e09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49291862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244f91d57358a09ed84fba7ed1ebc4b198a4c0693d134ef3999dffe85a672d24`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:31:25 GMT
ADD file:8efef3fd1e16c5994e0b27af5c19056cc369818d299aaf62b89b89ad82426fe3 in / 
# Thu, 23 Mar 2023 01:31:25 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:32:50 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ddb08f6d450933d22f98a93a56726ec0491dcd496caf4455cfe7066900409348`  
		Last Modified: Thu, 23 Mar 2023 01:35:52 GMT  
		Size: 49.3 MB (49291637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ff5ca1ed1b75cc80a36b3e5b8c397119db89a500da3c7633b51b79c09900f3`  
		Last Modified: Thu, 23 Mar 2023 01:37:54 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:290fad6388e5f8303bc47d4a25aea60bfa09c96d59d4efc85b9460b59a367fd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48108007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1864a4ada56cade710496d0b44f529a2f3f4f583bad19e9c82d7d5087f965e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:01 GMT
ADD file:4fadb88d3ead8d91349c79d7e903bbb8f6130b292bda6cb8099131210a815bc1 in / 
# Wed, 01 Mar 2023 01:49:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:50:06 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a03e1abdb2ebe924d64faf35eb6563891039999ec54a62f65419caf539ba6a88`  
		Last Modified: Wed, 01 Mar 2023 01:53:21 GMT  
		Size: 48.1 MB (48107781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a697f4f7c80925375ac8e1d74ed3a3d64fab57f396b32037ef2c661adb7a0d08`  
		Last Modified: Wed, 01 Mar 2023 01:55:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:ae787365a75c0406aa32262b12702673ffbeb4d9ab71ece0df657bb367be1fa1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45911424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff56154b351f7ad0a1adfffc87daaf75bb62b75d52c4890fe741ceaaad2f2e4b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:28:43 GMT
ADD file:628ac1300ca273dba23c7d617164bc6e664cdebb4106910020d7b3dcb39429c8 in / 
# Thu, 23 Mar 2023 01:28:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:31:57 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:53d7f1f008e91cd29c47c933b404c16fc1d4cf64b8699ad1269e882f53ca6e2d`  
		Last Modified: Thu, 23 Mar 2023 01:34:10 GMT  
		Size: 45.9 MB (45911196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605c55259a39add2691d1f3f12092b368e83d0c232f0db9042a1e57369a9406f`  
		Last Modified: Thu, 23 Mar 2023 01:36:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ea483426fa2ad36f0df345f0be5c1da2f08dc7c1d675cc0fee80de400ad7d88d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49319211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cc532b4c05015061075b90ba414a680ef4a2c3068b8a45d3aa2be31751ab754`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:42 GMT
ADD file:56248f74ca6cf497dee2c80a5824447bf5ee5e730a9c092f440d9c666ec1c076 in / 
# Thu, 23 Mar 2023 00:45:43 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:46:35 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3a84baeeebe4b5ede833105ba5c2fe8b6102a8c47c386cc79b5833fea9489c99`  
		Last Modified: Thu, 23 Mar 2023 00:49:34 GMT  
		Size: 49.3 MB (49318983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1218fd8da6a783a7dc13948785148890b1f787d35a34b7a33f08e61e50d27d`  
		Last Modified: Thu, 23 Mar 2023 00:51:32 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:87e94af4b6f84983c723824e1f39e9dc117d6fbd96c18f8937320cfc2951ccde
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50314774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64a29e44d5a250eb35d8dc8ddc47b61b347c969c2b526e3c877daff6724bbf2b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:40:10 GMT
ADD file:b6719d98d83dc3affc1d45dd9bc533456f19b9fbedf5369cde4c632f24f6146c in / 
# Thu, 23 Mar 2023 00:40:11 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:41:28 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:1dab6ed4b4dcc22cec1b58fa38e2c22941443603bb1cb3a1f4025cca4556556b`  
		Last Modified: Thu, 23 Mar 2023 00:44:54 GMT  
		Size: 50.3 MB (50314549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac699be48ae71b195e1ea27dfc98b7530ad28a4ccb23169da88af9712c796275`  
		Last Modified: Thu, 23 Mar 2023 00:47:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:ef7a575c4c94bf7f83b23523f71b2743a3f9ac5ca6df035536f259a95ca61692
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49270858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b95bfba2f90e5bb2900b0ece3641df3230b9b0ffa9bd0461facc5b859957e25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:11:29 GMT
ADD file:0cba93ebf4cf24adc0d2ab76ca2285ed3e4c1d07e2498a55a964f61a47d0f560 in / 
# Wed, 01 Mar 2023 02:11:34 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:15:48 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:f6fa2f96bfa02eb0ced41b1f356f7b6aa1c6dcd2de446f0e6931fb513751316f`  
		Last Modified: Wed, 01 Mar 2023 02:19:32 GMT  
		Size: 49.3 MB (49270629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7c91f5e78bc69e91c7416d2e341fe57c9750d7eed97f94a40ca593b7b151ad`  
		Last Modified: Wed, 01 Mar 2023 02:23:51 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:1c20b0823aff24dc623b4f3736ca5145e490e772baf78db3ae213f6570161227
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53290397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0ebd54df83a24b95f32df620c4c6c97e9605ca65f444de1795fe2419761c63`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:05 GMT
ADD file:3534cf3f10dae5b70c64865fd70cf5b9aa6ace6be9caa2d69518d6d59c4943fa in / 
# Thu, 23 Mar 2023 01:20:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:22:22 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8de2c12bac6cdfac096a845424e637222b157d221d8080dfc0e3cd14581716d5`  
		Last Modified: Thu, 23 Mar 2023 01:24:47 GMT  
		Size: 53.3 MB (53290173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aba8265353d30b6e06113115ba72c33137842cee29bd0d2c05b0a183fee0061`  
		Last Modified: Thu, 23 Mar 2023 01:27:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:52928246f6e589113851c199192094ef2077432ac0d2ba0cfdae3decedd4297e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47648268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:756dab91a3d3492f5e975478f8afd839066353fb72a9304255c24dbad91767eb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:17 GMT
ADD file:f722c963bb9fb9eed0d7ba7fa5de1fdaf0fac91107cd71702d55f0cc074cd6ee in / 
# Thu, 23 Mar 2023 00:44:20 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:46:00 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:866ca1f7e7197a336b8f05cbbb9eb6e6a32a17ade3068f3bd62dd93f926293d6`  
		Last Modified: Thu, 23 Mar 2023 00:47:32 GMT  
		Size: 47.6 MB (47648043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7948cf364c5012447b59e2ff3ba220ed2cc8b7246d571ec8756cf6e267074c4`  
		Last Modified: Thu, 23 Mar 2023 00:49:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
