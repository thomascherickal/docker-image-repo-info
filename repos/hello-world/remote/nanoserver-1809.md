## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:9e46c9c09f4e9fe5787d5d3ab4b7a0958c21ea0c4bed0722d39ea288008d4821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull hello-world@sha256:f220cf100ada1cad5d2c1ce8aa6765da9a261f4cb3911ba5a1bf039769fa117b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103207239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176ae9a1c97cb9b2d217b3c53e99931db185ce6e5e4664feb8d752745fd8d429`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 12:48:43 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Wed, 10 Aug 2022 12:48:43 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44a3a3e1ddc458b3e72ba23d3be4c0c5bf9e5a73c26249dbeda531ce8142727d`  
		Last Modified: Wed, 10 Aug 2022 12:49:09 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bb133af64fd59ae28f0c8c39af16aeb342ee6f9671dea111128fb6dbfacd5a`  
		Last Modified: Wed, 10 Aug 2022 12:49:09 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
