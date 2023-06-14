## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:9635aa61d2f4ded6c4fe872bbfc6ac9eb9ead3fae0ad40131c26d8618d68fada
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull hello-world@sha256:b4aaa8a7d6bcaddce4de86d84fda8e8c47363583f273a792f5a21a71b4e80d15
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (120031578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96fb9a013a942dcaf30c8cda86317ac503437e838a5fe3d8aa2717a5a8106939`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Thu, 08 Jun 2023 12:38:25 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 19:15:01 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 14 Jun 2023 19:15:02 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:f94f5e4cef3f52c830328b87b7298c638fa9ef22a0babf737eda2a2dd6d024c4`  
		Last Modified: Tue, 13 Jun 2023 20:05:48 GMT  
		Size: 120.0 MB (120028549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e081239de66420206edab006314510997bff2ff24a23b91363440873bb8a71`  
		Last Modified: Wed, 14 Jun 2023 19:15:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb32c3fd4583453977ef7fef16efafca2d713a458d299eb6f5ded7172781451`  
		Last Modified: Wed, 14 Jun 2023 19:15:24 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
