## `debian:testing-backports`

```console
$ docker pull debian@sha256:5983837294cb158a1b669718e739a44343c98d935620c887fafcdb2c4a968a34
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:73f7bf1bda6a125d0464e28a07bb15043bf301e4d6bff543a563ba36ae0dc4c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49278250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7212629620b8eb2e590331a0abc64fb452459244599211dcdbcaba55803fac9b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:32:10 GMT
ADD file:8d8307b9fddc1a85bdc2e0cbae7db307f7175165470e518c843af6017ba20392 in / 
# Thu, 23 Mar 2023 01:32:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:32:14 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6206d2afdcc78a73e0273edeb8fdfdbe4df15938287b733a2bbe2c7d634134cc`  
		Last Modified: Thu, 23 Mar 2023 01:36:54 GMT  
		Size: 49.3 MB (49278028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bc9b418b84c0322c54858c801d5f8a768c7926f209666d2f57cd72cc3d2c3f`  
		Last Modified: Thu, 23 Mar 2023 01:37:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:e8292f26ce78a896ae0c64fa23eefb753aa26c8a8b463aecbdcdaf01eba1734f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48073055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2334c7148c1590a9b2ede897e9ebb66510fa827a27bb86dac9d7abd4de8bc712`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:34 GMT
ADD file:2754fb0733bf053663be45fdf8749e4c88158b9b85a85403f9898c3dfb53215e in / 
# Wed, 01 Mar 2023 01:49:34 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:49:38 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3ec0704dfd86e01503ca7c8e58baaa3616684e2a382e2ae7ce46e3466830b2a1`  
		Last Modified: Wed, 01 Mar 2023 01:54:34 GMT  
		Size: 48.1 MB (48072831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2df0b944c64529f9142b7c44697dbabf1ad89eb38cbf101f8e7cf9c9f631e4d`  
		Last Modified: Wed, 01 Mar 2023 01:54:44 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:f3a4a0a6164a4bef9d6aca228c754c325158118087999851948df49d96cc9c8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45889369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e155478144166795f76ca3697451c79d7c1c0a1b6f472cecf093012d7f6a6f48`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:31:16 GMT
ADD file:4e68f2c6540dd962a59a592ac044a782e3e9d836cc38ab48dc26e9dbccc90bd1 in / 
# Thu, 23 Mar 2023 01:31:17 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:31:20 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e87471986c096ea04657db39da99a36798d80478383fd18d1ea85a33eb174d4d`  
		Last Modified: Thu, 23 Mar 2023 01:35:09 GMT  
		Size: 45.9 MB (45889150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab09dfc5cf2ff86af684a0e3dfa7e320044961a95b6daa28427447b05bf71732`  
		Last Modified: Thu, 23 Mar 2023 01:35:18 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:8d5a65033705d8a2fb721b5b88edf341ac749041722fab94e24268f6d8d1b7d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49328478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed79da747c3ac833850fb71dcccef818fc3cae48fe0f0072d1686c4253a4918`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:46:10 GMT
ADD file:659cb8b541c9a906fe60747ea4b6ec72bb4e3525e53ed5e749127f0d9cb21a15 in / 
# Thu, 23 Mar 2023 00:46:11 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:46:13 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e8c9f32eb3a01effeef152afae1272c7a3054f6070bca27f29886acb89e6b19b`  
		Last Modified: Thu, 23 Mar 2023 00:50:32 GMT  
		Size: 49.3 MB (49328258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba1173fc1cb5f8cfda391f83c4bee2665cc690c0c8faca06011a6816a3181e1`  
		Last Modified: Thu, 23 Mar 2023 00:50:40 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:5fdb01aae3b62fe4d7a01686d14001048040f08774150f6268120a90112c6695
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50324151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73b73e7975be4d15e78c83ef6b297922431229afb9d796c497951a4a7cb7672d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:40:52 GMT
ADD file:f75b62250bff5d8572fec727da09f8822bc35c8a17646f1565d5ff0a13560c8b in / 
# Thu, 23 Mar 2023 00:40:53 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:40:56 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:852656c6bb930aeecbbfdb1c3b074519bbb3b8bb52bb3fad65e3ce1f2019c591`  
		Last Modified: Thu, 23 Mar 2023 00:46:03 GMT  
		Size: 50.3 MB (50323929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5032906680a8f70b9cce144641de62fd9b0024622de4d51ee63a80d0236bbfb`  
		Last Modified: Thu, 23 Mar 2023 00:46:11 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:10b6f73020588e97b4d6c35f65cbf479b1ab5110265e79e34fa80c2cb4f0416e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49245732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16940537906a118a74e5b233a78dbf1ccfb92383fafe7e6d9b7ba52d9d64f8aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:13:45 GMT
ADD file:1bf792d3c4330d4faf867dfb2e9689482bcfd0a8d9c641abd7cca9b6a218978f in / 
# Wed, 01 Mar 2023 02:13:50 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:01 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9abd347c7d1810d25b14d496d1aea23dffa3a1bdfd637405ff33a4f90244ddcc`  
		Last Modified: Wed, 01 Mar 2023 02:21:51 GMT  
		Size: 49.2 MB (49245506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1df3a413749712800dd37603aeba16f017976baed61398f73e1f2a83ce6ef8`  
		Last Modified: Wed, 01 Mar 2023 02:22:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:fe5e2ad5dccb765b7430eb1658f0103a8d8def2ba9d17358174ca43056ec284c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53290545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157ba61487d39da90215e7850c8b733de2f04cc69f52cd4c2a97aa3a0313f069`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:21:23 GMT
ADD file:bfc3cbce948978fdfb5c510c1a2c7571e7b45792bd78a210a70e292234c6e4c5 in / 
# Thu, 23 Mar 2023 01:21:26 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:21:29 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:493f18ce92294a83aa5e06384c48d22bad737c7a13cfcd85d7928b862798dd46`  
		Last Modified: Thu, 23 Mar 2023 01:26:15 GMT  
		Size: 53.3 MB (53290321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7a9e8476061252d5edec1cd20646b6307e836da234da2a895c26cc2c360d3c`  
		Last Modified: Thu, 23 Mar 2023 01:26:25 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:eadb59faa50d6eedceffc18abe7b1164cbc64ecb2135c7132dfd7831983f7b0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47671241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32c295ceb6b8759dabb96eddc9f82d81bf136acee54f2f9a002514aa9e639f1e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:12 GMT
ADD file:a96b8cacbcadb2068e0368c020589f4d2eae9fabb0965b387d5d9fc94831a1a5 in / 
# Thu, 23 Mar 2023 00:45:16 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:45:21 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:57560ce693355ef04b6283597b61cd71f7e8b7d7357b218eab0c8979bce7812e`  
		Last Modified: Thu, 23 Mar 2023 00:48:17 GMT  
		Size: 47.7 MB (47671021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe413e0a94d09e12d9238564e655958bc2e2ce663985bd7c11d778fadc2fdb76`  
		Last Modified: Thu, 23 Mar 2023 00:48:22 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
