## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:ef4f226b8c8e2a0a38cbbd53667e3aaf25beda5f13f949a53da5300b9f3b7f6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.707; amd64

```console
$ docker pull hello-world@sha256:1e0054d86f2721056c9db5c2322fb8883d185fa1165bca69cb0ac88eeb40be30
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117689820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb0f03946a7cbb9366ca8a9045e3f7d849bc026c91f1dfb1dc12f69a70327c34`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Thu, 05 May 2022 02:37:33 GMT
RUN Apply image 10.0.20348.707
# Wed, 11 May 2022 12:31:32 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 11 May 2022 12:31:33 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:2c74f0842c5a8e9b80b9e2cf64e1ab10a6fa67951f28cff5fee060b88128564c`  
		Size: 117.7 MB (117687017 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:825f6e12476845d63b9d9cb4ea7d5d792e558e34c9b6a195fe7def6625c8cef1`  
		Last Modified: Wed, 11 May 2022 12:31:57 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ca6dbce3fe3956b4878e9bb1c7d6790a65d16a74c50907ee45e624c717ce06`  
		Last Modified: Wed, 11 May 2022 12:31:57 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hello-world:nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull hello-world@sha256:02a91a3365149788cc22339941adefe48166286642688a1f094c3517da4e37a5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103136600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61da702062180be943c409d01288803e5b38e6e83f5d20e5cabadc7e6e7c5bb7`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 12:31:39 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Wed, 11 May 2022 12:31:40 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc7231f2694a744d39a878d613fc5d0d9fb7655b2d6e75dc35675fe62aeddd69`  
		Last Modified: Wed, 11 May 2022 12:32:04 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3fcdbb49705016b949612bdf1dbd0c6ea9971efd1d867c4d7c4850a48c0359`  
		Last Modified: Wed, 11 May 2022 12:32:04 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
