## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:d45f4f8e09708719186553b11488407e7b66c4ceb8702e01b83cadd9fbafc1a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull hello-world@sha256:fe74fbd310642e009e26dcb689ba2df81deac98fe28fd971aba907c9ad30fd47
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104512861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2eccdf85918fe8f08f56f1e84a0f8a30741aad72c5d622e5a2b8bbc8f5bc79b`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Fri, 15 Dec 2023 22:05:14 GMT
RUN cmd /S /C #(nop) COPY file:ab292695e43926d678c546efb98c5def57b169554a9718789f6d597045bc2114 in C: 
# Fri, 15 Dec 2023 22:05:14 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d191b5a69aba61b80376b47da6795ff862f0495d9d46816c13f3c77c83604bd1`  
		Last Modified: Fri, 15 Dec 2023 22:05:18 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768aaf9650a118b1685d7acced6804a16fab6c98d13f7259ecf4b292ee78f678`  
		Last Modified: Fri, 15 Dec 2023 22:05:18 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
