## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:2f00b9c871de957da84402df12fa042fc739bba0c7d4a76ca45c240ac1ff9844
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2113; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.2113; amd64

```console
$ docker pull hello-world@sha256:7aa16b09ac1a7ad6fe0e255e3d12442061de286019a52b72d794c9df1003c001
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.8 MB (120756348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59eda14d47e5271140edbe264a82ad28b0c68df01d0815585a12568aae5eb53e`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Thu, 09 Nov 2023 06:09:19 GMT
RUN Apply image 10.0.20348.2113
# Thu, 16 Nov 2023 03:16:48 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Thu, 16 Nov 2023 03:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:1ca4fbe907f22e883670decfa8d7f4490a79a995bb83a6c286248c21d61a62f5`  
		Last Modified: Tue, 14 Nov 2023 21:13:36 GMT  
		Size: 120.8 MB (120753560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6676e631917c833e1edafff98df1dc7872d38e66c37280a6fa60494e4932a88`  
		Last Modified: Thu, 16 Nov 2023 03:17:13 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a47e19893594722a3963e9e56ce97098c55c22a1bef171a1f50cbcb530b0b5`  
		Last Modified: Thu, 16 Nov 2023 03:17:13 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
