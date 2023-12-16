## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:7cc2f170e71159c37c71897bcf15ff59ee03dda0b2d16decc66cb7a137a34810
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.2159; amd64

```console
$ docker pull hello-world@sha256:18d9b0d6e2443810592341af797f9e07e847aede26fd795fb5d89a793780bbad
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.8 MB (120759835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7299156a1e9cbce8469a8ab41a2bc52dd22fb498b3d7c83ebdcb82804050ce`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sat, 02 Dec 2023 12:14:23 GMT
RUN Apply image 10.0.20348.2159
# Fri, 15 Dec 2023 22:05:15 GMT
RUN cmd /S /C #(nop) COPY file:cdba4efa08a1e42c8764fb75c060ef33719f72777fb28a7592f718539560d6d2 in C: 
# Fri, 15 Dec 2023 22:05:16 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:075332bb10f7fc70c56f7c073dd753e05cacbc93a38c181c5576739a29f8a7e1`  
		Last Modified: Tue, 12 Dec 2023 21:35:16 GMT  
		Size: 120.8 MB (120757041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0e8aea255e154bfb215792ba49a648b92d4f1d02505fa547225c82e5679569`  
		Last Modified: Fri, 15 Dec 2023 22:05:18 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddbe7a23c0fbaa4b28a8f5a49074c09859274ef4dfcece0541bb642fbd07e69`  
		Last Modified: Fri, 15 Dec 2023 22:05:18 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hello-world:nanoserver` - windows version 10.0.17763.5206; amd64

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
