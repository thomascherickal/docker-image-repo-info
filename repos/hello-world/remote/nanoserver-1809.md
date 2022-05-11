## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:457df44e3c359d7de4a473dab5255fc670a5b558cafbaa125f14b2fe4e94f80d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.2928; amd64

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
