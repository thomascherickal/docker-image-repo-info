## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:908f0ae75cae00369f0067321689f0484dde8a2b47739bff4351da1162a5cc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull hello-world@sha256:90e120baffe5afa60dd5a24abcd051db49bd6aee391174da5e825ee6ee5a12a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.7 MB (102674500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37a6d538021d27edf686dbd2031e09891f8cc98081b8daf9a760bda94379799`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 12:23:19 GMT
RUN cmd /S /C #(nop) COPY file:dbb4e437ca342a79d5980fcb71c065abfe00353f696b1b54084e7c09d32ec085 in C: 
# Wed, 09 Jun 2021 12:23:22 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cf2d5ca925aff15b75f9ce343176bb0462c7fc9b802343633ab7384bc7c78986`  
		Last Modified: Wed, 09 Jun 2021 12:23:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4044ff653a2aa908fbfe5cd5be21fdc6aa4abd71ec7605a1a920a51135e71f4c`  
		Last Modified: Wed, 09 Jun 2021 12:23:37 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
