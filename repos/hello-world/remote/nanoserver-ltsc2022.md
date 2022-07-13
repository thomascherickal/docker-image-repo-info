## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:2a1bbdfaad0272a9f623b99e01893258da508553fa435caaa7b512bbf76d6eea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull hello-world@sha256:8377f36b3d74a8a4a95857a49d17a2969a2208eeb47a8af77bfa0136ef88e968
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.0 MB (118049128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c764b8ebd864571db3689163cd960f3631acafa81bb1f0d81dc629cc738994a3`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Mon, 04 Jul 2022 17:25:17 GMT
RUN Apply image 10.0.20348.825
# Wed, 13 Jul 2022 12:39:55 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 13 Jul 2022 12:39:56 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:3719b23d309b17276277110a008a58133c9fc92465d2519f2f32c9961c39887d`  
		Size: 118.0 MB (118046090 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b22313ae3c47142c42a487d166c96f6e6329478f07773b10d40568fd2c5fee3`  
		Last Modified: Wed, 13 Jul 2022 12:40:19 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e722b31e5c23da518f37f60b2a7ad6f256f58c21a0262c441ce20b71f07b40c`  
		Last Modified: Wed, 13 Jul 2022 12:40:19 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
