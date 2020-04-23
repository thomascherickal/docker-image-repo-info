## `debian:testing-backports`

```console
$ docker pull debian@sha256:d05a059efc2be4ca1c9669ce7e2d9405ce99b4fd76f724dbbb40799cd375f107
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:0544e5c816241880d5f106ea4e6d4285e6dce1632b0faa742ad857651462bb80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51981441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11739e8e919a4028558b6c2e41cf64a4deace1adf075f522f0c89012eda9d791`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:15 GMT
ADD file:19296a07e1c4a35ef4bd6813edc5f8402d5c77ce03f19354ec6b9b7db5286aa5 in / 
# Thu, 23 Apr 2020 00:23:15 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:23:20 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2dffa903b83a05e8f7056f2d8f378ea21af1cbc9a30f68bb9f93f103520963cb`  
		Last Modified: Thu, 23 Apr 2020 00:27:59 GMT  
		Size: 52.0 MB (51981219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbcba46f841681351a4185769b62f19610cf165ffd1d25594fd88dd88ff6f345`  
		Last Modified: Thu, 23 Apr 2020 00:28:04 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:1f410d957e7be97b492bd2a80218546c0475ed43f67a09b19e997d2452e5df4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49911793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8095e99177349cbedfea9388974cad50b99d049791e04932b97ccf2a9093572c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:55:14 GMT
ADD file:3b996b1e7d5b0484318fdd8c256c2a7f3e3dabe2f06b200ea2dd06071d3c212b in / 
# Thu, 16 Apr 2020 00:55:16 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:55:23 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ba15baf41b545b49d09fcdb81d89baaadd11fb24a179aa88f278d1e383105ea2`  
		Last Modified: Thu, 16 Apr 2020 01:02:55 GMT  
		Size: 49.9 MB (49911569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bab565dbd34f2d9c059df424e44b66e761d12eae953c8fc1ea054972cf6578`  
		Last Modified: Thu, 16 Apr 2020 01:03:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:204bbfa19ce08f5db16ee23ec926224384d55b8d483531957f3180c5ba37974f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47646630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75e71f0aedc76c836241c1f63f6e4dbc99e70987320c07707abf75c5d5681a1c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:05:34 GMT
ADD file:12b4fd3ef0ecafd7ed60f3ae19a40668b936f1e950757499333778dd68c8a1a4 in / 
# Thu, 16 Apr 2020 01:05:35 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:05:45 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:66256cc4ea6ae5fd4fd9d1f4c5f00901aef3fdbc90f55cded458d05d71bcc9c0`  
		Last Modified: Thu, 16 Apr 2020 01:12:54 GMT  
		Size: 47.6 MB (47646406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d335ca48327bd7097bc731cf8e0ffc3cbfc8c8ff6e887861ba1168f25ee40b`  
		Last Modified: Thu, 16 Apr 2020 01:13:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:4f7a0b53e01e991a8755cae8be25c83bdad0c2b3f88f14b8e93bb77a7da9aa73
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50901725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6ababc59f0eaccbd3f2f48ad5eb34bd3563b5c6183c64d23ea45ca6c17802af`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:45:43 GMT
ADD file:7889791d9d8a0f23f6f4ab6a0d8682d85f7e7a1e9b4d848520bc142d9beddeb3 in / 
# Thu, 16 Apr 2020 02:45:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:45:57 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c6cd2124ee36486f20d00d2b543361b5c507677295c8c211c433d5f2b9884a90`  
		Last Modified: Thu, 16 Apr 2020 02:51:53 GMT  
		Size: 50.9 MB (50901502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebee629158b07e25422210c6abc723eba515d7172aaf5a4e877b9ee95cf8c91e`  
		Last Modified: Thu, 16 Apr 2020 02:52:02 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:8b95788867388515eb44ca5e04e7c27b587ad03e69bbf89595c1a23f296f4ffc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53125025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b09658ced217763e2641de41d3307c5d79e035a81e3c6059bfc3f2521cb5c5d3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:42:25 GMT
ADD file:66ce6a333e02ded4796aed0b73dca44eebdcd10d3276bfafd6e35cce8b33bad4 in / 
# Thu, 23 Apr 2020 00:42:26 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:42:32 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:41e5514480560cfa8cd27b0138fe7133857c22a04253775d736219697aeed383`  
		Last Modified: Thu, 23 Apr 2020 00:47:58 GMT  
		Size: 53.1 MB (53124802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8ebb1596a647d5db3cf5badf6831601ac5c3076e05ea6493f45ba355f0c7a4`  
		Last Modified: Thu, 23 Apr 2020 00:48:03 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:15a9357dc0574dcca3702045003cea303af8fecc4de2e7badd1621e096b793ff
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50694393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42a0656a07eaad7289444a0dd0d5b2ff3fc4cdecd1c14098b76012841d7f1e2f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:13:17 GMT
ADD file:8965afefe80113b22b46512994393e31ae3e3b6b28467833d110149837d0c6f0 in / 
# Thu, 23 Apr 2020 00:13:18 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:13:24 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:aca473d24d99f30e88d712637b8d1cb5d936e098336de55bb3b14fddba634a60`  
		Last Modified: Thu, 23 Apr 2020 00:24:09 GMT  
		Size: 50.7 MB (50694169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d387ba1a35fbbb390416cd8e01b593063e759b186c3256053acad90c504d1197`  
		Last Modified: Thu, 23 Apr 2020 00:24:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:0e8f22e1fdd777018f02ff369983c4a4a29e68769fa42cfd8b50b4399ce7ff85
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55848328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf08151cc0719bed71d9428feadb8d7ce4d3bc5c223eb9edd78024be5f17e1c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:44:27 GMT
ADD file:e945c8520157fcc7358156614aec15e724dbd20f568803df9a3849cac07d0b22 in / 
# Thu, 16 Apr 2020 01:44:37 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:44:54 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:eb3b1a8d813461d25aac34bdfec6a2fa70c3a8910e327bb7e5fccb15696cabcc`  
		Last Modified: Thu, 16 Apr 2020 02:05:44 GMT  
		Size: 55.8 MB (55848104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bad06f7ad3e29b66efc2273111078fd7d5b0e18d89c4f7273edc9a3a7373af4`  
		Last Modified: Thu, 16 Apr 2020 02:05:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:50aa60394ae096fe3d1eb87b3b57806ca3e9a3fceabaecc42f3897ead10d544e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50569327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61189303f2f21d468e16654f6470fa74cb908b2b26f577874ebdd3dbc94837bf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:44:14 GMT
ADD file:0533de9145cbfbdc0f63d2810f571b22d55353c5217f473939a6d857aea1449e in / 
# Thu, 16 Apr 2020 00:44:16 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:44:21 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:15947c2a65fa1bd5d95c3d02ecbbedee8ff6a1e58799cfcf81e4256df7fa5855`  
		Last Modified: Thu, 16 Apr 2020 00:48:45 GMT  
		Size: 50.6 MB (50569104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa06162a2f624634bd0d0cea4d6e7ddd5196777a62a55e1a2f787848f6faf44`  
		Last Modified: Thu, 16 Apr 2020 00:48:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
