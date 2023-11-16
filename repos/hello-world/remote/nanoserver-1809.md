## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:f0a7e94a148fed1a5ebab7b6e03c4aa04e487c13b1b47a1ea2a18a5fb97e3129
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull hello-world@sha256:d4895b1920128bbccb4d28852f458be791c7de3b6eb2e89c475d328a55cf8b3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104500314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:619743389b4e4ca9205bb2094aa4117443c1e1bdc755e9a007ea1c91af90249c`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 03:16:55 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Thu, 16 Nov 2023 03:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441e173a4878a6fd174e57e2b59aadfe5b842f6bbe8b450a64c7b50e3ae13316`  
		Last Modified: Thu, 16 Nov 2023 03:17:19 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e64c5413c9933d7ddd072c9a7a1ff5449211c4f7c6ce64db1f9526a88e79c`  
		Last Modified: Thu, 16 Nov 2023 03:17:20 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
