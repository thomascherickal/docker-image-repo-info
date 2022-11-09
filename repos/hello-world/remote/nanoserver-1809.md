## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:16a5598b275fef66d7b85518dc7c3c7d3cfcfc8745afacd0066b36905498ee73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull hello-world@sha256:c597fadc51747a7392f4d0312e9740aaee11793a47658a77a4ba51bd5d9b6be0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106726577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e0642de95d2933b18cee07e6855db56e96490509e729c5d89cb75c0ef8a6d3c`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 13:50:20 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Wed, 09 Nov 2022 13:50:20 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a68771cf15a60e5f06c6d473f353291ea4a606bfce1acffea8816095aeb42`  
		Last Modified: Wed, 09 Nov 2022 13:50:46 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1491898410a23ef51f66b21a67079da3fef217d88024374bea1618072d8275c3`  
		Last Modified: Wed, 09 Nov 2022 13:50:46 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
