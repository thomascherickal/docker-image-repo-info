## `debian:testing-backports`

```console
$ docker pull debian@sha256:ac7a74aecbc8bd13ef7034930697c94504ca687bdef49449a8a433c620a33a4a
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
$ docker pull debian@sha256:064e2d5dfe6f0783de35e18471f1fbf425dc80278f6a4e451ce991921ae688dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49043231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:264feadf4da6aacf7ad28f3cd18f1e0d64e1aa248f0456f99c5f11699c191bd3`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:53:33 GMT
ADD file:6d6719e60ccbf39132571a488cbe5e0237079ef5a236fda3a19dc7343fc34bac in / 
# Sat, 04 Feb 2023 06:53:34 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:53:37 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:57bcb44855e036a00082b63104a953f2e7172588e397422fc4db80abde25ed1a`  
		Last Modified: Sat, 04 Feb 2023 06:58:51 GMT  
		Size: 49.0 MB (49043008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d6ce2ee33c0cadabecc3b34ae52e8d47ca3dd23034884eb4d86595a8d75ed6`  
		Last Modified: Sat, 04 Feb 2023 06:59:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:4002f41284247f9c64990bcd89fc0ff034b73e63a931c9ab5535364f19387983
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47993471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7220ce7b48adcb510cffe423a1e94797ff3059a41a38c6aa8c82c458ff303f86`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:47:39 GMT
ADD file:98e47e6350976474e8c5ce450917a12c04e080ced6ab05eed9e04772c5728570 in / 
# Sat, 04 Feb 2023 02:47:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 02:47:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:01cdab3e0a4d64aa88c8c65852e4599d329659e9aa85a26d1ae3f1565db6ea9b`  
		Last Modified: Sat, 04 Feb 2023 02:53:31 GMT  
		Size: 48.0 MB (47993248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e542969ffccee238f8d18194c3c32fa7352b532da45e6ce9624db3718aa7a1b`  
		Last Modified: Sat, 04 Feb 2023 02:53:42 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:29f598bbe94f6e034e46ebde69e3e34e0e931cf823799d39c9003b04bbd34006
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45794386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ca5f5e81ef4843f17510606fbd2e976af3968276758fd0785d66216fb34303d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 10:01:46 GMT
ADD file:0a9c474422e8c0f119b0473bd550098fa14ececd6f4e1ebecb0519057ee3949c in / 
# Sat, 04 Feb 2023 10:01:47 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:01:53 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4acd2d529567dfe96a5a0e4495609a52502ee02aa4ee77b1c33f6157e5f09282`  
		Last Modified: Sat, 04 Feb 2023 10:09:37 GMT  
		Size: 45.8 MB (45794161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad901c40241e7172194a257a7e1243d004fb4aabf530377824687aecb68863e3`  
		Last Modified: Sat, 04 Feb 2023 10:09:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:0bb16314a25ac70de6123f70d3bec337e0cfaa28a4ff12aa64af016bdfa4de64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49081711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed9144778871673a506f483281b74ee61c255f41201c50723a17e9a05ba3a84`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:54 GMT
ADD file:45f2f09495aef8ab54f81db15f593e777fb18880028f3099dd77707a143d2acf in / 
# Sat, 04 Feb 2023 06:18:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:18:58 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d4637841f1417b168a5fcf6ae681705a2726c9ab1178d66fd4b8659b70a858fc`  
		Last Modified: Sat, 04 Feb 2023 06:23:53 GMT  
		Size: 49.1 MB (49081488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b96d3246d7bdd329a2aa74ab010e483380b9db0dc008acb940423693c77165`  
		Last Modified: Sat, 04 Feb 2023 06:24:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:4f8887f629002e963ec510c8b1ed08392464dde3bb09448ee448e44f61fc4931
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50093648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d63cde2419dd8434c5743e075934069eec42b3eebed67bf173ba32f0c518e346`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:51:12 GMT
ADD file:ad17cd9a85b389575f6b3289675831e1173edaf33986260823441a61f1c904ce in / 
# Sat, 04 Feb 2023 07:51:13 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:51:18 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:661528ae13ac034793f44e59402c02c52f6728f6df010da9e53b93360a821eb8`  
		Last Modified: Sat, 04 Feb 2023 07:58:02 GMT  
		Size: 50.1 MB (50093425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3fafc776e44bfcb3358bd3606e29200dfd77a4154935206a369d0466d7ad69`  
		Last Modified: Sat, 04 Feb 2023 07:58:13 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:54e79cb1c049d1763aa1ba0dad14497e88f1b7733089cda4dd82ee9f2f1b63c9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49041164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60706f6904c91bc4fd5cb15315cf5b68de64eae5c778402d3d009a8dbfa7b0f9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:23:07 GMT
ADD file:a86d10831e490fd95df396c6c88db321817821efd0ff2e0866d6b5ddb1d0ee83 in / 
# Sat, 04 Feb 2023 06:23:13 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:23:22 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2663b89decf1b05f44b3c11d351ce9289c713772abddcb4215d45bed522886c7`  
		Last Modified: Sat, 04 Feb 2023 06:31:41 GMT  
		Size: 49.0 MB (49040938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5665f25f850928400c2438a167c360f579839fb967ebabbcac0beb70e4213a`  
		Last Modified: Sat, 04 Feb 2023 06:31:51 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:798e279ae4790690ad545242f2831de9ea3482cced1a2ad3bf77d714504eab8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53066789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d9e1f3d32726a50c6679337155203854705bcf1d31170c7a90e2592e8e529a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:27:38 GMT
ADD file:6a8cc39d059a87a9be2271282490dff13195c22926b3dd5458cd80a387fe6f53 in / 
# Sat, 04 Feb 2023 12:27:40 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:27:48 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:62e04a70589e68af436acb6cbbc46421df8df67fd86623b045e1f16d4b3c285a`  
		Last Modified: Sat, 04 Feb 2023 12:34:14 GMT  
		Size: 53.1 MB (53066566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1e27f8bdd0ef89d5a0a53d06cc7b41b17f4eea83cec5eff63f277e9a797a8a`  
		Last Modified: Sat, 04 Feb 2023 12:34:25 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:8b316db32eb51d8b035aa9631cd8edd51421637daaf4e1dfde84019d4505df23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47429925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739da72d284bb05e62815eb38fa84fa807a5edbb7005a9ce9a2379822d1ca096`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:07:20 GMT
ADD file:bc5ff0fc30abad7ccd04b372b80a22ffd8fabd60c0b4ddfa367dc841415fbc8e in / 
# Sat, 04 Feb 2023 04:07:24 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:07:30 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b0d4d83e89902e21b3d9b4ff69c9a54c6af1968d9820327767ffd6c6f44e07dd`  
		Last Modified: Sat, 04 Feb 2023 04:11:30 GMT  
		Size: 47.4 MB (47429701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b77f205684f5ea27f72fab73a22d60fdd4edf9300ffc6d5a5f788b07e3e2400`  
		Last Modified: Sat, 04 Feb 2023 04:11:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
