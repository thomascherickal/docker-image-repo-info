## `debian:buster-backports`

```console
$ docker pull debian@sha256:aff49e3ad895ef738d9f43990c90ab35f66668a5f6861a177cd5cdfe0bd207f8
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

### `debian:buster-backports` - linux; amd64

```console
$ docker pull debian@sha256:6efd2ae4c36aa57d2f225cd47c51bbc478695198820444ce38126fb5eb0ed8ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50383152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8984c136ba7ac79be63792aec5c8ea9da7f6cf227887ecd57578c633ad0a8be`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:17 GMT
ADD file:f086177965196842af3c15f50a7f6ad7912aaa7bf73a60b1d00e3129265eec9a in / 
# Thu, 23 Apr 2020 00:20:17 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:20:22 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:90fe46dd819953eb995f9cc9c326130abe9dd0b3993a998e12c01d0218a0b831`  
		Last Modified: Thu, 23 Apr 2020 00:24:56 GMT  
		Size: 50.4 MB (50382927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ef6dbd517405e887c80ae5e3dc38151f7f651a17601dba0dfaaffe292b773d`  
		Last Modified: Thu, 23 Apr 2020 00:25:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:71c7158afdcea93afec996f1a32273e42e54655604bca0344126acf43fe742cb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48097047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27eb2ac7b1ba1b80f79e22dfcbc2a6f3df1be857e6297c07d5fe82c46ab58158`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:49:45 GMT
ADD file:1daed63e84abade24fb29c2232024fa993101aafe8a874d4bef96c5635c9ce6e in / 
# Thu, 16 Apr 2020 00:49:48 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:49:58 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:e139f841569e5d49ea694b0ac42568ff6f00a378e70c53d3153f77487eba09c0`  
		Last Modified: Thu, 16 Apr 2020 00:58:04 GMT  
		Size: 48.1 MB (48096823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17be88fa3228ca9d70ae7db7377eb39aae38d71a85d7cf3b875821d85097f9e3`  
		Last Modified: Thu, 16 Apr 2020 00:58:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:06c497346f4b4ec92007d4f4dbd1d00dc181a8163d917da792feca4993c4d8aa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45864596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a4e21a739ca3061b74cb6bd97868f8e308ee15cb6704324fb5c006b8298d22`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:14 GMT
ADD file:c2369e5669e570f90abaa1fd4fcea4ae1e6654bbd81e8fa070a5b2484c03ee74 in / 
# Thu, 16 Apr 2020 00:59:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:59:25 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:020b29c91094d59c5eb128b7bc2b0b835e2ba4414358664e467428fe8b95bf52`  
		Last Modified: Thu, 16 Apr 2020 01:08:38 GMT  
		Size: 45.9 MB (45864371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8a051f92fdc89995370b689b7d1f1f34c1fb089a7187c7c390feafb4d6ce35`  
		Last Modified: Thu, 16 Apr 2020 01:08:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:cc66c267357ddf4588fa730dcbef12e2559aaaafd89357657b90797c7d05ef9d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49169745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee3f5f038d1b2e68f54449c033b5bd8d058c01768dfb9be06793116d728ff02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:20 GMT
ADD file:02afb66e938cbc67271aaf8cbee75def87458a21d961d02e86383e0ed36b0c71 in / 
# Thu, 16 Apr 2020 02:41:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:41:34 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d080dad46627d4103daddf54c89f2ef0a0b72ba8270066c50e95ffbf4a79362e`  
		Last Modified: Thu, 16 Apr 2020 02:48:36 GMT  
		Size: 49.2 MB (49169521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2699b166f302ea66232d63fcf456985f76c6ed7e536fa65b785bf25ddb72343`  
		Last Modified: Thu, 16 Apr 2020 02:48:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; 386

```console
$ docker pull debian@sha256:4c1752a580c0392750db6f75e1269cc195fc457ed1930f0debc27c7f233297a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51147265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46b2aef1b82dfbe7edf99508ba75c670cc112f2dbae78e5a9d93782e24dc7190`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:21 GMT
ADD file:10751e25934ebcf54b529ebd800a690886012d472846a404b452a1b27dc97eed in / 
# Thu, 23 Apr 2020 00:39:22 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:39:27 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5ca4f2c0deeb8dae824229454aa24e8d27bb031c4d3229fbc5465ac18d0fc46b`  
		Last Modified: Thu, 23 Apr 2020 00:44:20 GMT  
		Size: 51.1 MB (51147043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c047a466c4abc798720bcb0887a84f4c41ba00bc4e16e85ad0ca4117fd8c528`  
		Last Modified: Thu, 23 Apr 2020 00:44:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; mips64le

```console
$ docker pull debian@sha256:cb836d44e37b3c8544d984795bfb62dbb23b11b801dcda1a0c2d149285ddff54
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49019384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4c9856a411d457c6f70653490652d9e5c0ff105d586dbb3c9e8289ecaf80c7f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:25 GMT
ADD file:ef71e7285bfdea3942f5b4db577b5b14ba7dbc37538dfeda1886a6afcef86692 in / 
# Thu, 23 Apr 2020 00:09:26 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:09:32 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7754e26af5c07372dee067377cd032efd21a4266d2a432d0bfd78f25f8cb5e64`  
		Last Modified: Thu, 23 Apr 2020 00:17:03 GMT  
		Size: 49.0 MB (49019159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436e5b125c4940ce0f50e3fe7c2beb3eff8d65906a6fea6573c727694a8afb50`  
		Last Modified: Thu, 23 Apr 2020 00:17:19 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:1f46e73afeeb773e2f6d3ed1de477c470f061b134a81790e631077e5ed68c885
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54139788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8ea7dd8073d7f307fddfb180a81b164a3314d71758b0a7d8b5162256a2d02fd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:37:39 GMT
ADD file:5ea6b62430ec58194ba5685d0b5ecbc2df83c01b4e6c7d8b70f3e96c89390cd5 in / 
# Thu, 16 Apr 2020 01:37:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:38:08 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:219153a374347511566d1327acf4e45fd3425c20cd49110ef8041930fdb965a4`  
		Last Modified: Thu, 16 Apr 2020 01:53:24 GMT  
		Size: 54.1 MB (54139564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b6a630d1b9c8d627205a3821f78d13d22dd00d27b75971ae6dd7d8eb731fbd`  
		Last Modified: Thu, 16 Apr 2020 01:53:44 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:buster-backports` - linux; s390x

```console
$ docker pull debian@sha256:05082fb3854c32dcab3b52264b674b8616968382867fc673020c46c6d8867710
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48960437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19e50f1b169680d37d63511cb5c3e96caea37d924c8c3ef4f5162824373e293`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:03 GMT
ADD file:26367817216af13dc3ba9f495303f7bee8fe138fc8fb728289781563308ce0bd in / 
# Thu, 16 Apr 2020 00:42:05 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:42:11 GMT
RUN echo 'deb http://deb.debian.org/debian buster-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:54e2fb160a5d4a95ec7efe70c0045923ee557e87ee68ce03f2150b8366f26729`  
		Last Modified: Thu, 16 Apr 2020 00:46:03 GMT  
		Size: 49.0 MB (48960213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cc78ae6cf29741b68ceae25683744b2854cb4dacd31a959c4afc5b3bc15b67`  
		Last Modified: Thu, 16 Apr 2020 00:46:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
