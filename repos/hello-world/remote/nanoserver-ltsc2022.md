## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:27f5aab8087f948e933f5a98421ba80c930a8f6dbdb076eed07ee2e0845d4d36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull hello-world@sha256:fb353688bcf45fc724fde3d1dcd7935ddf56803e2b7027164a7acc28758002f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122095116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da23fb7f406b3d5450749db232f19a2661b191a6bd2cdf9031c9c07dee472055`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sat, 05 Nov 2022 07:21:30 GMT
RUN Apply image 10.0.20348.1249
# Wed, 09 Nov 2022 13:50:07 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 09 Nov 2022 13:50:08 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:72e5d750fe8c1a32d4a26ef3b4a4e1f6124ac079b142f12724af2abfcba1c8b3`  
		Last Modified: Tue, 08 Nov 2022 19:57:58 GMT  
		Size: 122.1 MB (122092167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4267a005d89882fc74ee2259ab7e96e1b12bb529cbb189a0fde4805c6784432`  
		Last Modified: Wed, 09 Nov 2022 13:50:39 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed05d2e398c3584799b97b4b000a5c2f3681576df31f5a72bb56778afd6fe940`  
		Last Modified: Wed, 09 Nov 2022 13:50:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
