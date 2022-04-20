## `debian:stable-backports`

```console
$ docker pull debian@sha256:59f67f4c4a26c7155658b8a19b64d920a3702d44707eb3dd625fef7c2a266b6e
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
$ docker pull debian@sha256:4fe98bd09fc7cbfffe8e3ea24a53c851778469c037fdc8d051421bbb2cfa2a54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50133942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d9ac26ebc67aacd57469e44ba70c8bd0e03e675e277ae253de2a97e8cdeae0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 13:32:11 GMT
ADD file:ed430d73187a99b2caa4e7b1596b9ebcd4662344b0610aafccdc9178a9e803ac in / 
# Wed, 20 Apr 2022 13:32:12 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:32:25 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:567476beb4c5ffe964b4f185e7884956f7af30a95f00283da4daf1684841b17b`  
		Last Modified: Wed, 20 Apr 2022 13:49:21 GMT  
		Size: 50.1 MB (50133717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f00418b6b6f607491af856868b8692cd348b48161cef5809e8879b2f4203d9`  
		Last Modified: Wed, 20 Apr 2022 13:49:33 GMT  
		Size: 225.0 B  
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
$ docker pull debian@sha256:daf74e00f52987dd7f89f1234fcf242804d0ec5f260565cd18d3e64fa7d5bb62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53203483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:947d3fb2306255f4d1d668219b6a1fae75a5f28f58f30be75e130e5ba1309c58`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 14:32:34 GMT
ADD file:24a080970cfc5d917a4ea5a8b1f488f34c988ece6535259aaea0a287042dbaa0 in / 
# Wed, 20 Apr 2022 14:32:39 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 14:32:53 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cf3cb3f2bc71af4c1e96d89bf589b5205dba5cff404af0b1a2090fadb02b18fb`  
		Last Modified: Wed, 20 Apr 2022 14:43:53 GMT  
		Size: 53.2 MB (53203259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989b6ab4b24643393317fdeacdab30a3da40ea470fe401945bbe6409583251fb`  
		Last Modified: Wed, 20 Apr 2022 14:44:03 GMT  
		Size: 224.0 B  
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
