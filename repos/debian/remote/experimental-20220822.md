## `debian:experimental-20220822`

```console
$ docker pull debian@sha256:5f123179d4aa1b680f069952124d56db3cb15e47e4b1ffe1dba515eade0f1b9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; mips64le
	-	linux; riscv64

### `debian:experimental-20220822` - linux; amd64

```console
$ docker pull debian@sha256:7ed2f1729a2e49b53b19733779eb763c30901fcedd89c3508e8b3c7b4e4acc0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52769000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e26f8d70f370666e8f61316464730a954bb39a7f09736fd118d89400a1d038a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:22:36 GMT
ADD file:fb5801241cefe989ebaea4535c1783ade754d3f110b6582a1bf373193075d454 in / 
# Tue, 23 Aug 2022 00:22:36 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:22:47 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:9982fb59e253104d024374bedd9697731eefe95d4c35d5f4d76b419739ba8548`  
		Last Modified: Tue, 23 Aug 2022 00:28:22 GMT  
		Size: 52.8 MB (52768778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92dc0bf0ff16d9a34d1c033e455af7967e1f39edcbfac4a6d21eb5c1459ce38`  
		Last Modified: Tue, 23 Aug 2022 00:28:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20220822` - linux; mips64le

```console
$ docker pull debian@sha256:7f1b884cbbffa5b3e0d22f887d427dbf8f9b7f7bae3e4085dd5aee0a0baab28b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53216875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7054f25de1425f072e88a81807a07f1e3f38fc2072c6807c4dd3a120cb230e4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:15:27 GMT
ADD file:289ff967122b94852c18b08616d72bff729cc9d607c295c6c758bb8917ce5864 in / 
# Tue, 23 Aug 2022 00:15:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:16:13 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:10ecab1bdcec7f490bd4865c91fc25cfc0d3d5506b9673055d7740a86765bdea`  
		Last Modified: Tue, 23 Aug 2022 00:24:06 GMT  
		Size: 53.2 MB (53216652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8187526258e55e7a283249775de7fdac990d25e667fd1d930ae0538e05ef8d`  
		Last Modified: Tue, 23 Aug 2022 00:24:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20220822` - linux; riscv64

```console
$ docker pull debian@sha256:d0fc011bc400eec92d94f1fd20be03a0b297fda36f5c500670e6a3fc607ce352
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49268422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b818a232cb48bdf3ca4b84bf371194cf9db7306df1a847f76a5b93c975490ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:15:54 GMT
ADD file:922879b545740da41d47ffaf3bb1d9f5cae855386457ae213834f5f1eb869dac in / 
# Tue, 23 Aug 2022 00:15:57 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:19:28 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:243eeed5cf29613bd014532fa4bc8fb367b678d2973dc4a950c09bd2df4886c1`  
		Last Modified: Tue, 23 Aug 2022 00:34:23 GMT  
		Size: 49.3 MB (49268194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9074adb383b955e8e4e755127062849db72c1e821950bf6386d8470eff567f`  
		Last Modified: Tue, 23 Aug 2022 00:37:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
