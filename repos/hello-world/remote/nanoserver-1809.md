## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:26acea9ef1c510cc374ebda70a462ac1ebee932e05aa64a5a762cc0e246f8d0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull hello-world@sha256:8ecc1906cb80f3250bc965d853a1d0ad964ab40d2ae929d0a8b9f04250d749b5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106791984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4a09ae782323e9fda58d34f95bec459c4f7926c193837066f7f26e2af982b83`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:40:23 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Wed, 12 Apr 2023 02:40:24 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4600013d74378244aed7509ec5fa7e64d3c0d8afd0136263bb31678b65e83f6`  
		Last Modified: Wed, 12 Apr 2023 02:40:47 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81950d3c9d0fcb88fc5a3206cf4370301c38a12d99b1787a96c2c03fa7d642e3`  
		Last Modified: Wed, 12 Apr 2023 02:40:47 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
