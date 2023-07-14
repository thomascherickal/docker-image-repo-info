## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:7d829fbe03a89f2f8a6e7964047b82269be85bfbb4e95aa15a0f38cba86a8dd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull hello-world@sha256:91ff1a715efa1e5ac1349d069c3fe3ef48d8a74f732b5f2eb23efd28795bff14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.4 MB (104411275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b4b7a6d2f0b277d954b52716fd49661b7c4ab6f2d4012e59ce9acf25ad3986d`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 22:34:09 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Thu, 13 Jul 2023 22:34:10 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951b27319c56e2f608a3662c953a96f537fe8700d2e49b9f7654f8d083a17f4c`  
		Last Modified: Thu, 13 Jul 2023 22:34:30 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390ab616b216480a475d5934934556cbc296b415bed2e9f32d32cf762f941f8a`  
		Last Modified: Thu, 13 Jul 2023 22:34:30 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
