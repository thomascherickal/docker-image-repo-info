## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:35591f2099b26e84656bcb2651b38bc2f2d67b9b7db22743045eddadbafbb6e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.887; amd64

```console
$ docker pull hello-world@sha256:3624dfaed3b147d49409b0306a2faedfc8da7117b1b59d81714632cef2367e57
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.1 MB (118091473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4d88879abb06dd4d6f3cd4e0ca1bda978afd4e049c3ca21390f4bc724ef2664`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sat, 06 Aug 2022 18:05:23 GMT
RUN Apply image 10.0.20348.887
# Wed, 10 Aug 2022 12:48:36 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 10 Aug 2022 12:48:37 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:2ebf439f800cd4c1fccaf4a0545e6bff60caa5141295c8ab81f6c525073c423d`  
		Size: 118.1 MB (118088450 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:59d9f62c09b7fe34e1ed694e64ada66666a798fcaf80db61e92b448386cb9e5f`  
		Last Modified: Wed, 10 Aug 2022 12:49:02 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6884bc3f6c78d9a07ee572115cc1a2f9a103d517ed2d0924b89d0e4ab1e6271`  
		Last Modified: Wed, 10 Aug 2022 12:49:02 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hello-world:nanoserver` - windows version 10.0.17763.3287; amd64

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
