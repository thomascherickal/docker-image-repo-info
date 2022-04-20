## `debian:stable-backports`

```console
$ docker pull debian@sha256:5582d46eb38e38dfa9c9ea03c8bd8f46d8925a0f18ce13fcc2578b022ae5633f
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
$ docker pull debian@sha256:e48257b4c3c946ffd8e961c7ff05895eecf707a5ff53102e778e693d0976bdf4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54942031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6432b06c60d3cdce30a05e1158c966c1d80fe60b2456b7b3488412599cda77f0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:44:55 GMT
ADD file:70d54120d8cfb74e196d7f06205a5afbb6d666c607d98bb6fb288403d27cac5b in / 
# Wed, 20 Apr 2022 04:44:55 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:44:58 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7e4019cb8009a11f4d0c0305817ebafd8aabc5efdd2ccfb680768c686fbf59f1`  
		Last Modified: Wed, 20 Apr 2022 04:51:23 GMT  
		Size: 54.9 MB (54941807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fbc92289b20574efbecaffcafecd68353d8c7d8b0bdcca29247eda94c2bc50`  
		Last Modified: Wed, 20 Apr 2022 04:51:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:1e651b6407e5d02fd96a46b16aa4b7c237a2ebf13944cfc1e29fc0ddca0b1a96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52475036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4876f4114ade2bb394bdc90c917c01697143e3bdd098b9c45852653f7624aea5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:21:06 GMT
ADD file:68b75e09ec08e461705ec78b5040cf58c621ea9c79c137de9a8112de3fdbe5f6 in / 
# Wed, 20 Apr 2022 07:21:07 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:21:20 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:59cbbab28dfd690490cdf7eabe5ef0336e0cd6081d0e42156e2a07a3910bfa47`  
		Last Modified: Wed, 20 Apr 2022 07:38:21 GMT  
		Size: 52.5 MB (52474813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e0a118d3e9d5e5bc2650067587607b96d25b5855f9a937eb02d733d1bc57fd`  
		Last Modified: Wed, 20 Apr 2022 07:38:37 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:fd19f8df3cf4ddd3be30a1b83a267755e8f7a7d2600f5ba2501c986f0576cfc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50134068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7720b9e200b6e69eea4690a4ecff20decdaf47496c1634311ec6ad3a2ca07696`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:22:57 GMT
ADD file:fec28b71de25ce3cf786a79457d6ee9659ae8ac861ecdd680d533c0b664045ca in / 
# Tue, 29 Mar 2022 02:22:58 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:23:11 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:192d4a3a853ea3cdc45d1b46a62cfe119b61b61c9e93ee197c9314032f7fa367`  
		Last Modified: Tue, 29 Mar 2022 02:39:33 GMT  
		Size: 50.1 MB (50133844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cb9419849c842448b21788e55d9cd1b3987376b201e32526e9797cd343a1aa`  
		Last Modified: Tue, 29 Mar 2022 02:39:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:fafc23ff1c9860f1757010c16c774cea89c1456f81f9ba000f667f2f2e4a5e54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53633323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:607729f0e0eb8fc21b82823c7c5f3dcc60b24b2dc03c551a751f7b965cdb900e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:30:56 GMT
ADD file:9cb2ef4274be4c1a318ca57c12ca95f467f143eca0bac4c199e2a86f11c10eb9 in / 
# Wed, 20 Apr 2022 04:30:56 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 04:31:02 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f9d085fb4027d698e9010339730647a2cafcd6b562f259def78de7b561267965`  
		Last Modified: Wed, 20 Apr 2022 04:39:00 GMT  
		Size: 53.6 MB (53633103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763140a5f75386d34014d2975b6f1f53443a8cd19a9c507901afd8ea9aeee9fd`  
		Last Modified: Wed, 20 Apr 2022 04:39:10 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:95c0b4fc58bb5f54ef1942385955fb47b28114efc1dd92ec0f1c48dfe15ef55e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55940909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d06ea66de2b3b53a2390915a3c999b80a7129cb2a50426238389953ba5d0f3f1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:39:30 GMT
ADD file:92b44faca8628d83825b927748987e74da58dffc328fc6c5613c27749255e877 in / 
# Wed, 20 Apr 2022 07:39:31 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:39:37 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:61b9c3fd915ab1c74b16d1e1369048684cd36eed0ead6d0ef99401069fd2fb42`  
		Last Modified: Wed, 20 Apr 2022 07:48:03 GMT  
		Size: 55.9 MB (55940688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5467fe4e9503027a0a01e4b1a28e4aa3f74678d92048518fbbdd539a40248f`  
		Last Modified: Wed, 20 Apr 2022 07:48:13 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:4deb166e82551aab1b3db3af4fdfc1a17ea0444c80e6b6074d1ece9f78638a8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53199555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d6948bbcc454f8859ea7e1db3a470670a78e85161d36771329bbdfaa456d81`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:46:21 GMT
ADD file:0fbef85df7c69585e70b9596838509ae1c00562f24fa354eb32e872202dfa7d6 in / 
# Tue, 29 Mar 2022 07:46:26 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:46:36 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0fb4a12948a42065e860c13e45b3238ccb73f0c66e8c6cc4ad8b23ba7879f522`  
		Last Modified: Tue, 29 Mar 2022 07:57:30 GMT  
		Size: 53.2 MB (53199330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79dad7ad6060aae57a9d550ef733aa04579b3644ccf436f534f6a8f45fd7284`  
		Last Modified: Tue, 29 Mar 2022 07:57:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:5420de5f237cacd006e5a6787bea346401e445dfc47567be4d422321b34d146f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58835483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a38a601136715449ccb26eef56dbe693f07410ab3694c3b86dd86ac5858d3d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 09:50:04 GMT
ADD file:bfd1cdc74762b2fd575c1887fc1ee1830df56a7327ec69522f616240418491be in / 
# Wed, 20 Apr 2022 09:50:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 09:50:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cb41263da1dc6eda181580f28c1b3d2d552197140b58337fdec1318f27f01274`  
		Last Modified: Wed, 20 Apr 2022 10:00:12 GMT  
		Size: 58.8 MB (58835260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765c2fbe4c7936986609f407607d3ffe54f8e73e0479b5c8d1bb286692baec85`  
		Last Modified: Wed, 20 Apr 2022 10:00:27 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:5b2fe8607e9248809058400783c75f604abe474199a79ab1dcf7ad10776d5822
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53207615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9463a3d80a6987deae4b3b5a3cecbb6dd0139e808be60e5516e55c23a4910c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:43:05 GMT
ADD file:a1728962611fc2fb01d4c24d61347ae9f5053b293d5d8650bcd4c196f25744e1 in / 
# Wed, 20 Apr 2022 08:43:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 08:43:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:97f6537fb8406b5d5515b31cb525bb261828bced06956c6ad38e825a1c7131d2`  
		Last Modified: Wed, 20 Apr 2022 08:51:39 GMT  
		Size: 53.2 MB (53207391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4014d2da36b5fdc20f6cf9378e048e3e3643879e3efbd6c971e39bdf9b8125`  
		Last Modified: Wed, 20 Apr 2022 08:51:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
