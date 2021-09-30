## `debian:testing-backports`

```console
$ docker pull debian@sha256:dfe14f043d63f7b63c39119ae6992ccf3f33a97250b1990f510b846e513e4051
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
$ docker pull debian@sha256:5a4a256a53baffe33e7cef3beaa09f008cda7f48c6309a86e01470000bca6661
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.4 MB (55449659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c08e2860a22822ddb1209f56bba6bd7ccb65d99d1aec7148a10b95357ab2f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:43 GMT
ADD file:296666bd4e40daac711ea6d013efc43f7c50e58222b69b3d7116e4f5aa2c9e91 in / 
# Tue, 28 Sep 2021 01:25:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:25:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8cbc26cedebcd0983d6a6ef269bc8a686ef391b21a05f40917e03b8bc050f5f8`  
		Last Modified: Tue, 28 Sep 2021 01:33:13 GMT  
		Size: 55.4 MB (55449438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b7807ebe33e2ed66568cc9e836f24e2f66fb6f464ebc72ca0e162b6c89c3c`  
		Last Modified: Tue, 28 Sep 2021 01:33:22 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:9bcbd805ff5b092f51872c9a5a8a627981f0c53c3c79d5e12dde13b6ae99f78f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52959741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a8cc0ad3ef1ca855e469d40c0cfeb069571cbab3bf6b4ebee824724628ced6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:57:11 GMT
ADD file:b6500095cce7ebcb8cc6dffb6ca25ac6a2a99615c926c3c4460b11d061e9ad31 in / 
# Tue, 28 Sep 2021 01:57:12 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:57:24 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c1065737f43252bb61b016925046a85c465641a80928242342fb59fe79c60e52`  
		Last Modified: Tue, 28 Sep 2021 02:15:34 GMT  
		Size: 53.0 MB (52959517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07c81d26be7ebbb2036f65960ebea77e89282d8863b0563618fe7842db4b605`  
		Last Modified: Tue, 28 Sep 2021 02:15:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:b8c7cca43c21c6f19e0c9e61dd7747ad158201fec59587a5070b76dafeb060dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50562032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f619dc81294996118dd5087473e93d1bda3e06d86163656ecf2cd30fd24c3543`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 30 Sep 2021 18:10:06 GMT
ADD file:60b141079058581933b81f4850d740128aab91ebc4b6e7b633c007840cd17321 in / 
# Thu, 30 Sep 2021 18:10:06 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 18:10:19 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:271f9b3f1ec4b9f851fe5083a6d01887c8fdd9550bbf5eec5a1808d2e9d3dd44`  
		Last Modified: Thu, 30 Sep 2021 18:27:40 GMT  
		Size: 50.6 MB (50561807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b1fe4496452c3a199f28712573a7b1e812a347b1e7a46f879fda9de441c07b`  
		Last Modified: Thu, 30 Sep 2021 18:27:52 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:6d67dbaaccaef817c5cdfee1fd1bfa39e24fa04afbfc9bdc598328401f502c3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54460561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f8a4da5d6413d61156067b03c7d8ed3f1986399c431102e0d4874111f529c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:39 GMT
ADD file:df28df42dbd83dc9e69cbc59efab23a55fd0a6252480edbc355435be4e55acf0 in / 
# Tue, 28 Sep 2021 01:43:40 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:43:45 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5fd04373f6dc4ec57b4af01b70782245fdb26a426888b8d0fe9169590ef679b7`  
		Last Modified: Tue, 28 Sep 2021 01:53:17 GMT  
		Size: 54.5 MB (54460337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55920b702b8f425f498071a3c1b23346e3c518d14e64364ee85c3c9672039eeb`  
		Last Modified: Tue, 28 Sep 2021 01:53:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:208bd9043ea32cdc0f28d565b8a301fc7f070425a4bfef7da8184d1a8e3b4414
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56469906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1994d7edd2bc6fdb35361fe2ef4871bae71cab6c2cf04feb740f1f4ccc66d736`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:56 GMT
ADD file:171aa2f7b9b807824f9dcff0b5370aeaff51005a4db0442a0d922f0dc072a65f in / 
# Tue, 28 Sep 2021 01:43:57 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:44:03 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5c99d92b251c23b8fe8d936e0795897504e195d64c189239c7173c44ef899177`  
		Last Modified: Tue, 28 Sep 2021 01:54:32 GMT  
		Size: 56.5 MB (56469685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c22a4d6f68e6cde0443e6208d901fab48ae65f2836d31352ab4a2c168ceb5ea`  
		Last Modified: Tue, 28 Sep 2021 01:54:43 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:8264c57b6bd987e009a139c0622f8408e2b9cb7f53d9b15944627a5d0959a2f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54053875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95755ae7411d79d9193120e9ab08610c3d5f6b158cbd659b3f1ac268a2a84ea8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 02:15:23 GMT
ADD file:30eff74ae8209fcafe4713d1789a499c6a35ae6014467ce2b7991f21518d7bba in / 
# Tue, 28 Sep 2021 02:15:25 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:34 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e0693c7024fe468a992c81ade579d76ce386144ac09a4020ea13c0b9e532047e`  
		Last Modified: Tue, 28 Sep 2021 02:26:36 GMT  
		Size: 54.1 MB (54053651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9e65020ccc8fcb6903f7c8264e54eb9cd57e2473ea8218fea2c2d80d581922`  
		Last Modified: Tue, 28 Sep 2021 02:26:47 GMT  
		Size: 224.0 B  
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
$ docker pull debian@sha256:4a870c175e3045329b7defde8b9a20fd756385e2c5daed278b2400baac5928ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53691234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40bd3d160a45dded1d93e36a19e7d76df7ca95cd9088d5035bebb967ad07e1fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 28 Sep 2021 01:45:08 GMT
ADD file:094728d97cbb14c94edb377e3d4dede62bd88e82f98ecd93bba64aebc4e7916a in / 
# Tue, 28 Sep 2021 01:45:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:45:17 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:93e4733dccf8c066cccad1642f393ff63777ee8c1262cdbc961912a70203c3cb`  
		Last Modified: Tue, 28 Sep 2021 01:51:12 GMT  
		Size: 53.7 MB (53691013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8eb792ace35fc667cd159721cc46ea4111f9a05f2fcdb64874084104bc9875`  
		Last Modified: Tue, 28 Sep 2021 01:51:19 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
