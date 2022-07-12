## `debian:testing-backports`

```console
$ docker pull debian@sha256:716fcad52df89fe72121a76deed3865d98ef17ce6a5b6cb9aa96a02379d21ca0
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
$ docker pull debian@sha256:d3529295b4a93fc688e56891f209be9dd054e15239f21996a0ad546654fc59e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53022542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9306f3112609fd2cb1be7071511c2c1c32becb3ffe41a50669c7e7ddb65f90cb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:21:51 GMT
ADD file:242a7253146210771956ed1bda9124125835ad9e76a50d745d06b34fbf5e50df in / 
# Tue, 12 Jul 2022 01:21:51 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:21:55 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:df98203a8b21cb36e308dd353908ed338642491ef167d757bebb3297146a77a4`  
		Last Modified: Tue, 12 Jul 2022 01:27:27 GMT  
		Size: 53.0 MB (53022316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f55606a532f98e4de0863bf1b4c84621d9149609bc2c7df29a52d5ce2c81109`  
		Last Modified: Tue, 12 Jul 2022 01:27:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:153f6ded171d49ffd6e9d0e2ba13af934fcf48b5ab80b309d610e5443b25fa37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50821791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a259877548c2c206b96197d1907323ec77115d1d09d300a1342a049d35a5d04c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:54:53 GMT
ADD file:c6179c8aec0b762efe1793ad6195ffc725215a2119b032d1083c0519745e2b08 in / 
# Tue, 12 Jul 2022 00:54:55 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:55:08 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f83dfb1f058c2677da0ae8544263be98b5478b5809f125d62cde7b5b1b4dd644`  
		Last Modified: Tue, 12 Jul 2022 01:09:10 GMT  
		Size: 50.8 MB (50821566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9443e5d4b71b078269476c3aa045dbe1c30aa0b2d5014a08b6e72ac86f64f232`  
		Last Modified: Tue, 12 Jul 2022 01:09:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:61e03093173ba0f8bd93e9176ed916b30e2ca2d3ca01225c9c45b43bb4ad8ebe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48563083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad78e302f619b9574fe128b82e76283b22727af6fc6e4588758682c43b733a26`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:04:32 GMT
ADD file:317db84b28908021f136a605aaf69b42d1725ce731379ed14edf6efd1decd2f2 in / 
# Tue, 12 Jul 2022 01:04:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:04:46 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a8ecd9f0722e6e2cb75e6bd25459933c3f38176d6141c92acce638f018231c76`  
		Last Modified: Tue, 12 Jul 2022 01:18:13 GMT  
		Size: 48.6 MB (48562862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ab19c2dd4d53afad3740a1a6c3d27ceef8f8f6c959fa276c459f0be5426607`  
		Last Modified: Tue, 12 Jul 2022 01:18:25 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:ef5fc77d03219497588bd63cffb032567804922e6857167f8d26e75a1593f4e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52128852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68fec8e0cfa072c5c027914a9c043d33014f000c9f89708e213cf15779d6169a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:42:26 GMT
ADD file:52b0a411bbddbc5a40d2288e5189606bd2fb03bdba9ab2dfa0b29ee90195a43b in / 
# Tue, 12 Jul 2022 00:42:26 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:42:32 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:370af700e1ed84d7809745357ae1357e57448bf6e682ad1ff1a41f20c19fe232`  
		Last Modified: Tue, 12 Jul 2022 00:49:31 GMT  
		Size: 52.1 MB (52128630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6029c6655172b28d7933cba26bc204e2f8553098c11e8ef26a605b7e620f937`  
		Last Modified: Tue, 12 Jul 2022 00:49:43 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:fa335b6c78cdaee9fdd4fc3076d9bb392f4ac0e5e47998e5155749d1dc806aab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (54004242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd898a178c006df4e0a2d6886db385c530ef172aa37faa86b9e3c200018e3e8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:19 GMT
ADD file:044345c3015d2fe1cae3b8a12314680146d341abe9874bd58fdcbc1589642c13 in / 
# Tue, 12 Jul 2022 00:41:19 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:41:25 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e40b58f267b2fc10cacd56d0f087127ea8b9dde1c3708ff2b4f4650a5ed2d08a`  
		Last Modified: Tue, 12 Jul 2022 00:48:38 GMT  
		Size: 54.0 MB (54004020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d8a37281c18e3d31e1221661b8b496c03dd550e4e93b66c80cbfaecb5f3a76`  
		Last Modified: Tue, 12 Jul 2022 00:48:49 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:e04d3d76cefa9894eeb7fd9c5ec992db6ba7cac086ddcbd78c55d0130e3b9aee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52148484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0c4dce7b040f3a8faeec2113652dfda1d57ba5de17bb92ad8af315618d7e693`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:46:23 GMT
ADD file:cafc20a19b7a947f5cebaa2e04c5fa4dc96b0580d9a70a92068aaed8a19ed722 in / 
# Tue, 12 Jul 2022 04:46:28 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:46:38 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:311579db3109ad3829a7cc600da26fe8f56d9ed46e904060a08b655b56a8a2d6`  
		Last Modified: Tue, 12 Jul 2022 04:57:22 GMT  
		Size: 52.1 MB (52148259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270387476bb72e24b888e96bec6b0501477db1a1856b866091c97de47163f093`  
		Last Modified: Tue, 12 Jul 2022 04:57:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:1fabba15fbafdd0458418059d64c7f6b6b2b7957e40e8f8e19fa40785c398e5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57237826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309a1a57b178af283a61ee2399a9a988cc47e84a9d0823de5e9d2874315a9314`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:29:05 GMT
ADD file:50749df5dfe83d67bf06b74c10d8d4c0b6c50902fb0b3fd4b1e944bb4d04d838 in / 
# Tue, 12 Jul 2022 01:29:12 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:29:27 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0a914d717e21264ea59989c5b8ee06609e61159738242df44dc331a1146b94b4`  
		Last Modified: Tue, 12 Jul 2022 01:43:45 GMT  
		Size: 57.2 MB (57237602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78e09d38971941c3b2dee93582be52ac3ec39c79eafc1946be46d8bf478b917`  
		Last Modified: Tue, 12 Jul 2022 01:43:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:215d881beefb93b2aa019b733b1faaf76f6ebb1720b9e801461184c846467946
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51554349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:663cbbd57a0d7a95aa3fd14fd6367aeeac1959f24b599080ee768798c9503487`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:48:02 GMT
ADD file:d73eeeaa444d7c8255cd2ca31c00a952231237fc5487b1e6772c5f70cafd440a in / 
# Tue, 12 Jul 2022 00:48:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 00:48:18 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:80dbf564ccdb8d822debfb926a7eaccbc64bd2365e4541f63e07fdf1295dd5f1`  
		Last Modified: Tue, 12 Jul 2022 00:56:09 GMT  
		Size: 51.6 MB (51554124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c3d2a0890f66ceefb89fd3d66a144187e7641f7d47fdfd95e251762fd76466`  
		Last Modified: Tue, 12 Jul 2022 00:56:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
