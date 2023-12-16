## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:d421a2daec833ae03569727f5456016ccbdf893918867eefdfb11f4e8e2da40a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.2159; amd64

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
