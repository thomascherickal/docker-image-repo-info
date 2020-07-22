## `debian:experimental-20200720`

```console
$ docker pull debian@sha256:761416101c9f6f5d7b1a03974df1fe933c7b2e0ff45b356e1039fcaef18ca454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; s390x

### `debian:experimental-20200720` - linux; amd64

```console
$ docker pull debian@sha256:fc4faff077aeadd107f6d5fa759c3e1ddd2d3927cc16587379c0cfb7269a5fc2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52340511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:616c0bd1d54fd38e78576b9226a5833959ff331a4dc0f54f1c24037b03fe0a54`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:08:07 GMT
ADD file:721780a83b9ecd1c3ea680c963dca8e8ecc345481bf807aa4dab082fc5322443 in / 
# Wed, 22 Jul 2020 02:08:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:08:28 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9760f327e5ea357a0446f3036ce75f6309673b69b16167e5cf89184fcf56f228`  
		Last Modified: Wed, 22 Jul 2020 02:13:06 GMT  
		Size: 52.3 MB (52340292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedf91c2851bbdbaad1cbef3750342726b781edec0a70d369a4ed6e0fb5184c5`  
		Last Modified: Wed, 22 Jul 2020 02:13:20 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200720` - linux; arm variant v5

```console
$ docker pull debian@sha256:6b19146f95f1962b6747c9ac91c368d5617549babccd57fc2a3b324f19a7084c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50268903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a949ec04771b4b5bf3a8bc4cc4a6d46c248cec2b3cd2b51636992c4980ea5fe6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:56:17 GMT
ADD file:56cddf74f350d3289e1cf8f72486f85a1136e186e0b395a88454f8649b2b58e5 in / 
# Wed, 22 Jul 2020 00:56:20 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:56:42 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:12385a4eba6600ff6763a993ec9371a0a2553fb5cd604fd23d02d693350e8661`  
		Last Modified: Wed, 22 Jul 2020 01:04:36 GMT  
		Size: 50.3 MB (50268680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a893de48c0c5358d540c47084241f1a011ec03158517ded5b1ab7c8d278abaea`  
		Last Modified: Wed, 22 Jul 2020 01:04:58 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200720` - linux; arm variant v7

```console
$ docker pull debian@sha256:4d95bf39a6324fba746f036c2dab2fdcb02a04fe9172e21f95a6066c3c8349d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48046777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2226dc226dbe574a87b69fa179d2eb41beda02b2f712d3b4475dfeb28345363b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:36:23 GMT
ADD file:9aff7af4262a688d1c25236cd2067da994bd371572ba02ae34d7a5383aa4cc9f in / 
# Wed, 22 Jul 2020 01:36:33 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:38:04 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b321227a313811bf73b88e3ba26f16c7a555e51d176de967f75868342456e199`  
		Last Modified: Wed, 22 Jul 2020 01:45:30 GMT  
		Size: 48.0 MB (48046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d929d204995a024cfd122ffceae6812a6a885acb759ebd539e4cd3c8ded6137`  
		Last Modified: Wed, 22 Jul 2020 01:45:54 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200720` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:fddcc0d247c8112eb23d40c96dff8895a399e89153f08c38eef000d189725572
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50699778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:045dc0b0db953fb5c1466e72d907bfcd806a633bd12353ef0275fd842cd6c397`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:45:16 GMT
ADD file:a0750403ac81eed436a38d00099fd2e6caf1823ec340641d4d739dcafeac0d86 in / 
# Wed, 22 Jul 2020 00:45:19 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:45:47 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:75039184104e63d906128306cce9873fb84c9dfc98087052f03f3bc87f060b1c`  
		Last Modified: Wed, 22 Jul 2020 00:51:15 GMT  
		Size: 50.7 MB (50699557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed84faba5931dcdea3e6e03b165aa6a94b55eeeb176c66c3ee2cae786c258535`  
		Last Modified: Wed, 22 Jul 2020 00:51:36 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200720` - linux; 386

```console
$ docker pull debian@sha256:a02820d2654f6aeef04f52c970e4061701bf97aacb32c4d8f39c9577a8ada7e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53433813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f21d8af9ca264d119b490d2b3a6ba52bb64fe2914e6dd05bc914669d29f8b8a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 02:13:31 GMT
ADD file:b1108bffabfe9fcf6dad1ed7928671d562a99c455a0066cdd1eaf3c7cb438b94 in / 
# Wed, 22 Jul 2020 02:13:32 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:13:50 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:a50ef4752fdcd4ae5fc565c3e74bac4e9a04122eb724e666cecc081601564954`  
		Last Modified: Wed, 22 Jul 2020 02:20:20 GMT  
		Size: 53.4 MB (53433595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05fc27c78bc901c2ecab15a6e860f3eaab59daaacb52fb6188d8854098a598d`  
		Last Modified: Wed, 22 Jul 2020 02:20:35 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200720` - linux; mips64le

```console
$ docker pull debian@sha256:fe588d01d9ec4731360ef68349a34cd040a58b257dad7fa60e2713b880f512e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51079102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f90ab20c9dfd5046d0f3a1beba6468cb8e0683781960dbd60991bf5b9361311`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 01:13:06 GMT
ADD file:95573cfac38269a692511a10c8de5f5cca452449d9005669715cc884d478d81c in / 
# Wed, 22 Jul 2020 01:13:07 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:13:34 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0f99d3ce0ef9d710b01baac97fd0028cad68b26b56c1410680e8e97c27a66606`  
		Last Modified: Wed, 22 Jul 2020 01:21:32 GMT  
		Size: 51.1 MB (51078878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4c1c897a6e7a623f065de7b4f16dd5895ee871e721db53c9a1bb82d50ed56c`  
		Last Modified: Wed, 22 Jul 2020 01:22:13 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20200720` - linux; s390x

```console
$ docker pull debian@sha256:d50080f8690bf2179a7b08d6f9c0fabf9a3a222203aca02e0606228b5b1a9d76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50903367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:789285a20cd69e9f4acb69e3aba94541cb2261f158bdd92ab946dcbe145bd130`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:44:20 GMT
ADD file:d2d04b6f49562d7fb8530670b2d00ab5b1e210f05b138abffd723a3d179018f1 in / 
# Wed, 22 Jul 2020 00:44:22 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 00:44:39 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2a34b8c774abed8b9eddf311f31e28cdf84daccac8c7293fe4b357ae6814bbed`  
		Last Modified: Wed, 22 Jul 2020 00:47:37 GMT  
		Size: 50.9 MB (50903149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecfc309fde5057c7f102c5e74518150db890cb8a6ed75df1ec0a134c6e47c2a`  
		Last Modified: Wed, 22 Jul 2020 00:47:51 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
