## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:ecc4cc44120d9d5558337532574db8122c66bdf2a693fe8a659f925a0a9af5d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.887; amd64

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
