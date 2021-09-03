## `debian:testing-backports`

```console
$ docker pull debian@sha256:07745b67b1c9624e3ff7288f8014dd18ca58db7428af0675762ef2731ecf5f77
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
$ docker pull debian@sha256:ad74ea2440cc3ec06b60dfa8cc97dd1019fc0bc7325cd5dabfb102e1e6ffb6b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55464862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbe5c50abdc931a6322084c73e0a773d581baa56af8a785c3089229bc91416c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:58 GMT
ADD file:34bf1f6ddafae4895f45a110a2d7ea6139557d82a9508b85d7518a54be80aa91 in / 
# Fri, 03 Sep 2021 01:23:59 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:24:04 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:931337f74a7f142aabe368b4eb63c0e810923f0f0d4f6f018794c6213a4c07ca`  
		Last Modified: Fri, 03 Sep 2021 01:32:30 GMT  
		Size: 55.5 MB (55464641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10ccb2eaea6ac785127af9ff95d34a766c04f17494f30ad1039d1f6aaf912b9`  
		Last Modified: Fri, 03 Sep 2021 01:32:43 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:51a57149e31d961a84a913497727920738ade63c06c982b43d561e46beb1251e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52962829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c85b7584322d1920707f687b8cc50be770820ee8ca92083337902988b26f8194`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:56:19 GMT
ADD file:85473705970b9a2a7e3f503a77360f998648a95f35d8a349a7da9d886eec20ca in / 
# Fri, 03 Sep 2021 00:56:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:56:33 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ee6a9e1e7e2d3980cea17d966eebc0f2d5a7b973da66e550ed3cd517fa38d109`  
		Last Modified: Fri, 03 Sep 2021 01:14:55 GMT  
		Size: 53.0 MB (52962605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea55340efd126bd8d9012e558b39715f8d976db7cd46bf9177ac7dca4dcfd6a`  
		Last Modified: Fri, 03 Sep 2021 01:15:13 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:a6275d14b8928ab53e8e897ab82d1dd44f3322b8e9445ec0beed5406a50e8741
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50611885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22276f2c944fa395f6220abd1070dd4c7f5168832af8574a05e38dabc88e5435`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:05:45 GMT
ADD file:c06a5a30f75111e5744f21bb1d1c0f2edc6668f98d281535c7d6bb5313a18f83 in / 
# Fri, 03 Sep 2021 01:05:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:05:59 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:01e0b96307de81c80d1cf443bd3e569e14bb5ff1c70b7e86acfee257777ebb65`  
		Last Modified: Fri, 03 Sep 2021 01:23:27 GMT  
		Size: 50.6 MB (50611661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7596c6220aaa469abe70dc1f3b97580da7531e12665d4eb892bfeeeaceb2f49a`  
		Last Modified: Fri, 03 Sep 2021 01:23:41 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:f46d04490b827d33002ca64927b4b256c96c1c70c136c450698a1b4739f45325
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54510451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d673c19680697f5ef9fc8fe738fae02e15a52896a7e2a2b04f0b5dcaecb83a5d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:59 GMT
ADD file:024a3f01f7d5ed6ce6f4ee6507a0dbb6edefe3267e1672fb07b5e5eae29a47b7 in / 
# Fri, 03 Sep 2021 00:42:59 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:43:05 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cb1c1f26816daf4a362d7ca0dfd432a0efc976e7a23fda91e6d7940176af45d5`  
		Last Modified: Fri, 03 Sep 2021 00:53:52 GMT  
		Size: 54.5 MB (54510227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e525a9d345743b543c414d10f0bf4bde527e6093b2b4d8d194c456865569bd`  
		Last Modified: Fri, 03 Sep 2021 00:54:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:ffa9fe57ce10ed11bc2ebd4d7935d0d2c289d1c3266e019423886472915eab66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56509054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7ff50254b8066317919b780ce29e3253951264950d89cd066f1b90488c23a64`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:01 GMT
ADD file:9ef35c30c14b19ef5036d3e2bb77ffc3d5b6d271907a910ca2cf862651cf7c0d in / 
# Fri, 03 Sep 2021 00:43:02 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:43:08 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2ab7e270df6d81031d5e7e30c73cbbf82fcf8703513982551504e30e9e0554ad`  
		Last Modified: Fri, 03 Sep 2021 00:53:51 GMT  
		Size: 56.5 MB (56508832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd85e0e6f39ba5b8efb3297ec85300e0d0ac0a5f6122075176604083f7232bb`  
		Last Modified: Fri, 03 Sep 2021 00:54:03 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:4df2d04af916a9105a317938a2f1db72f995616512c9008bf73ea87079348b81
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53802303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd240d9784cebba60fae5e597d3f01324cfe23b72f62fa726f3823fa8b9d2401`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:13:37 GMT
ADD file:8be188e36283a201ba8fee375e57dd8fcff3d866e3e13899d0465f88d5132ef7 in / 
# Fri, 03 Sep 2021 01:13:38 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:13:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:884b720ff0fc8e882637158ecfab27d74351e84a76cb42f2a03b7316b7f7fc30`  
		Last Modified: Fri, 03 Sep 2021 01:24:31 GMT  
		Size: 53.8 MB (53802078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0e3b55124050a2ae0c86d0e2baccfe0fa02b48e0bcdfa47ce830af9fd75e6f`  
		Last Modified: Fri, 03 Sep 2021 01:24:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:a1232e0f9018d02a4c98fcc41df5a4be20b93b39717880d3954d64f3a29f3157
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59526348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e7ddfd942a8e657fc7ef33f6204cf71120e2e12240191f1a568954194805fd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:28:03 GMT
ADD file:3c352e1c5b975bab6ba80213fc86e0b5836f9976e755be58fccd6f003941ca8b in / 
# Fri, 03 Sep 2021 01:28:12 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:28:27 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:61eff2bf557a409d063c940d589dc8f98bf037655ffc94d8e30b546974554826`  
		Last Modified: Fri, 03 Sep 2021 01:47:00 GMT  
		Size: 59.5 MB (59526125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ec6ffebef65179cdc53e188b69336b20b0ca3a75ac0409b5bb40590fceaa77`  
		Last Modified: Fri, 03 Sep 2021 01:47:11 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:912d7fb99de0cc23a4a8aa55d8f2d641cfa0ebd6e468299848180c8aa2cec658
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53749864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5dbffc14b03d8be48d99f12dd62044ed4305cf5a53983965e21ea728e11df56`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 00:47:47 GMT
ADD file:54f05be13650e2f59f5ca102e738802e756fa0f0264cf9f12db6ed40461387c8 in / 
# Fri, 03 Sep 2021 00:47:55 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 00:48:06 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:09142d8bf3fde8b878e8f7bddf00b824e1f1b97647c8d5dbc3df6e87335828e7`  
		Last Modified: Fri, 03 Sep 2021 00:55:37 GMT  
		Size: 53.7 MB (53749639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de841cd4e63835a4344ae5ee88aedbbec5411ee4b527b0260b5274f032d97c69`  
		Last Modified: Fri, 03 Sep 2021 00:55:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
