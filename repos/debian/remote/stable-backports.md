## `debian:stable-backports`

```console
$ docker pull debian@sha256:fdfa8d7d7570aba4e72b745a6e4a5b915f699f7cb97df7652a220bd15a9d3d89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:5441cc13468145bb037bd6777cd301fb6bba138497fa1e5c71bd37ef55e453c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50382260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6cc06b9f263512ce2b043391e8ba0dc8805e04ad08ae2397a0827ab48396a60`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:23:17 GMT
ADD file:cb0e66fdb9a172efbd019fe6bb9f91a657cc9a5c5430497a08a60f7ac33f01f3 in / 
# Tue, 31 Mar 2020 01:23:17 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:23:23 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:cba288b0d4fd0fa57bd941c9f37069df1c6b451324bc2bb4ecb1aa000a901d39`  
		Last Modified: Tue, 31 Mar 2020 01:28:46 GMT  
		Size: 50.4 MB (50382038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753cbf8540af400959c23adaba363cf776ee7e89957b67ed099c04e016ab193b`  
		Last Modified: Tue, 31 Mar 2020 01:28:51 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:c817c4d18e75ddc55b610a890a97a9dd269beb887c56f0ccd4fef96c2c9f8a27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48097073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce719e8f295f3090e3d98f62a0adb16b3b6ff574336b8d476a1579b03a944b1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:53:40 GMT
ADD file:23f70ca25035d3d4691f839848ad06c67a1d2b9b576ca986450da4d0e2d8ea5c in / 
# Thu, 16 Apr 2020 00:53:43 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:53:53 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b5f6acc2ab7320368b23052537539aff44c7ec0bc510120ca3e5652bb2ff45a0`  
		Last Modified: Thu, 16 Apr 2020 01:01:23 GMT  
		Size: 48.1 MB (48096848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38999288a20674fe3a7c925e9d50e50922f3584ff2387315b355fe5e128d3b3d`  
		Last Modified: Thu, 16 Apr 2020 01:01:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:2acac217aa2341e1d86a5158106761b67231c8db0d997f8d4153f9c85971f53a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45864563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df07cd536773b4a8e4f4fcfcc7fb0e64ddf415ef33546172d096f3ef9e64dab`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:03:40 GMT
ADD file:c8406a97f6656403247a639ce59b98f335c0f5dc15316dd9081eb63390209b6b in / 
# Thu, 16 Apr 2020 01:03:43 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:03:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:86a12899828a2a74c1d490aa40f103bfc741565ebb89f0d48a06be44cc7b3beb`  
		Last Modified: Thu, 16 Apr 2020 01:11:41 GMT  
		Size: 45.9 MB (45864339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a5cfd82c03baa05106a6ad63ab2b6749013b69cd0f57878bfec7c7e7bfef55`  
		Last Modified: Thu, 16 Apr 2020 01:11:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:925ae330c3d4f15ac75e224c82fd23dda652e8580df1c283d4d2bc740f8ae40e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49169745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cee8630098921244f72aab4981055c844b327a3b32fce41b5a4b735eaf9b3d09`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:43:54 GMT
ADD file:e7d8e40e8e16f9a041b99e3e6c1924a60c92b408ac6d6f2121cf46d2d3507896 in / 
# Thu, 16 Apr 2020 02:43:56 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:44:06 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c101c9bed027a8f0e896efcf6b2e51e97889ed0856eb4e904703780a6c8ddbdd`  
		Last Modified: Thu, 16 Apr 2020 02:50:33 GMT  
		Size: 49.2 MB (49169521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11b574b85ace54b6add4863b74e56ecd527df1206a2daea859d919cb2c3bc8b`  
		Last Modified: Thu, 16 Apr 2020 02:50:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:9f5be85bf24b58544f0a675e46080e31e308af47186b4447783d966b78e0a927
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51147241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3543d53ece6bca33a583fa70200a8f3c2ec798488e1d46e68b9a172bb1c78c0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:42:29 GMT
ADD file:5e43edcd8e12a55513c38ffaa0a7274013c8791e38d7916d4aa607356e5666a2 in / 
# Thu, 16 Apr 2020 01:42:29 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:42:36 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:94ff29e37b6119ec87fd5bb4d1196063780a5ccfb26e2596c88faddfbee48625`  
		Last Modified: Thu, 16 Apr 2020 01:48:45 GMT  
		Size: 51.1 MB (51147019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e2a8cbb70c87d0b3b157951b7d62e7636575cbebe6420ef41f5e5a9c428063`  
		Last Modified: Thu, 16 Apr 2020 01:48:51 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:d1916990586594bb45cc9ee013e62c4818652fc7a27e2b2cd447524184ebe41f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54139807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41725a3a9f0e4ea9b3b9ca41749f0e52a85be78dfa09c77b9dead7b079e3f071`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:41:33 GMT
ADD file:85a04362e3efdd250997ea9bba80ed52756ef0c3f7322b3a960268ff89143de9 in / 
# Thu, 16 Apr 2020 01:41:41 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:42:00 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b1c24aa5245c0d34897b146a84d40c7f507611a524be7916a8e115d7a2d3be2b`  
		Last Modified: Thu, 16 Apr 2020 02:01:30 GMT  
		Size: 54.1 MB (54139582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41f440dba8d829c3c6302a57335cbda96baac37071cc3b0dc0a996aa3ea58ed`  
		Last Modified: Thu, 16 Apr 2020 02:01:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:c5c875d6e2c8f11a9427529c040863f44721f89780d983427679ff1fcbfe6700
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48960397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:834a3b1488b1cdf6f77ed32a17267ac3cb1d3302031d9807f64e24a70ec700b9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:43:20 GMT
ADD file:2eb7b2ec60faeea186fb3ac331d6e27ac16caf96b1951795f3f00f0cea4af2b7 in / 
# Thu, 16 Apr 2020 00:43:23 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 00:43:28 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:58df80516a6f54a565a783ddd86a13707e5d2deb530c3150e59c3e85635b644d`  
		Last Modified: Thu, 16 Apr 2020 00:47:49 GMT  
		Size: 49.0 MB (48960175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2faba9e69ba9499a45c30ea4b2f1cd886a99eaf40956348aaf77b9ef4924405`  
		Last Modified: Thu, 16 Apr 2020 00:48:00 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
