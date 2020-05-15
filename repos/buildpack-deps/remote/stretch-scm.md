## `buildpack-deps:stretch-scm`

```console
$ docker pull buildpack-deps@sha256:f72758194f4339c90a44d015dd998920ce280845f7946a7f50e2eaafcd42a01f
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

### `buildpack-deps:stretch-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:96809c4d1c9582324d84928df630808d6e9736ef29e2bebdd3f5bfea934e3006
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110597019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb8d5201270644ad6b42d93a2e95c018fe85453f994e20545c11895bd72ac07`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:43:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:44:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194b0e3c928807cfabf081055a117585ba5bf6697f65b2fede02225a5d73ad2`  
		Last Modified: Fri, 15 May 2020 17:55:27 GMT  
		Size: 10.8 MB (10797475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec00f35d5b2d1db6b8e925a3005c1a285365775028db0339903ddaeec4763`  
		Last Modified: Fri, 15 May 2020 17:55:29 GMT  
		Size: 4.3 MB (4340139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b1353672b6861da5f1b58b0eca02ec10373a25d2898bddafa1b4bae2271c55`  
		Last Modified: Fri, 15 May 2020 17:55:45 GMT  
		Size: 50.1 MB (50084198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:305d033c8650220e790f06a38ea39e5290d2025ad74887a5f22b033d249c93fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.4 MB (106403385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f989c879d602e5cc73cbd1ff87ce3ab147205c1e9593f6aa54274cf4fa2ab83c`
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
# Fri, 15 May 2020 03:56:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a71f712ec61e8aa09dc3513aa80387eb70dcfd98f801033695a428bb6011f27f`  
		Last Modified: Fri, 15 May 2020 04:05:46 GMT  
		Size: 48.3 MB (48305502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:42aab913af2d0e6c185e11e534e4178a95e6554592a43035bbc8e2310d694981
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101934713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2793efb404729b60c95a4ce789778b52a4d4abf35456d2a8287748609b0bc3d8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:06:22 GMT
ADD file:89db8453485648b09e63411b6e2ad84f08844ee55cb115e59cdc8c8cb1c29a1f in / 
# Fri, 15 May 2020 01:06:23 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:49:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 10:49:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11acdea2de14253903f5970d63a2076ff08912929430d1c33afe617c9fa6bf8f`  
		Last Modified: Fri, 15 May 2020 01:14:46 GMT  
		Size: 42.1 MB (42104346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99452f66748f5df5d89d2287e42b5c3d87c9d5e1e20c16ef729e87d463840cf7`  
		Last Modified: Fri, 15 May 2020 11:01:44 GMT  
		Size: 9.5 MB (9498344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cef06b7abe4487657829b47c97bd2992f14a34349e0bcf60a47de9c647bd3fb`  
		Last Modified: Fri, 15 May 2020 11:01:43 GMT  
		Size: 3.9 MB (3918713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c542e1b5d6ef8c44b0708c5d2d73da1f5269186501aaee2b172d32a8b50d86c1`  
		Last Modified: Fri, 15 May 2020 11:02:04 GMT  
		Size: 46.4 MB (46413310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d2d5efbe95b78462edec381abcd34718665cf8d7617945e28da481e457709f54
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105036255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368aee20debdb765a73bfab3a928e9f8a09a0a4ae0f0da87a88c02a09dbaa0dc`
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
# Wed, 13 May 2020 22:33:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:3166282442cd611f517b83932715119560eac9ad53b1356b6377568687f87a2a`  
		Last Modified: Wed, 13 May 2020 22:42:58 GMT  
		Size: 48.0 MB (48034360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8b54832c0ea7e6ee213de19f498a29612b94e971585fd99436419287cc49ef59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113090953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d74b785669254b943ff9bfdcf9f09479edf4145e399df1728f7712578a0aedd8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 07:12:19 GMT
ADD file:22284e8c6e684308a95b18c7ed63ef235582dbb1890d1d02c22213e41ae47192 in / 
# Fri, 15 May 2020 07:12:19 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:22:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:22:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:22:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddf311fc69760572da5334a35e5a0e9fa15690ee1e40ed4b06e9a65213bc7223`  
		Last Modified: Fri, 15 May 2020 07:22:51 GMT  
		Size: 46.1 MB (46094205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b241dd4b1f1a808fb80049baea941ffeb595af14983b6e48560fc4d07b66cf54`  
		Last Modified: Fri, 15 May 2020 17:32:39 GMT  
		Size: 10.8 MB (10818399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a58f9666641b58144531065f83cb2bf8ae4fc7968332d0563612de804752c0`  
		Last Modified: Fri, 15 May 2020 17:32:36 GMT  
		Size: 4.6 MB (4561476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a5af2e44b2e93a8556c765c57f7a929c2e24ace22880ce91c76ebbdee145d4`  
		Last Modified: Fri, 15 May 2020 17:33:00 GMT  
		Size: 51.6 MB (51616873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5deb214b24126ac811d610669924af6ad0f0efe1c704567c5199483f5d8eb944
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.7 MB (108746804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab5687303460bff0222871cb5d466a74f9cc9a57a0e0d758870f880de8bc3507`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:51:29 GMT
ADD file:5610fb3daded60b4edbeb9eee1de6844d7fc8f0e0c16bf0b52b103c049a0b35b in / 
# Fri, 15 May 2020 04:51:30 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:46:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:46:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 14:47:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93c302869e1cf6b947e854056b6eaa233f67b16066dcefb9c1af21d3427abb7e`  
		Last Modified: Fri, 15 May 2020 05:01:51 GMT  
		Size: 45.0 MB (45049851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779973970282cd32b24e4aa9a133357e3723fd22dc2a3fd1dc392353a69693fd`  
		Last Modified: Fri, 15 May 2020 14:59:01 GMT  
		Size: 9.8 MB (9826383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e84f102e0a7201b95c7c46f30d1b0636f08785711c13ca56452e7b4b0d32f06`  
		Last Modified: Fri, 15 May 2020 14:58:56 GMT  
		Size: 4.4 MB (4394835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d46f97eee0e73e9ce759e89509d371d5240a48701dc046bbbf8cfe1f64f964b`  
		Last Modified: Fri, 15 May 2020 14:59:52 GMT  
		Size: 49.5 MB (49475735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:29da8a63cf35fa0e373e78683ea697d733d91fc6727c9b28b1183dec703c05ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110026709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b93600833a7d838c146a1ad78daf95df52d8d3f9593e8ff62e9848b82c856a8`
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
# Thu, 14 May 2020 00:10:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:59a5abe5a03ebb35ed027af57237427bf1650677f1d4c6a907f88cf889b5e403`  
		Last Modified: Thu, 14 May 2020 00:39:16 GMT  
		Size: 50.1 MB (50081278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e91d8d06eedd2decfafe5386de2f8594c5b5df2314e60f8f933319b98d838451
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110441778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1489f1695298394bc2f6d1b40633fdb812914de68e4357fbba2029c19b06f26`
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
# Fri, 15 May 2020 05:04:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:5ba95febc21c79324c26de8b0b5fd907b89a7799fd541030a61348f0fd2caf6f`  
		Last Modified: Fri, 15 May 2020 05:10:41 GMT  
		Size: 50.5 MB (50511235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
