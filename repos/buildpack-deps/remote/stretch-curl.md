## `buildpack-deps:stretch-curl`

```console
$ docker pull buildpack-deps@sha256:f89d39f2ab3bcd7b2fcec3e16f7560eab574e9df215f618950f282cf03f4395e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:stretch-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d570e283cb8b21d14f166abad0f696f5552d80568eb74f3461726b46c232e9fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.5 MB (60513583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:338f623ad59df54ed78b4841b118338c270a103ce95a3eccc8c563f3b337e0de`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:23:35 GMT
ADD file:82e0eb87c6ff97b66f86c9fee44884c4cf1b08f5721f36878fc7a15a125b5079 in / 
# Wed, 13 May 2020 21:23:35 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:39:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:39:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e6ce7b04634a37b5c20274b3cc1469490cb28f734448d2c84d01454465418e1f`  
		Last Modified: Wed, 13 May 2020 21:29:57 GMT  
		Size: 45.4 MB (45375936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99828f061d94e903ecb427fa486d6f5876932a98b7bbe2dbeaf26d1b7a4d52c`  
		Last Modified: Wed, 13 May 2020 22:48:42 GMT  
		Size: 10.8 MB (10797470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c850eee83158cd6c3f9a0c3a52202356cce4782a6c3e17f69786722711814e11`  
		Last Modified: Wed, 13 May 2020 22:48:41 GMT  
		Size: 4.3 MB (4340177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:4e929f0c0fa5c6d6ebbbae3ea8c57f0974682557eee4d7d2fc66e1126a6045e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.1 MB (58097883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abcd1aac93d351bdba480932c24904e202136f9235c1a6c66881806ad4362e10`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:42:21 GMT
ADD file:57aa6b37e4a65a6ce77d5943dfa67cd85ae4b6c145f9d2baa87ee4e569a77100 in / 
# Thu, 14 May 2020 22:42:22 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:55:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:55:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:910ef58b27ef80c5e71df714f5f3d3c8d01b34e7e567691809a33f51d01953c1`  
		Last Modified: Thu, 14 May 2020 22:50:41 GMT  
		Size: 44.1 MB (44071876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d73f59cb15fb4026e8f0dfa7ec1d84fa68e890cf1efc97d809bef79936bb00`  
		Last Modified: Fri, 15 May 2020 04:05:19 GMT  
		Size: 9.9 MB (9866834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b13f5d90742a12b6750a0920980bd0267791366745eca3ba7f181448c922a5`  
		Last Modified: Fri, 15 May 2020 04:05:18 GMT  
		Size: 4.2 MB (4159173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4b5fd869ffd56796fb2df488b11531b6adbb4620ad1a8dc157fa3a92b86eaa5a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55518250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:695b83cdd4d37f886dd5f08b7f7b8a127c5af76559b51523c3aece97878015cb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:18:55 GMT
ADD file:22401e33698b1bb830736dfb4dcfcae97faee4aeb57fbc910c50a0806fb726e3 in / 
# Wed, 13 May 2020 21:18:57 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:11:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:11:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6d01aee5144e594ba9bd007624dc3b8437510d15e6c34689c8475bf2d6b5c3e4`  
		Last Modified: Wed, 13 May 2020 21:28:12 GMT  
		Size: 42.1 MB (42101107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe054c42f454952057587a2811701e4d75d2373543ff044e7bb2ac01b58b9ea`  
		Last Modified: Thu, 14 May 2020 00:24:33 GMT  
		Size: 9.5 MB (9498400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c387dfbcc5dd736b7a3ff0e096644f3893be259a4dec30a1309d0374383da2c`  
		Last Modified: Thu, 14 May 2020 00:24:31 GMT  
		Size: 3.9 MB (3918743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:eeb2abde388c1344e896a5dd11dfbf56d86c5531a37c17a8067b770bc557bf72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (57001895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ce6b600f6a94ded440d19037ead0d59b0248a7b1e272d7f910654975c69763`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:47:38 GMT
ADD file:e7776aac0b87be303e31e5947db89f835a4e17175e339ec23becf5fe4a9548a5 in / 
# Wed, 13 May 2020 21:47:41 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:32:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:32:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0480c895dd1d5b237cb931426f18706cbe8dac16e19ed583f3010f3655094efa`  
		Last Modified: Wed, 13 May 2020 21:56:03 GMT  
		Size: 43.2 MB (43158976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13cf6474b5cce4b1c7c8d54d2c80e8db074f4c5d89471a009859e0c318ac7d76`  
		Last Modified: Wed, 13 May 2020 22:42:35 GMT  
		Size: 9.7 MB (9748540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f97c7d6d20cb6dbf105d3e25bea385e4b74876e9fcd4cbd49ac0e5b30c69c80`  
		Last Modified: Wed, 13 May 2020 22:42:34 GMT  
		Size: 4.1 MB (4094379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0ff130061e6293179a32572909fd6a2c18586433e56e59ebd167460248585d10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61474941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d64e6949caa75b6f57d7776d01cc0e550df07f901b848602f39561a5161aa697`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:23 GMT
ADD file:0d501ab6846646b4793ce31bd08a81ee75bf7ca50e44fad4f41d38ea73217f94 in / 
# Wed, 13 May 2020 21:42:23 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:56:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:56:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:738ccd27fcd21d91d1826e5bb5ee29ef3a82a770de7e1407c86b04395fdd1335`  
		Last Modified: Wed, 13 May 2020 21:49:47 GMT  
		Size: 46.1 MB (46095041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82205e09585e2a065853d934b8b472473745ad9b5efb22d99c6058389714f39b`  
		Last Modified: Thu, 14 May 2020 00:06:36 GMT  
		Size: 10.8 MB (10818400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3797adb63c6052aa7506f3676edbac22d3e2c0f54ee7d52a3d9457de30b41e4`  
		Last Modified: Thu, 14 May 2020 00:06:34 GMT  
		Size: 4.6 MB (4561500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3c39e4ab0598b78f7eb7bddeaa2d8cc9009139e8ede276108f46a588679b35e5
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59269938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676268978b3233953cc8a3b20d1cf683be3a7efef1a92479027e6eddb9a826bd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:52:06 GMT
ADD file:7bf5ef3df2c7fedfe3177de091f107679e7882507d08882b3203eff7ac42da5b in / 
# Wed, 13 May 2020 22:52:07 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:05:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:06:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:690bb78d0f5d6a469cf42f228761b11696fe51dbcca8ec4392ae892677a415b6`  
		Last Modified: Wed, 13 May 2020 23:02:33 GMT  
		Size: 45.0 MB (45048775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7defc0f982fc7a60239b6792c0bae2cf47b26cdf0863043492bbba235b9f0035`  
		Last Modified: Thu, 14 May 2020 00:23:25 GMT  
		Size: 9.8 MB (9826324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f70cc1cb7d757de66211d78d4b389425f5ae180b0ccea6f03fecbdea3dd5619`  
		Last Modified: Thu, 14 May 2020 00:23:21 GMT  
		Size: 4.4 MB (4394839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3fb7b8b58ae399eea52e95f977bb533c26f0240688bf003bff2e6e0742418eee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59945431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d8f952ed92131f951435b33212f6ee48b72742952207c4313b4e3388985ba8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:39:29 GMT
ADD file:fa4c7e3ca04f092e53cc791a32c929663412df3f68de2733bb867053577bf1d1 in / 
# Wed, 13 May 2020 22:39:34 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:7732483b686efe14a1cf8add89a1568b83892e243798fba30808f1fc6287210b`  
		Last Modified: Wed, 13 May 2020 23:02:10 GMT  
		Size: 45.6 MB (45646193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df33ef5c6dd4781defd528815174987b67a617a4fbddd5e5241a2f67a34098cb`  
		Last Modified: Thu, 14 May 2020 00:37:47 GMT  
		Size: 10.0 MB (10002565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02507bd450f72bbb529f56f9579bb7169fc9be7900bc5b9b0587e4855e51ad8d`  
		Last Modified: Thu, 14 May 2020 00:37:41 GMT  
		Size: 4.3 MB (4296673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9f25ea9ae64c887c2de2fb4b821e10c386bc4c79acb6e259379b4be1eb2c25d3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59930543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b936cb20f9370245f9befe4395c21e90f198af60e06b488fb75639cd0b66ee8a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:08:23 GMT
ADD file:32ad2f356c0ec407aa31085089417aaa9f72a5dc2757ed68a0adf7a432e4bdaa in / 
# Thu, 14 May 2020 23:08:26 GMT
CMD ["bash"]
# Fri, 15 May 2020 05:03:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:04:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dc69489da20ae5bdf6cefc772e7ff8420ffbd2c920a57165de6ead66d1a997e4`  
		Last Modified: Thu, 14 May 2020 23:12:48 GMT  
		Size: 45.2 MB (45232081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe5c3a82fe7eb310483d893dd90a653f2b29688e70bb3a0000e8c208de755b`  
		Last Modified: Fri, 15 May 2020 05:10:26 GMT  
		Size: 10.3 MB (10325875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757a1c09293f132a58fe2f774191e2545fd945ba597ec8d9a399751180aeeb2`  
		Last Modified: Fri, 15 May 2020 05:10:25 GMT  
		Size: 4.4 MB (4372587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
