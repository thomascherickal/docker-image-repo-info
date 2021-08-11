## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:b3374d3945c1389a739fc74bb05fadd2232c9e9d2652f3e57e16147cb3cc9a55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `hello-world:nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull hello-world@sha256:e70692d3144e0ddb23e2ecf72d4b78f1e9ffcb32a9c863b98a35d43adfb42ad8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.7 MB (102744227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a9d119927e869538c3c0e57a7eb1dd8b0d885f28df91a0325d069227847b02`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 12:30:08 GMT
RUN cmd /S /C #(nop) COPY file:dbb4e437ca342a79d5980fcb71c065abfe00353f696b1b54084e7c09d32ec085 in C: 
# Wed, 11 Aug 2021 12:30:11 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd722a8ad7b404772d8bc6b4c4537ccfef35bb51e0be763d819ff1e35565e201`  
		Last Modified: Wed, 11 Aug 2021 12:30:26 GMT  
		Size: 1.9 KB (1892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d47b3ec78ed532400404c8d7f2b8860490b512aae4c9e70dfc896b7404124bc`  
		Last Modified: Wed, 11 Aug 2021 12:30:27 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
