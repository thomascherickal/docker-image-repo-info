## `debian:testing-backports`

```console
$ docker pull debian@sha256:1f2c8c2e69e8098bd743ff53c99f85e159e3a8aca41816fcf19fe8e440b28566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:0a525a07ad8bbfa6c61e44956787747444c4fd2de9c2d460cd2939e7be663026
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51922920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5eca466c4245c675e0437093d727d7ff1c9eebcb801e68abcce368194d0f74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:24 GMT
ADD file:ef6d0ed43a7e57298514883c056f9c35630c293bcd6a5189ade9a7c839492abf in / 
# Tue, 31 Mar 2020 01:24:24 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:24:29 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c551897442bae279f3dc3299b5e89627f556d06912d81bd777e18eb066414c32`  
		Last Modified: Tue, 31 Mar 2020 01:29:45 GMT  
		Size: 51.9 MB (51922694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9f3509d0d7e4901d568e013123371bedfd18333aee6d0e509fdc7359df07cc`  
		Last Modified: Tue, 31 Mar 2020 01:29:50 GMT  
		Size: 226.0 B  
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
$ docker pull debian@sha256:396ef63c8d5a81b0bfccf5954dccb5383a968d660f4b740f6707a26cc983f149
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53116766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca962c31ca16cc76a4a0236f800655506b31abeaa88eb2ca22e57ed0ab73e6d7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:43:42 GMT
ADD file:8aa8042e164e78fd0ecc9d31ed1516e1902bcf6fc1f255970c0daf5accc23745 in / 
# Thu, 16 Apr 2020 01:43:42 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:43:48 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d6f2db5e3933175c475410e1606c01b7b5093b73964f559cb6575df6bd58b8d0`  
		Last Modified: Thu, 16 Apr 2020 01:49:51 GMT  
		Size: 53.1 MB (53116542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb13ba1a44351dabe287eae12ab44c44edfd03ae0c39a7474632260d0e98e1d`  
		Last Modified: Thu, 16 Apr 2020 01:49:56 GMT  
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
