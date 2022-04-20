## `debian:buster-backports`

```console
$ docker pull debian@sha256:fa8535312428bd169b9e40b110c53e0537c0e3718b707a76cf94f275e1f401ba
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

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:aa99e15dabc88c67375a5bcd4b0b330678a97fadf536a804ed886f481786c096
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50437207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db6737e6e3305c6605f023abed0975cb0abcceb5c222ed50e51d386abd1333ba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:37 GMT
ADD file:7c5789fb822bda2652d7addee832c5a3d71733f0f94f97d89b0c5570c0840829 in / 
# Wed, 20 Apr 2022 04:43:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:43:40 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:85bed84afb9a834cf090b55d2e584abd55b4792d93b750db896f486680638344`  
		Last Modified: Wed, 20 Apr 2022 04:48:49 GMT  
		Size: 50.4 MB (50436985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6bd587522a21952ca26470113c848c07d020fa048297162069cacfcc13d431`  
		Last Modified: Wed, 20 Apr 2022 04:49:04 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d6e0b137fd859993be272212793c6b224e9862b8486ba55559d3e08dc16d51f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48153831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119a27061a4d5330e432df69d2f4bc94650a79a194fc83cf37757fdcebd0974b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:17:11 GMT
ADD file:ad329516525d9a2e9eecb4bd6263809faafa65bbd9e6deebcda8196b0ea24234 in / 
# Wed, 20 Apr 2022 07:17:12 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:17:28 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d426a13b8d217ec7cc2eceea9d798d79a1c36c60cb9363d2ef2d86abcf895e88`  
		Last Modified: Wed, 20 Apr 2022 07:33:13 GMT  
		Size: 48.2 MB (48153607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081520d2a94fe831c1eca81aaebb40486e92c1d2ff0c9094d41d8ba579a86e14`  
		Last Modified: Wed, 20 Apr 2022 07:33:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b20d2e24f04079c04e9a39ec01e9e4ba0008b958dd6011b63e9e9aaf03924262
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45908369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a60d696958ed4b474fd446b464f25d6dc0dc82ea6c90deb714a8614bd2a41b9d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:49 GMT
ADD file:fbbe7a4ec12b0fdfa82879ff73d49ba760c5b6cc47b4c8ecabe64f7e8f4e6340 in / 
# Wed, 20 Apr 2022 13:27:50 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:28:05 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ca53ad6266ed4ba4323f1553d8b226d0a180384cd290a8361ab19347f6d761fa`  
		Last Modified: Wed, 20 Apr 2022 13:44:25 GMT  
		Size: 45.9 MB (45908143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b0b86771b0c247f208f44f8c27d1dd1a68614155acca96c36e48683d954cd6`  
		Last Modified: Wed, 20 Apr 2022 13:44:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c221b609f44c706d88518d5afa4e25b2a389688cb437b9d52c1f373caabdb57c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49227960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae36706ec6d034436705f6490f83278531fc593c23eb4025103249c71660daf7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:22 GMT
ADD file:5286ff5db23c42ac6a437e8f2f9ef01b6ee6e523d7866c752428d54f177c7108 in / 
# Wed, 20 Apr 2022 04:29:22 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:29:29 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b9f330b3a7e234282d632d95bd19a655cf0e06c1a76a51d0f73b9581be8f851b`  
		Last Modified: Wed, 20 Apr 2022 04:36:12 GMT  
		Size: 49.2 MB (49227738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcf61c50bc20ce89acc6da83284c168f8a27dee2f04757a4d43ec7785f79daf`  
		Last Modified: Wed, 20 Apr 2022 04:36:28 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:73beaf0209cdb2bda81e69cbd97bfeac26411c10dbbaf8bad2b4e023afd2ce54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51196090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12970f12d60844dbc23d54c178bea432ea784490909b718ed6d74e4413f50d9b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:47 GMT
ADD file:f66ba5e7b2801d19041661506f244a3bb89fc613e2e27891bdba3183bd6ee097 in / 
# Wed, 20 Apr 2022 07:37:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:37:55 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6e8f333ddc9f58dd9e74b1f250e3812ba3942ef13abee1d6b4e3d3131a7e29ff`  
		Last Modified: Wed, 20 Apr 2022 07:45:17 GMT  
		Size: 51.2 MB (51195868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f744635066267b8ec0833903081dcd12425841a698105cda576ce096163160b`  
		Last Modified: Wed, 20 Apr 2022 07:45:34 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; mips64le

```console
$ docker pull debian@sha256:bab804f5fef6357c1140b07ae0bc308f005bf7d427cc718310f17f23f5900942
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49071170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07fa847521bc900ac92934a41c31e00903f8e0c023c0f6d51cdcad7a950748c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 14:29:07 GMT
ADD file:4d72d556af68726f3f6b8a1201825561024a6b9863d3458352941912fff3a1b7 in / 
# Wed, 20 Apr 2022 14:29:12 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 14:29:22 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cd1d11c7d9330cfc741196dea55cb8a7bfad252f4b3640a183c09af331282960`  
		Last Modified: Wed, 20 Apr 2022 14:40:00 GMT  
		Size: 49.1 MB (49070945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db03463d2c87a12579e24422713018d4fc83d9ffd436bc14134955a4b41d00f`  
		Last Modified: Wed, 20 Apr 2022 14:40:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:4dbbe597fe1f25894f385d02c2ff67f055244c8ccf0a0164d7c94763e6b77707
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.2 MB (54170099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb5483cb1442bf80e1c8f7be7f71c55108770078838458c7d23381a0d68a3e3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:47:08 GMT
ADD file:0e047f9a02092945498103cc7b6483b67ad3a6d4945ac61230d539e4b6e14663 in / 
# Wed, 20 Apr 2022 09:47:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:47:31 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c9d81baca7c32c0c0c5ac628e027c3c89760343d8a3469fbf7c764d60badfa23`  
		Last Modified: Wed, 20 Apr 2022 09:57:27 GMT  
		Size: 54.2 MB (54169874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb012f4f2706e9479637735267f86262a6a19d9894b78beb2b53049d261db8a`  
		Last Modified: Wed, 20 Apr 2022 09:57:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; s390x

```console
$ docker pull debian@sha256:d269d06592391adbea776fcdf4668a495b7ee3fb56f7112d39e9f6d55523d52a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48999449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1f632b1436c781b44b51848336bb7e325a3ea66c788af7f4602f648312d488b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:40:05 GMT
ADD file:fedc64967d4810188e8bd8289de1b1848a9501e7c68ae5bd4af83377fb9e3108 in / 
# Wed, 20 Apr 2022 08:40:12 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 08:40:25 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5c2799a5996f1eb24bb7f4c0219facf7e95c780314bb9e9b62594f1fe56cd511`  
		Last Modified: Wed, 20 Apr 2022 08:49:56 GMT  
		Size: 49.0 MB (48999225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3422788b4b795ea88c9c68a41d74c3cc960912d937b142a8bb66ab25f19d7c1`  
		Last Modified: Wed, 20 Apr 2022 08:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
