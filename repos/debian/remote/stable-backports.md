## `debian:stable-backports`

```console
$ docker pull debian@sha256:e9c8a59f9db53fdd818189860e22d80bc950eb91375c74cd9d5f7310d8b4239a
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
$ docker pull debian@sha256:a9a79fbfae1729ada9d52bd5dfb0f8e4e29449e29b27bd26c20ed57fc7c5c56a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55007780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d444c22564565736c6ad1dee5b14c7e5df8ae90481dd745d28f12f8cbc2c4456`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:57 GMT
ADD file:44c550a883e90ed6f9256847f2e0b7d03dfa87361c0c0256d3f7eb40580d78c7 in / 
# Tue, 23 Aug 2022 00:21:57 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:22:00 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0b5aea898977d2f7786116d9cb106042377e6221d2552a75ded2f040beb2c24d`  
		Last Modified: Tue, 23 Aug 2022 00:27:11 GMT  
		Size: 55.0 MB (55007556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4293a17c1b49faa7fbc0c8d2e57b39228458076fce2cc2a85f795a527ff8d46f`  
		Last Modified: Tue, 23 Aug 2022 00:27:20 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:2e4e375e31a42409c92e721bc246e9d35a7fc15b9d79151134a8be61e580a91b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52537545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:213c1994138af7cee17fa73022a49f3797038f8162f5a287c8543d3fb750f22e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:50:49 GMT
ADD file:52a6d8229e5ac4dfbb34fe2fb2d592f5568d94577af32ea2f582a7572230cfa0 in / 
# Tue, 02 Aug 2022 00:50:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:50:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bbfa844297afdb04b2d19f686b44257db9d439144828f7cbe63079baa3aff5d3`  
		Last Modified: Tue, 02 Aug 2022 00:59:27 GMT  
		Size: 52.5 MB (52537323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c52e50f26309d44f22c4fa41c3f3dcd0aa0ca0a8d9884e8f1afd413e7ab8ab6`  
		Last Modified: Tue, 02 Aug 2022 00:59:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b18d85fcd3192773f6e7df5598a29a5d50a54fb1e1efd43e0fe2a37b1d9a6d00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50195528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6836a1f6ff0da6511ed459ca2ef4787256dee00385b4a464448d1d07bfeb4137`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:01:18 GMT
ADD file:87779f497c3b9ebf91ec2cf311358f76f20eb515ed6b183da52c14088803fc85 in / 
# Tue, 02 Aug 2022 01:01:19 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:01:26 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:08a6bdc1003bf2bd374f4295cb01d1755444f3bd214e75a8369e8e11001cd2c5`  
		Last Modified: Tue, 02 Aug 2022 01:09:46 GMT  
		Size: 50.2 MB (50195306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725e760ab7589c6e9d7d3d54893d6f241831c1e4b4a016b35aa93f2a3f27e42e`  
		Last Modified: Tue, 02 Aug 2022 01:09:58 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:d4f698df794761cbc51e118cf85d98724b23785358a6cae144477f456320d8fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53683259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d68f06b7578157852aed9d7767eb15399c2b2acaee4e885416d5012ba3ea934`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:56 GMT
ADD file:e9e1a80abdd9e28b7a7279be8f171672f11c4eef9f8303a5afed5035269f2a6f in / 
# Tue, 02 Aug 2022 00:41:57 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:42:03 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1d90322913db8b41c2e5aad681509b79eaa89aae0f4060e6101919637809ab74`  
		Last Modified: Tue, 02 Aug 2022 00:48:33 GMT  
		Size: 53.7 MB (53683037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367372a44d75671088f9d16b72e1caf3331192d151be18d11b992993de2ed190`  
		Last Modified: Tue, 02 Aug 2022 00:48:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:429cc1726a0800b1c14a32501d5e3018b5469c2b2f49a3f1f0065f47ad664996
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56002396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1ed227dfc6b371caa03482930d045aaf1e8bd307f4971d0a7d2654d8da816c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:44 GMT
ADD file:9852bd11f2ac634027eacf67314290b88218522fc900a95a2c67c3ba1943dca2 in / 
# Tue, 02 Aug 2022 00:40:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:40:50 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1c092776bb568ebc5f3310d657622e6b172affb770546c2ce1246cec19563507`  
		Last Modified: Tue, 02 Aug 2022 00:47:54 GMT  
		Size: 56.0 MB (56002171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8be317792d3f17016bda83410372f413836b952924b159dc886cb8850c437ab`  
		Last Modified: Tue, 02 Aug 2022 00:48:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:18a313441151e284921b989423c23549c7392422ceb9575fe2e137ec8632b00f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53273243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2285b7b159e6be701f33d3da71a027868c38b059f65b264ad12a622702b239e8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:12:57 GMT
ADD file:f111219fa55c5df38672bb7b42040526beb6baca250e4ad4ee724c1a9090f961 in / 
# Tue, 23 Aug 2022 00:13:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:13:17 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d3836c0ff2a3ebbcf11d16fdfef0948db59cc812e579ab311b2e3b198b373427`  
		Last Modified: Tue, 23 Aug 2022 00:21:30 GMT  
		Size: 53.3 MB (53273019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93507289598b4214668e787ef501a02c71d8721717fcfc4b2ae725fcf4a8af93`  
		Last Modified: Tue, 23 Aug 2022 00:21:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:32634886b21b75f0bada3dadd657646cc102d5cbda57e285cd560f6be1e0af5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58896173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744d784ed67d5e6881e4ae80ec34759431857b54fe9435d798ab39d8aec13151`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:20 GMT
ADD file:e3c8c0436300537d941b66793138c25729cb08ad4c31b728fbd38204d1c6b787 in / 
# Tue, 02 Aug 2022 01:19:23 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:19:29 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f3d36ae67ac28ba83123a92acae9b3bb36513bc227660b2cd1dfef688fb3818e`  
		Last Modified: Tue, 02 Aug 2022 01:27:55 GMT  
		Size: 58.9 MB (58895950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e5bbd93ee2751acc1b7a42908ca8f4bc59a2d18d0e967b37d8b0b6bf18cc35`  
		Last Modified: Tue, 02 Aug 2022 01:28:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:bf51516b157c351f2311fc080c35b79ae9ea110b37c083734f4ba6db7d08a2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53269505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab285031ddee2b28a86a00262b92845d01c6282d10c58d85fcd5bab5d8559a58`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:43:58 GMT
ADD file:b8eb179ea4633930d534f97a4492919ef0f04b76e64638ca420126e8e6c283de in / 
# Tue, 02 Aug 2022 00:44:01 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 00:44:07 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:138917c3beea79078118bf931fd764018dee33be43999326d009971680156b4d`  
		Last Modified: Tue, 02 Aug 2022 00:50:22 GMT  
		Size: 53.3 MB (53269283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b38b88b13451f9c034d20a094c4cdea475275588c4e057fd7bf3ca5578cd70`  
		Last Modified: Tue, 02 Aug 2022 00:50:30 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
