## `debian:stable-backports`

```console
$ docker pull debian@sha256:3fd5c433fc0dfacb2920d3c3ada6907f656fb9453b3412b60f018cdcfc75669d
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:d7e571966c110afcc4c601b7f297f8af6f0809b83fa449ff6df582cb3403237a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50383081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53feacfa691e2ed10c876e5c8f654ac73e96075e2bea256d58ff90ec87813bda`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:21 GMT
ADD file:fa5e41bdd83bdcb44dba68dcf6fea81a4556ce01f7ede8168839fdcf0aeafb74 in / 
# Thu, 23 Apr 2020 00:22:21 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:22:26 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ab068d65c76515479a49d963119d9c4c88be2a322583227532edcd053131d61c`  
		Last Modified: Thu, 23 Apr 2020 00:27:12 GMT  
		Size: 50.4 MB (50382859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39e0cbf289adeac97b432064df46cff67e35441e001233ca4d3339e9affa41d`  
		Last Modified: Thu, 23 Apr 2020 00:27:16 GMT  
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
$ docker pull debian@sha256:3f55e03dc399277c9a9d44571b84de8b0f588645c6b1320d172508a92dfc1102
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51147195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0495de66f843e4ef53fdff97a3f522abc087b7e4fc5e308583c83a34ea75b566`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:41:31 GMT
ADD file:da50ddd228ee07b54262e4379379f3f7e8ada106fc660fbc09fb47145590f85d in / 
# Thu, 23 Apr 2020 00:41:31 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:41:36 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a4088cfbfca15fd87713a59e1368a9cdda9845981615080cf89f5c7b1accd331`  
		Last Modified: Thu, 23 Apr 2020 00:46:44 GMT  
		Size: 51.1 MB (51146972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00092cde2b0217ddbeb87b0330a471c4ffc9c54d02f747b66ce91696fc58e9b7`  
		Last Modified: Thu, 23 Apr 2020 00:46:48 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:639b176e27fb227c06ed1318e504daadeb4281f73d8219b1a515701e0001ac30
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49019385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df606ffcb68f591ac21c81e6aecae0920cd3f3575c35d913341080b4449023b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:11:42 GMT
ADD file:5a0065ff326073bf141f8523672b836937bbf34a234e73e42466ed4e18e3bdd7 in / 
# Thu, 23 Apr 2020 00:11:43 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:11:50 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:192cb836eb60701de82e3544a2c2279127dbd4f93030d06a700b28355cee7d0f`  
		Last Modified: Thu, 23 Apr 2020 00:21:17 GMT  
		Size: 49.0 MB (49019161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f26bb7e4228c121e48d3e89dd9fa8569c51bffc6ce0a89cd6c5afed485d2d3`  
		Last Modified: Thu, 23 Apr 2020 00:21:28 GMT  
		Size: 224.0 B  
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
