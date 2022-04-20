## `debian:rc-buggy`

```console
$ docker pull debian@sha256:7dc8211e6493ef75565d805a59c9a8e2d933a3f40532663486017ded30648cc8
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
$ docker pull debian@sha256:44263d20df1fc634877f59256459bf6ac75502a1e17da3a99e0229be04b11fba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.1 MB (56112788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de96b6ea729e5e4feca37bbd1123cd9d51b5024a3907505f027ff059ec1f566b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:44:37 GMT
ADD file:859abf2d579747b132742454ad96e32dc879955afff8af84fab63dc41312a0e0 in / 
# Wed, 20 Apr 2022 04:44:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:46:10 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:212be0dc3a8ffdc400158a5e3a9812f7413dbb5a86269ff50e41b84b37fdb9f7`  
		Last Modified: Wed, 20 Apr 2022 04:50:51 GMT  
		Size: 56.1 MB (56112566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dd6831f9568bd76d2215a05bb28aeb4f27d47c57302f6f79005a3cca616fcc`  
		Last Modified: Wed, 20 Apr 2022 04:54:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v5

```console
$ docker pull debian@sha256:be943ec362a510134e7a610997179b4eeab895d37eca1d3892057311013fe366
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53518714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:081ff399031684549d25ad4cd357406851873b8b1987ef2e8ff6d5e3b8b244a1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:20:15 GMT
ADD file:5cf288f7326d2adfff5d4d3ad0b8951ab86c23ab83cbd1d7799d5c3f7e16a857 in / 
# Wed, 20 Apr 2022 07:20:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:25:04 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:8db2a46143e157b04953cf05194b0c408afa491a70876185538ed8dca91f9f55`  
		Last Modified: Wed, 20 Apr 2022 07:37:08 GMT  
		Size: 53.5 MB (53518487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3edae2b955816dd61420df6f8651c24acb6625bd1dca09a2f2175d2adadf0c`  
		Last Modified: Wed, 20 Apr 2022 07:43:20 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm variant v7

```console
$ docker pull debian@sha256:b8ba5d0c8373da0e6c3733da46dc5ae711e6974478b55de6dcfb4b29e07d8ff3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51125893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38af82d290611f53d346af21193260ef62a3030754afe471bab1c3d93bee6d73`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:31:17 GMT
ADD file:0bbaf7ead1d59ceb682d490a4942a357b01272b17a3eb062c89673ee4e166052 in / 
# Wed, 20 Apr 2022 13:31:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:36:20 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2bdfb6c7c7f66a4f6d01a8add17283f952a25f6c31c2267fd53d1ff9148edc16`  
		Last Modified: Wed, 20 Apr 2022 13:48:09 GMT  
		Size: 51.1 MB (51125664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a0b3d3b2e91dcbab7183261c268de2e4e250580a9431cc3c4ca0372cab0ec0`  
		Last Modified: Wed, 20 Apr 2022 13:53:59 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:f2c882c8c2fa7ca3e90ae4d4330e68553c48c42043e5537c185412bc31895fa1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55064030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15628421858686cee7f25a0ec8d68dc32ffccf4706c58be07f6ca579e7029de8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:30:37 GMT
ADD file:21175f4b5f80ba5d755041ff362152a8991b53f89e3c6699275e0c99f6ff6acd in / 
# Wed, 20 Apr 2022 04:30:38 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:32:30 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:414d522b7454847f294a8c61536f57f36cb195df33ab1fce8c838de3d5ae109e`  
		Last Modified: Wed, 20 Apr 2022 04:38:18 GMT  
		Size: 55.1 MB (55063805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0618986ec147bd863b6a8cea7ee692a66f12d587dd47d451895ae7c0ab65baf`  
		Last Modified: Wed, 20 Apr 2022 04:41:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; 386

```console
$ docker pull debian@sha256:3c546b9abfe22250450a44bcf01f5f2c42c5b21788f329d61809230e8f8fbcc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57154243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4ec8e9655311040fafed267a624b16e994247c75cb868493e92fdb077a2026c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:39:08 GMT
ADD file:92a4df746589380f0ee875ec89574f67fa2f56164bbf20da79eaa902a778eff6 in / 
# Wed, 20 Apr 2022 07:39:09 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:41:14 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b42fb3c96c9db2aa67a5b3b033791b735ef01e8c8f15321f44a085532b703190`  
		Last Modified: Wed, 20 Apr 2022 07:47:30 GMT  
		Size: 57.2 MB (57154017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5559635446e91cbf6742e4a4085e246cc0814a5163f6d729020cab3f169216`  
		Last Modified: Wed, 20 Apr 2022 07:51:04 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; mips64le

```console
$ docker pull debian@sha256:693c8732f637f85b07570f191e52820e5d104611e0d249f1f9ad2d609e3ab7d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54772511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52fc048038f2d99658426fdfe81100135c276c5d5a86b23c59a0cf5156866a1c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 14:31:30 GMT
ADD file:3ad0c34fcd14c5fe7c8ebdd604aaf6408b7bd1797df3867dc95c1e62649776f0 in / 
# Wed, 20 Apr 2022 14:31:34 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 14:36:00 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:5f4c77aff8255984992f37180c0f928131e7372860c0f93b1c0b9320726de80d`  
		Last Modified: Wed, 20 Apr 2022 14:42:37 GMT  
		Size: 54.8 MB (54772282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1668cdc79a42af14ac0b22dc9a6fafd7c2a7f448c171a94a7000029e3b4da0c6`  
		Last Modified: Wed, 20 Apr 2022 14:47:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; ppc64le

```console
$ docker pull debian@sha256:bb9f528b66bafce1fc13b4e7a7ec7f4ea731d96baf69d140d84f14fbe6f0d244
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60558229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8968f4824cb98430a28f23c5618a28e7503aabab2d0a5b9e1c40d4ef2d07971`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:49:13 GMT
ADD file:fe481980541905937ff6238feab8ead20ee273dfc616bf9e647446ec0f98b510 in / 
# Wed, 20 Apr 2022 09:49:19 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:53:08 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:7a4e99688ea8909140343db9b1a83e87f7ddcee1e1ba6d630b79487e5e720199`  
		Last Modified: Wed, 20 Apr 2022 09:59:29 GMT  
		Size: 60.6 MB (60558000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0515ac2c161210aa1b518129517bf62841f211b9608b3d8b946ee301acbc25d4`  
		Last Modified: Wed, 20 Apr 2022 10:02:53 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:rc-buggy` - linux; s390x

```console
$ docker pull debian@sha256:e0ce76cb0f35098ed00f2fbdce5e98241669e75d37856dafccb6d0aab2aa92f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54331196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:536c75ccd7ef158fee7a049176b94ed29052e8eeb69c6117da42e6f99d02da8c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:42:10 GMT
ADD file:39be572f6c0b3f6f84497807d4bcb370f80b4ac4167f1857002b5571a4dba6b2 in / 
# Wed, 20 Apr 2022 08:42:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 08:45:59 GMT
RUN echo 'deb http://deb.debian.org/debian rc-buggy main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2d9529e5f0bb592a3bb453a841aee9e6a765fede232bccdc538ec2c8b96421d2`  
		Last Modified: Wed, 20 Apr 2022 08:51:05 GMT  
		Size: 54.3 MB (54330969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd965c6427627772edfce6c727e7a17cef230fa08f03eed51055d19429c5f44`  
		Last Modified: Wed, 20 Apr 2022 08:53:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
