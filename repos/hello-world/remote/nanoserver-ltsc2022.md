## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:6bfe80c89fd429a09f88cc5e1a04979cf7ccd849677b49a4a61bc74ac2effa99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull hello-world@sha256:088ccea51a3d18c2dd1cb30809c71014b7ec11aa0cc7a677df11e26798a70d15
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120503730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:519639ac44cb25b2dedbef86e5dbb9ff29875c67628aae581f0f09ef2e7326d9`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Thu, 03 Aug 2023 09:40:19 GMT
RUN Apply image 10.0.20348.1906
# Thu, 10 Aug 2023 01:07:27 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Thu, 10 Aug 2023 01:07:28 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:ea9613880997b3ab2284a37c0c14a403553457b0c331b41c6bd6d1cc7838a222`  
		Last Modified: Tue, 08 Aug 2023 18:47:21 GMT  
		Size: 120.5 MB (120500677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e54c6461f0b327427c5941262cef6a5b5ee6b706e01f922a367d8f9606c7af`  
		Last Modified: Thu, 10 Aug 2023 01:07:48 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e327b1189ec4c0896298e14f9ff58f78ce23f537280330d953a3590dc3d6672`  
		Last Modified: Thu, 10 Aug 2023 01:07:48 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
