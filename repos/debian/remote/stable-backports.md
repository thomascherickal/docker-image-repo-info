## `debian:stable-backports`

```console
$ docker pull debian@sha256:c74a9a25a633035ba90035652d94dcd863735f144cf76f2ccd6c0fb563e33ced
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:35981c8993dd9db40ed3becfddb3b6bc4d7d3b9832337368e1cc274a7b289844
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49557830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40ae3c3a98424be7f81ffd5cc7acc71a4f3b5e1d5185afa3d0690abae6b1a46`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:35 GMT
ADD file:d55795d0db42b960cb26a71300c9e09e21a8bd517d9d456b139e107bd11a559f in / 
# Wed, 20 Sep 2023 04:57:36 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 04:57:40 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f479ab1f1d7313a83d1f2617085c8111323342da5f3b6114f4834c955a686a85`  
		Last Modified: Wed, 20 Sep 2023 05:03:41 GMT  
		Size: 49.6 MB (49557606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bf42fb9eb120c785d3743f767ea1b955fdbfba3679127e6c9310aa6e68df5a`  
		Last Modified: Wed, 20 Sep 2023 05:03:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:b7a2bc1e9a3e9fd05609bb5878bf03b25fd22a5f360876cc1ed26ce381cdce53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47355986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ae279f4fa206f8642a889eb2b0071a2377b1e1f97cf04f1b149ee44d12a645a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:35 GMT
ADD file:3dfa21483214d6fd6973bf5ea67b9141553d9c57ab18dd58be011147b89db505 in / 
# Wed, 11 Oct 2023 17:38:36 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:38:38 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:41dcea1ccb0cc2ae430dcfcf53e7bb28141a4c89547aaa5fd95c63c233cc81dd`  
		Last Modified: Wed, 11 Oct 2023 17:42:58 GMT  
		Size: 47.4 MB (47355764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc23ee2b798f6caae09687bb231f0d82fb78626c37bf96bcdd7ee1701d4238`  
		Last Modified: Wed, 11 Oct 2023 17:43:07 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:d4344ae77e079fa9b564a2ffc3771cafc3a6de3be8b34ae903a4a409f1505148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45180504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46f077b1a66b5a378ff26581eda180a55e73f3c116cb3775d81cea4f92f1ea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:49 GMT
ADD file:def114a3538bbcfa27a4ee203f247cce6350377fe1dbfcb49bab3a6cf6b13c94 in / 
# Wed, 11 Oct 2023 17:43:49 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:43:53 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a10bb75b0a43fc3e95263c414cc196144041906e596ee2d10115ce43f5937f10`  
		Last Modified: Wed, 11 Oct 2023 17:49:47 GMT  
		Size: 45.2 MB (45180281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc67b463fae0b44ea0b0c9e83e76a6593d4752a56142c715736aca1efcf85a4`  
		Last Modified: Wed, 11 Oct 2023 17:49:56 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:e00dfd4bc9a982a9d068e46752fa6badfac91e0c6a3c10c22ecbb6710137157c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49592067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f23ad459a1e7b4a6283836bc6f365927196217b89e5e58b465ad21ea0fdea22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:29 GMT
ADD file:ec644050dc5561e64384a4e0d183df970aaeac0750f1f762ffe29b7915295eeb in / 
# Wed, 20 Sep 2023 02:45:30 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 02:45:32 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d3dcf5c113a64725cb576d2f4e678aa926bd6ae3c3f413cd83e23503819fa61c`  
		Last Modified: Wed, 20 Sep 2023 02:50:30 GMT  
		Size: 49.6 MB (49591844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0945e730b58d50b3bf97b17885f7a47077182ab5cf6bfc4698ae0f3dbf1f3d73`  
		Last Modified: Wed, 20 Sep 2023 02:50:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:2c1a4b0b9c8ce61b1ae4bf000ef65d39d21f3b8b845ef46d0413420076e918e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50600967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b312b99d343d3d9677c0bcbbada967e89e28a3180710accab8e0613aaa4a498d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:37 GMT
ADD file:6168d4b38f14ce4fc332add3f9a40d4651c7d3fc6307b4b12fbe624ba851d20a in / 
# Wed, 11 Oct 2023 17:42:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:42:42 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3ee03d88e8927941b8f5c665d5f66b2e72b9713e22546461226216d3f9e0c2cf`  
		Last Modified: Wed, 11 Oct 2023 17:49:38 GMT  
		Size: 50.6 MB (50600744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8d48bb7401057875843dc5843f343690625447079ae6099e73b7d5d34e4f61`  
		Last Modified: Wed, 11 Oct 2023 17:49:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:276b5b53bcf8389e26490a6b4e527bdebef9b32447c3a528fe17219808bb8bfb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49569447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bcaaef1884788efbc56791c420ee31a1ebe393fb298574de96b656a4cb7fd92`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:48 GMT
ADD file:f4ff25ab3d231ea582babbf4f29165c3f65291434332b047fa2d41035314a14c in / 
# Wed, 11 Oct 2023 17:53:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:54:04 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:dba2f8ddfe5caee1ce4991c82269145959dd91d33f8f961efed3aaaf3f2b2deb`  
		Last Modified: Wed, 11 Oct 2023 18:05:13 GMT  
		Size: 49.6 MB (49569221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81863ce58a2fbb32e081d3f63bd239eba2b8ffddc9661442efc7b066fa5d351f`  
		Last Modified: Wed, 11 Oct 2023 18:05:23 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:5574e7dfae11555996699279528877bdafa1c2a21216907389297b0ff67e1d90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53576187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75cd8f3d2d59833bc5dbfc8a7c5f558892cfe04fd84a360df4f37528db0c2c48`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:46:14 GMT
ADD file:6f01471be4c62302b72e885495b3b47e7744664c11e162b97c2aa2e6ec59793b in / 
# Wed, 11 Oct 2023 17:46:17 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:46:22 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2b4cc8711faf88be58a5dab9e7d686aefbaacdb081873031cf190ad2325ee1cb`  
		Last Modified: Wed, 11 Oct 2023 17:52:52 GMT  
		Size: 53.6 MB (53575965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3551cc446bbd94f534dee055b87dd720b14c930126f72a995a67244b592b61fd`  
		Last Modified: Wed, 11 Oct 2023 17:53:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:a55f90daa7b73dd38991cce6798a0cc0fffafbffc1ab275ee58c767aa158e054
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47943177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef754df2c8f2efa4dfd61686caedbfa9027eae444106fa353921e511ae6b920`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:52:09 GMT
ADD file:9bdfe45aeecbd072e199f7d8fa443992573fe8dfc7d3f534f1cb43eba5659d67 in / 
# Wed, 11 Oct 2023 17:52:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 17:52:20 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:87a37cff3abc315812cf54485b206845e2a4fc1f3d87ca7f1d1d2ec8d930a47b`  
		Last Modified: Wed, 11 Oct 2023 17:59:41 GMT  
		Size: 47.9 MB (47942952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65289eeb1670b59b475e65f88850886658df50ad01b38780b2cab5bde7e1670f`  
		Last Modified: Wed, 11 Oct 2023 18:00:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
