## `debian:stable-backports`

```console
$ docker pull debian@sha256:adb5935d84fa80c392dd664a07e951814370308324c3826724e583f728ea629d
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
$ docker pull debian@sha256:d923907063c5a4303ac66475765af55fb26ffa9db2e898820b1f9058eb584050
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55045799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f69f129b0c5aac3134ad66e55347948a9c8c33b5c753863e72bb20169af6fe03`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:31:47 GMT
ADD file:bdf2c9eedba0acd35488f592044047931dc5a13a4f0a6923783cbc1ed9657699 in / 
# Thu, 23 Mar 2023 01:31:47 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:31:50 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4ed5f2fb37e281a299382e8fab2bbc22af2994dd30464f32e0f21b5200806a5e`  
		Last Modified: Thu, 23 Mar 2023 01:36:20 GMT  
		Size: 55.0 MB (55045577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f2faf2e45ac8bf9c3668b8824c422d6adaf03e186ed35d267a860244be6b01`  
		Last Modified: Thu, 23 Mar 2023 01:36:30 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:3bdc0404f1b4ea70e7b541ba0bd92a39d2ded60f0f7ca81b3210ceaa73bd659c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52549725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21871bd575e431402829bf51696092b9b998b464677132f44bcabf3a30bb4b74`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:49:05 GMT
ADD file:30388438fd6b8a68ceffc950d98fc11963f9f317825ab87d786d042e8cd97f7f in / 
# Thu, 23 Mar 2023 00:49:06 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:49:08 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a5af868c4b3a926efdb22a9a3b56d17995390b940f566eeaa9b8781cca2f96dc`  
		Last Modified: Fri, 24 Mar 2023 23:22:39 GMT  
		Size: 52.5 MB (52549504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10e5b0aacaedce0e856c9e654b6a30c2f22e1fe222e077aa66a61ed6ff67289`  
		Last Modified: Fri, 24 Mar 2023 23:22:47 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:a731616b4adc80950009dea4daeacafe51de218fe48176d1a321df37d2354c7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50212027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b93c8e297234a5c843b06bca2906fb25890bb6a0238f8f5378077001c7b09bd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:31 GMT
ADD file:75c6ccb0c507d5995bf9631eeb29804be7fd8ed92aeb067d47ab99157f95fae7 in / 
# Thu, 23 Mar 2023 01:30:32 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:30:35 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:fecb0fab7764093a84528aee6bbeedad85dc45ae0dcdd714ddd83c34318c5c76`  
		Last Modified: Thu, 23 Mar 2023 01:34:36 GMT  
		Size: 50.2 MB (50211805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c837a38d6a02225b61b0cca16ccdf7ad77903b4f7ce73a232bdfcb11b9e72e6`  
		Last Modified: Thu, 23 Mar 2023 01:34:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:af5b1a13677dc572a202c915295557ba0a1cc7f36414cdedfba6f2628dae0aca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53703364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6af3ac4b539a67ad49009b0350818704a0074e01984aca3583a88c171532be`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:55 GMT
ADD file:3b227c85bf0970aced33c4da102d7d282e814bf53a84d6a6ef7f581bbc76a7bf in / 
# Thu, 23 Mar 2023 00:45:56 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:45:59 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2312bb915b25efe9ce812b12ae65ea209b43c9ef384f3295eb1c663aa11a97b7`  
		Last Modified: Thu, 23 Mar 2023 00:50:01 GMT  
		Size: 53.7 MB (53703140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4208e1943b2bc6d2be32d78fb560f9a2bb957391905222a90db5de8eb285c7`  
		Last Modified: Thu, 23 Mar 2023 00:50:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:f8d4385f76f1996d13c4bbd524c1eb83161f07ee1a4caaa0f336cb87975b4b1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56028068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef7f5665d1ac0aa9d2b3a2487d0c704c8646b0ffdd0dce5e76b220c632c58f9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:40:31 GMT
ADD file:7e6282db7e6f5f89339f56dff6a7ce78d25479aad91e687d59b76948cd43af7c in / 
# Thu, 23 Mar 2023 00:40:31 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:40:34 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:255456fff76dbf9560f73643299d3b99f21e9ec4f1129ea6904f33328be0add3`  
		Last Modified: Thu, 23 Mar 2023 00:45:26 GMT  
		Size: 56.0 MB (56027847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc4a69a8fc711faca0cd78810adca0d551a9567c69a57f1c28db53991ab21ce`  
		Last Modified: Thu, 23 Mar 2023 00:45:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3afc6521ae370146835af3d78ce80c3a4cfca1a6efff8d2a80f18c4b26c95ead
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53264920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85aded3852f76f632f776ec98c20b6e8d56f8a55438fa3bcc1b201eaedca785`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:19:35 GMT
ADD file:ad71d18fed9a54f08962ed260895e248d5632b0529e80c990e43ecf453414e3f in / 
# Thu, 23 Mar 2023 05:19:41 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 05:19:51 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1b456ecc6382bcff949011c0e1791c82dd243ee3837a15605c016951144bee49`  
		Last Modified: Thu, 23 Mar 2023 05:27:42 GMT  
		Size: 53.3 MB (53264695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735b8960b091e156e5cf0e8a32e03151eb7a3065ef5f200380aeae4c1bab9ddf`  
		Last Modified: Thu, 23 Mar 2023 05:27:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:60483a581e078bfe78132c28f3d275e20a1c46d2431a47fd0abd75422f4db4c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58921248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c4babfeb850f63206ebe75c15139e2597060e5c0d31c2b4a2439195e8003602`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:20:43 GMT
ADD file:d51838f4a37d18901518b506ce14df54086071003c6efa1c9aeae7efdea2d348 in / 
# Thu, 23 Mar 2023 01:20:46 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:20:52 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:beddbecfd1432bd897bb0f2b9cba7063e832605b0e0fbe4bcc4b7d89bd936994`  
		Last Modified: Thu, 23 Mar 2023 01:25:28 GMT  
		Size: 58.9 MB (58921027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da60fd685f7148984323087432b8e1eec70ffc2b50c0a9249605f52a5c822df`  
		Last Modified: Thu, 23 Mar 2023 01:25:38 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:5fd09598a60fea569b4e487566a3c2ce5e7ead38df716e904047db37bc79d33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53277681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c618df44e605abd028560eb9b16c3922bc8be3aebf474b8e0bca911b1e85b822`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:41 GMT
ADD file:0a147643a8506b1b4bccf8b33cb7a3868d9279381b0cd1da59e01d3eb3e3490c in / 
# Thu, 23 Mar 2023 00:44:46 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:44:51 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f5e53e6370cdd67572dcf9ec5a8f5998c3025aff2de4beadf65f001656040863`  
		Last Modified: Thu, 23 Mar 2023 00:47:52 GMT  
		Size: 53.3 MB (53277458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c6dc75bbf8906d791b4ccba1e23ed018394090239d152f8b554f2ffa82a920`  
		Last Modified: Thu, 23 Mar 2023 00:47:58 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
