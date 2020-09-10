## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:a0be928e674b48c7c18e1ad24fc69954ab1b9f2ee79b6fc343086d6b093a4b57
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9fb3ba8e7c0ceac6d46a645b3f4b07fca5e0ee5f593c72a50afa386b26ff0102
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129836153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:197dfb0f1385f8995783bb472f7e45833352a17a5a2e0638f5b94f13d4aa9518`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:44:34 GMT
ADD file:7b4df5810238cdff80845df3de1b017b9646e41ae4981a0dc81447c9e63b2e43 in / 
# Tue, 04 Aug 2020 15:44:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:34:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:34:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:34:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eb43504b07c3311fd407398c6de1b3b659cd4413087291e081d599040a320054`  
		Last Modified: Tue, 04 Aug 2020 15:51:13 GMT  
		Size: 52.4 MB (52403508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54da343b269771dbf23c5981583739bf4bd61a501a182b83e04658803eda3d19`  
		Last Modified: Tue, 04 Aug 2020 23:41:17 GMT  
		Size: 7.9 MB (7921868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd0e91d8a06079fba129e4b4a489c0ebd206ec45a25cf7916c8b7ab789c48d7`  
		Last Modified: Tue, 04 Aug 2020 23:41:17 GMT  
		Size: 10.6 MB (10580741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0511f36f89e95042414306efb1e65ac63d57f7d5c4947f3de90f837e2fdbfc`  
		Last Modified: Tue, 04 Aug 2020 23:41:33 GMT  
		Size: 58.9 MB (58930036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ca529eb83e87ee195ddac283e1fd746281621f827124760c1889bd939570cd8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124381214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d7012fbc78ae2025473372b02afeafbf918935fc191f68a2a572b6d02f550c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:19:33 GMT
ADD file:966adedb56b8840e71e14255f1e10c11506897b861f32a0c8c84c32338edea04 in / 
# Tue, 04 Aug 2020 03:19:44 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:24:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 06:25:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fc41871a830209ccc29805b1bb08b4058beb41df471ae13bc23555229a9623`  
		Last Modified: Tue, 04 Aug 2020 03:37:01 GMT  
		Size: 50.3 MB (50310118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c042826fa49924c4933b5f443c67da73885272c029983f30a8e5a154ae5b2ba7`  
		Last Modified: Tue, 04 Aug 2020 06:39:59 GMT  
		Size: 7.5 MB (7501462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f2d1c9e043d778892369b2ac4ba55c261e45346581518d8e9c0923f580979`  
		Last Modified: Tue, 04 Aug 2020 06:39:59 GMT  
		Size: 10.3 MB (10267096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1e363591d4c61017b4adf9fc9d4b3da3938064ff6fbb809e08a84bf5049cec`  
		Last Modified: Tue, 04 Aug 2020 06:40:32 GMT  
		Size: 56.3 MB (56302538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:00bdde0413f57d556a4e3c18e22352cf9dffb46e63e00c58292e78c147e8ff12
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.1 MB (119116563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5141699dd6e5bc3d4fc1139d0688ec931b82fd2806ef67f4e8b6077ba4192dc5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:59:26 GMT
ADD file:5793438e4679788bcbcd7ff2adcfe8f0c31bb4ceca63088d7c74a20cac1e87b8 in / 
# Tue, 04 Aug 2020 04:59:32 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:09:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:10:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ebc2f87ea858cf67ec5ea8f8fcd77fa8fefcd9b35b71d1b3efa355f8289ce59`  
		Last Modified: Tue, 04 Aug 2020 05:07:30 GMT  
		Size: 48.1 MB (48082910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76657e19ac1e0b31daaf79a3e351dad82e57e1e9714d8bcb5ca885c77b1150d`  
		Last Modified: Tue, 04 Aug 2020 08:29:01 GMT  
		Size: 7.2 MB (7243562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227bb50b47817c708c54d7d565ccfc1a6a7f89fdf3edf9cb85c81453f41011e2`  
		Last Modified: Tue, 04 Aug 2020 08:29:01 GMT  
		Size: 9.9 MB (9915847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f083ffc50f274a9b7bab4204c81cb5d08c3488fdec1a235c7acd3d6293a1702a`  
		Last Modified: Tue, 04 Aug 2020 08:29:29 GMT  
		Size: 53.9 MB (53874244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:44328430baab5c3e9347fdd6ef1d25ee203eb212774ca6a0eb6d75b6872d6050
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128484079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00cd27c1fdb23aeaf923d9fcc94d87ed418f847052a2fe65bb1242af5801b4ee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:52:18 GMT
ADD file:0b10d18375e8cd004468a07659e73e4afcd826f2808314dcc8fbb6b773c3ed6a in / 
# Wed, 09 Sep 2020 23:52:28 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:32:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:32:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:33:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21fc4451f3aee8da37deddc4046fa3dd8ea41b5a39481b93c43bc5dd385277d5`  
		Last Modified: Thu, 10 Sep 2020 00:00:09 GMT  
		Size: 50.8 MB (50845252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a512823677991a1ec2c1f7550a8c3a6487f162cd565b6dd962c3aa9b66dc8e4`  
		Last Modified: Thu, 10 Sep 2020 00:44:13 GMT  
		Size: 7.7 MB (7742930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8c9bf36c9423fe3a0d5d41b5d9036503bf5255e2c101307b378c250acebbe3`  
		Last Modified: Thu, 10 Sep 2020 00:44:12 GMT  
		Size: 10.6 MB (10635615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73d6346b9916616b4076b9aff9d017cdd90e7fb012d0b3d204e9b370267adb5`  
		Last Modified: Thu, 10 Sep 2020 00:44:39 GMT  
		Size: 59.3 MB (59260282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d8ee149c206668335140752ad317f3113df935235b87b1737f10063988cefee8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133450673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3863f9103f6d6f3532685dc0e1d9cb6e5081735f658caaf5d9ad432eae4e4b68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:39:04 GMT
ADD file:545a4c28d2d65f9f31d6deed3b22ae80dcdf0f0ba234b36acb715ebf6da67f3f in / 
# Tue, 04 Aug 2020 03:39:05 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:19:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:19:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:19:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5671e8963d62284adafd28133509ee2239373c96d0091ce2b4491327cac9724f`  
		Last Modified: Tue, 04 Aug 2020 03:44:13 GMT  
		Size: 53.5 MB (53490363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58173079354050a764e0b7ab86cb86890a027949b6c49f2f6e431042520f5793`  
		Last Modified: Tue, 04 Aug 2020 08:28:46 GMT  
		Size: 8.1 MB (8099063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5b5148c590d93c505260dbab5cecf462a0afd80a0aead458ebbc0ca4cbf438`  
		Last Modified: Tue, 04 Aug 2020 08:28:46 GMT  
		Size: 11.0 MB (10960412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0958f5cb4e332f3b1109c6672be060a7766e25652f77917b2bd99d249c2dc27e`  
		Last Modified: Tue, 04 Aug 2020 08:29:08 GMT  
		Size: 60.9 MB (60900835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7fcf0c58e90fba5214e308273e38405babe465310221963c6d6ca1f2a3a0d012
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127024819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6582d5155b6defcf7736732ebb05574bc50ea9ff080e56d6da8aae14f002d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:49 GMT
ADD file:c8977e04a216367623fcae06b950449d648b73fe2ebfeea8ac4d43b825fd9072 in / 
# Tue, 04 Aug 2020 06:42:50 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:43:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:43:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 10:44:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1b4f7d45a45e5da796e6015b373bab6d97853967e128d506ed0b95683b889a2`  
		Last Modified: Tue, 04 Aug 2020 06:49:31 GMT  
		Size: 51.1 MB (51146678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a299ca8f90646201e10c46e3299d7cb736e87e65cf92c7bc2363c5f7d61a0985`  
		Last Modified: Tue, 04 Aug 2020 10:54:08 GMT  
		Size: 7.5 MB (7450327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0eab5aef0c2a963011fc5090931d6499bfdbcfbfa1b05f6c2134d7eec1353f3`  
		Last Modified: Tue, 04 Aug 2020 10:54:09 GMT  
		Size: 10.6 MB (10599009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcde08b2db228c5f62bc2c132c08a80d4bb091d3fbbd8918d0bd2307cf756a4`  
		Last Modified: Tue, 04 Aug 2020 10:55:01 GMT  
		Size: 57.8 MB (57828805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:42f062a951f5ddf91308f24a7d2e21ce07fc023385576717d4140e86f9961e69
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140485459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fa8035a099f7e91d7379ee7efb65722b7fd57e5a4e8ead4f53ecae9b4d29106`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:56 GMT
ADD file:4f9206295fed0198f64e3e8588d30592afb355ad315b7f02a90d92274b37766a in / 
# Tue, 04 Aug 2020 04:46:03 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:25:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:26:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:28:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54ff323e52b64530253b6d180607b58565d781a9b132031a9baec3e1577690ab`  
		Last Modified: Tue, 04 Aug 2020 04:53:50 GMT  
		Size: 56.2 MB (56196736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6163322bc0beea20fbb00969be62fd8e2c8790b205e246ff0b8d2a3b72ed82`  
		Last Modified: Tue, 04 Aug 2020 07:46:38 GMT  
		Size: 8.3 MB (8347727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8dbc9e7891e1d54106baaa34d375e35b66be62a672cd47f7d6388f7ed7797`  
		Last Modified: Tue, 04 Aug 2020 07:46:39 GMT  
		Size: 11.3 MB (11327086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123657860e3a0579d09f7f5f2bed55b40d18ab151ca05653ce1c874ea4be1b9a`  
		Last Modified: Tue, 04 Aug 2020 07:47:10 GMT  
		Size: 64.6 MB (64613910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:eabca592483a97188ae446f4796530435e85483a83305ff6a9cc392ee8f38cd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127337739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8895a8d9f007e38dcdb73e7d5d045193bce1801895e468a1978d3b7fdbdd3f7b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:52 GMT
ADD file:8cf459b787b06e517199d5538d4a79b845b7b7d72ccf10fffdee5a385c0895bd in / 
# Wed, 09 Sep 2020 23:42:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:08:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0777a1517003dde2e616b494a11a7867f55924ffac710d8d2c15b7b50fbeea1d`  
		Last Modified: Wed, 09 Sep 2020 23:46:42 GMT  
		Size: 51.1 MB (51060992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333de3e2208d03a2b8282fff302f01069c5055fcb9e04e30943bfacf9e32d01`  
		Last Modified: Thu, 10 Sep 2020 00:13:13 GMT  
		Size: 7.5 MB (7541388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6b6e21fb8e9c70b582f6590d13e44a04a2d8a32abce90cbd029989466129d`  
		Last Modified: Thu, 10 Sep 2020 00:13:13 GMT  
		Size: 10.5 MB (10504798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4641be68cc7431e368872e2c3c9c8325d04514cd9438c155d8f8e071d0b023`  
		Last Modified: Thu, 10 Sep 2020 00:13:28 GMT  
		Size: 58.2 MB (58230561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
