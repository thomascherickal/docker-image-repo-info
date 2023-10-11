## `debian:experimental`

```console
$ docker pull debian@sha256:ffbe0f5a5826e26323933e2637b87e9b036ed8e2f283bd1a68140a2cd45f559d
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

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:2ed4680c1798ce193b44e572397f2f5a6dcfc9dcd3b0eb3c9fb6231f55adb594
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49482951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784e818bf45a27ff34e633bd0f1445c8200fb4a0c2464db47443b5d121a15760`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:58:37 GMT
ADD file:9e949dd6812111c066604c2d4937c93e80b5183362157c5c16a106591f16da4a in / 
# Wed, 20 Sep 2023 04:58:37 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 04:58:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:6ea8d23205362fcfb06aff08d45d594ed9cc1fe0792bf22c588823465349a3c1`  
		Last Modified: Wed, 20 Sep 2023 05:05:22 GMT  
		Size: 49.5 MB (49482731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37f57e4b5b8ed57225597f7ec5153040b58d89f46e2769cc6941b5d8265a3db`  
		Last Modified: Wed, 20 Sep 2023 05:05:43 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:abb6930d10e3341bcf1fef16c3769767523c7cd6c5dea73be04ef409f7bea679
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47165082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f038f9cccdd142b7d37ea6d336d7f35a3bae5a76c3868a6f26e0d963e6acfc22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:22 GMT
ADD file:2b2bcee2ca1f3f375c40ff9a503e7b254a7563adc79e6ab5a9f24c6c3301d92c in / 
# Wed, 11 Oct 2023 17:39:23 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:39:31 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:57382a134b0378f6e86c6c4dd2947ec1c00b8007efd0cb2b9c5116940e89c329`  
		Last Modified: Wed, 11 Oct 2023 17:44:46 GMT  
		Size: 47.2 MB (47164860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0388a46350ecc92f756846ec7389df52e4dfd47b5688ded0e2da5abf87764fc5`  
		Last Modified: Wed, 11 Oct 2023 17:45:10 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:8797b5fe74b7909d51777c89590cc04c12a778969f8d0457aa84bff87f5f3e43
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44953810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27dab457bf47c4305cfc787eb979f4daebcefe7439b9cea1b92116dffc79bfcf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:44 GMT
ADD file:3a7616e78793ef8a223434f89c1abe43568ba17bdd5d3dd77c0efbcb3a0d95f8 in / 
# Wed, 11 Oct 2023 17:44:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:44:53 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9840df9ef2a8f74355857b1d11a95e75445341a4ca233b841b51c28cc8db3d49`  
		Last Modified: Wed, 11 Oct 2023 17:51:32 GMT  
		Size: 45.0 MB (44953586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f803e1d26de4ebf5122d3873fd847af10f7bb3c42c74e172b1ddfd99bc426e`  
		Last Modified: Wed, 11 Oct 2023 17:51:54 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:538261bf0e9adabdef459fc5866ddf8ed62376fd3d93bd826f367d0bb2359467
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49450712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21941270492380aa35b48a746947e8290371565abbac1132b0f9d9e100019abe`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:46:12 GMT
ADD file:c490dc1dd969e985b6ee09de2811426fe3e1f59c999434c58165f20e12999c58 in / 
# Wed, 20 Sep 2023 02:46:13 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:46:21 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3c7710302475abe138bbc1da10c4dd6cf01afcbcc1832cd54e1f313291e8304f`  
		Last Modified: Wed, 20 Sep 2023 02:52:00 GMT  
		Size: 49.5 MB (49450491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1cdcbc9d4070abff87713c27d593a64d42b3322b78f0b6af668886085ae7e9`  
		Last Modified: Wed, 20 Sep 2023 02:52:19 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:352d1f10bd1e226a3ddb00d1b993e8e87fca0404eecbcf16df04f5cb89d6a9c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50485495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0541241d6f2429adf6371dc3be09dfc1c541b5f6e13bac28b159bb20ba6258be`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:41 GMT
ADD file:dfef51f62c576cbdb97969055c452dc62caf5342b0a0be63c6312a95d82e1fee in / 
# Wed, 11 Oct 2023 17:43:41 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:43:52 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:bd61ecff7db7e3fa9d6f072266854c36acbfe9fd2aed28b4f169652a886f5ab5`  
		Last Modified: Wed, 11 Oct 2023 17:51:40 GMT  
		Size: 50.5 MB (50485275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a860930407456136e79793ff654bb46356356f6b6c414e7b3c14bf8cabb5468`  
		Last Modified: Wed, 11 Oct 2023 17:52:07 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:d1a85862a66aad3ab7c645724c97de852ddcd69d9e48167e7d0c30cc70b28922
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49300588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad05e6dac289268e09d8ab190db36615fdc586fa699909c17c5e3f18a290ba0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:57:31 GMT
ADD file:3787b0cb0cdce5b33a784a2f6fd989dedb167ea43116efe53071e686610398bc in / 
# Wed, 11 Oct 2023 17:57:37 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:58:17 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:c2742a84daba456d71d316b58a22426c5e64f4f87cc6c4ba615800419c9b5e25`  
		Last Modified: Wed, 11 Oct 2023 18:08:54 GMT  
		Size: 49.3 MB (49300363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e316b34a96ac53106a522942b53712898b35c7c27735e9dc662a2f234e0353e`  
		Last Modified: Wed, 11 Oct 2023 18:09:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:105bb440ce6dcfff50ce4fee6594490fa7abc5481e53ce890b2ed0bdad32fdb4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53418520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a810af674953e7839398d70c93b3d82ce7e6a347c04d17cc49ce88159705e919`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:47:58 GMT
ADD file:8a1d9d165b874c0ff84b985cc93b5caad49466ada996bd9ce3d8971c653b6bd6 in / 
# Wed, 11 Oct 2023 17:48:02 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:48:21 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ff9d393525b08f92f46c46777f6ac8a5ad1e5c8120ca966479c6d2cab0f45d4a`  
		Last Modified: Wed, 11 Oct 2023 17:55:13 GMT  
		Size: 53.4 MB (53418301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749e5a94f1b98f142cd5e6f8f64f4d05ffebae57eeb095e19925ac8607d50402`  
		Last Modified: Wed, 11 Oct 2023 17:55:45 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:f4378b822f6bed4a0f86aa6ba7c32706fdc983e85771f892eeec27385d223940
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47864098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9978cc964335529d194be1a6af16f0d4779061560477766880c66c5e675e94a9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:54 GMT
ADD file:c1ecdb6a5345ea8c8bca62006aaa8350f4461397e5c8c446b3d8a470d4a0c1ed in / 
# Wed, 11 Oct 2023 17:39:56 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:40:30 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:88cad205016e37a5441bcba16e7fbb88e2a9ce9210aa7f5c2c1d75d79b96c84e`  
		Last Modified: Wed, 11 Oct 2023 17:43:06 GMT  
		Size: 47.9 MB (47863873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6053cfdb1254651c5071fabfee48b0cd1614573c19ddbe63f0ced66011c808`  
		Last Modified: Wed, 11 Oct 2023 17:43:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:96f175f621c15c88560acbcaf77debe12bdfae6e4e89ea3653ab85d775126cea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48923930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e4b3a1a1176a500984fcad010997550f91367f2cad8830a4a3d4ad42cb0d4a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:41 GMT
ADD file:21ced749b1ff37266d0a6648c3fbcc74e65ab1b6af184b69ab8a59bf08b4b311 in / 
# Wed, 11 Oct 2023 17:53:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:54:01 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:dbc510859869b8c851f4760ac1e7610881fbdd53bb2abf48ef05dcbb3a99210b`  
		Last Modified: Wed, 11 Oct 2023 18:02:49 GMT  
		Size: 48.9 MB (48923708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20e954a5892004523954ef880ed94d55f85e82130d0525d03713eb0d609d0b9`  
		Last Modified: Wed, 11 Oct 2023 18:03:29 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
