## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:3f7bdfd2bfb8b67f8677522e4b36570aefadeeda190eec921200ebe9697d7ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1366; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.1366; amd64

```console
$ docker pull hello-world@sha256:931f97f6715efc40b998b68159fccb663b6fdfdf4b323001205f762e9bab02f0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122111197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c8c5cf24eda0e5f6971a7b8c7db3a5da4bc5c3028277f35c63167171166c060`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Fri, 09 Dec 2022 09:19:21 GMT
RUN Apply image 10.0.20348.1366
# Wed, 14 Dec 2022 01:24:27 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 14 Dec 2022 01:24:27 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:70d3e1cc3b0ea172dcc93064fe6fb9f1f2c8fec6962c90e39991fe89a3c1ca03`  
		Last Modified: Wed, 14 Dec 2022 00:08:13 GMT  
		Size: 122.1 MB (122108200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b665be2399a25f3356be2bcd11b608906ffb3af6151a7ed1561c75b55f0da66`  
		Last Modified: Wed, 14 Dec 2022 01:24:52 GMT  
		Size: 1.9 KB (1896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c3ebd1894a76146640d44ca8f17a61a1922c6fd1453d54b99f7db832c2c2fa`  
		Last Modified: Wed, 14 Dec 2022 01:24:52 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
