## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:2003dddf8cc568c197a5926d5c515701951fc98d98b01d2693d603e8a83d19db
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:ec45ef53785038c4e6d78f094260df6b304f98b464733d64066f2df81f54a956
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55567481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8478ac217d3c676202cdf76fed12901ca8fe812d5f926315ed7e622ea9bc11eb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:47:43 GMT
ADD file:d564072c450ac56e020375a2295aaa9d2d8deb426d0a1a50f5a500fa401e7cb0 in / 
# Thu, 02 Dec 2021 02:47:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:47:48 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e4a54c5157321faded684f3a0a8bcaee56b08c45f1d38a4e0b0b690d7e1c98be`  
		Last Modified: Thu, 02 Dec 2021 02:52:41 GMT  
		Size: 55.6 MB (55567256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06aaa2a87a0443bca2089f80ddcbc3379f4e04f293da2786abf6d2fc236e075`  
		Last Modified: Thu, 02 Dec 2021 02:52:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:a50710df0380f67a284d2a2300f466f5056e344a617110f51a71dd6fb3fcca02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53031380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74706361bda1711805c7cfa34345529b2c12de4d83a491f8eb0704269b0ef7b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:00 GMT
ADD file:565dc0a92c6ce86500c032d7c7e8112f62771ff3bac3aa84192e8309ae7acbba in / 
# Thu, 02 Dec 2021 02:49:03 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:49:16 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:92dd04f71649984a91d8241840b2fa0a06cee72bebcd6503ece93ae1b5f47d07`  
		Last Modified: Thu, 02 Dec 2021 03:07:38 GMT  
		Size: 53.0 MB (53031153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901f9bdb26f2fcaf0ffa5c2d39c0ef10d210f8af310e92efa6b337b7356593a`  
		Last Modified: Thu, 02 Dec 2021 03:07:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:754437f2d1b75e9104554e4472155f0dfb70d03e1ca005545b9213d9edcc88e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50668211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd7aca774f43f50b0740ba35047a72f2a8f435b879f1fdf96aeac3ccd6105eca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:03:39 GMT
ADD file:bd5233b326b625660d820fa962832e6c5413ff9a56f64a6f072b9a9adfc545b2 in / 
# Thu, 02 Dec 2021 09:03:40 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:03:52 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4dcb906f06af542b010e092a9a4d4ad8ccb110debf57beb0d4ded9baa51b82a1`  
		Last Modified: Thu, 02 Dec 2021 09:18:59 GMT  
		Size: 50.7 MB (50667986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fb9f8a8eeb1a11d5a1d14a1b1b29f5559ddd3f9cab664e2629883b147b5ebc`  
		Last Modified: Thu, 02 Dec 2021 09:19:11 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b14a1a9d9ef5a74d1d147a7628264470a2d4be4c832630ecd0eb6df2cfffb2cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54576607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:160f54f7a0664ee1858c9fedd711be48f4f433434529c08d6b4040a2b5605f04`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:07:31 GMT
ADD file:78d948a7fd7213b583a0b4e09434d4542df75c0620617b011ad06accb9b6f26f in / 
# Thu, 02 Dec 2021 08:07:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:07:37 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f8d7e615d51e5d3f12aa3d99598a9f720f067abdee11ee16a770e8dcedce3069`  
		Last Modified: Thu, 02 Dec 2021 08:13:28 GMT  
		Size: 54.6 MB (54576381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbbbe28d2fef04117103bfb5ceb32fd6aa9dcc726a68f8dd0f15ddc32aa8639`  
		Last Modified: Thu, 02 Dec 2021 08:13:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:d6c643359f4d99374111fae2c74932ec88fe216d1eb14915d2547b1f7000a5bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56610449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54a9576e8b945343b01e6fa1e35c58d4f146848c6c6d44b172b1c7b014095667`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:39:07 GMT
ADD file:233579a3cce5db7166a5e91e9473aa28283fe69ec6809ce49c166994ffe2d461 in / 
# Thu, 02 Dec 2021 02:39:08 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 02:39:14 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:66c36ad92a7d15b3332cd4cd2fd424021c2ce01463b45621fcab89004c4c763f`  
		Last Modified: Thu, 02 Dec 2021 02:46:31 GMT  
		Size: 56.6 MB (56610224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ee8179926ed6277b4acdb7617f830ed37052bc0b0804b77fe6f7f0947e0c03`  
		Last Modified: Thu, 02 Dec 2021 02:46:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:08a20159ed23ba78318d847b7fb8a5454caa8a351f8a6095c9833ae3e4191981
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.3 MB (54269820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb1d2a8812283847cb5aa15b80cb4ed890154847feef633408f59f14cdfc4eb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:07:51 GMT
ADD file:2b78b392bcc6daef3d9c93dcae4adf8b84cac89c57ed08bd43854d23774078d6 in / 
# Thu, 02 Dec 2021 03:07:52 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:07:58 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8c4a35c3e932252ccb2418c1bc14531f11d21f13ba131d0a52cd9cb690dc9623`  
		Last Modified: Thu, 02 Dec 2021 03:15:53 GMT  
		Size: 54.3 MB (54269592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a8ca1adf7665d8b56eb5f4dee37f9b21d2c8d750c93da7939bf44e64c9d2e`  
		Last Modified: Thu, 02 Dec 2021 03:16:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:b4b32c9d948ab084825d28c7273a21a32145d53c80819d87c5b63009c030ac0f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59851596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64e1c9aa75865eb49b4409c88da5a5d5b7c24532c24a7b63da5a3fa1ac6fd7a4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:51 GMT
ADD file:b1221d684becfd74b167e24d774eb6099d264be14e0abd56599cb6a39c9eed74 in / 
# Thu, 02 Dec 2021 07:20:00 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:20:18 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ad94a9a32e9daafdd41e8b09d1671e7fd6b6d7cff42957db5b36cf5fe8276d1`  
		Last Modified: Thu, 02 Dec 2021 07:29:36 GMT  
		Size: 59.9 MB (59851370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bfb2b607328eb15d7ac51fdcb7b40674219e70a36bafea9f10c090e469c338`  
		Last Modified: Thu, 02 Dec 2021 07:29:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:9585209736dc48167fe103811bc16349462012e806b9a3727ae462734ac68608
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53867025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a20115bc9831f32e6abfb072d75943d87ed5a5aad315a71c62254151938db953`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:18:15 GMT
ADD file:4a1285cad893d349a6acf3dd79546f01288abd1351b9b86f32011a9d1dfa80a7 in / 
# Thu, 02 Dec 2021 07:18:19 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 07:18:26 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:2ce0b9fc523de2185f9dbec93dc5492c43667e801a28c8f6f3d92d45e3017e7b`  
		Last Modified: Thu, 02 Dec 2021 07:24:22 GMT  
		Size: 53.9 MB (53866800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59641226ef7691e01b29483948f64160bbfe156307bf7364298991c50cebb35f`  
		Last Modified: Thu, 02 Dec 2021 07:24:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
