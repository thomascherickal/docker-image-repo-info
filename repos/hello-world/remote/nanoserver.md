## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:a5d9251753fea16c2572a75b9d4f4d309d9e5729862dab67def36d3bda79b6b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull hello-world@sha256:864c195c22d2c86e7e60b4bc34c5d3d4308e88618b45d6c134e7d6a794fcb7a6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.6 MB (120607361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21892d3f5adc37940835cb29db95479fa434aaabd3b6aa82ec0c1c18f5813758`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:53:11 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 11 Oct 2023 02:53:11 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:fff54800e03713ba81736f43d985319592fc643a1a32b62dbd5c0ec36549de00`  
		Last Modified: Tue, 10 Oct 2023 17:30:43 GMT  
		Size: 120.6 MB (120604344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b066dfa8d937386fe33e13cfe0c20d54dfd6d30552b2f545fa26601b72e6f`  
		Last Modified: Wed, 11 Oct 2023 02:53:40 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f16e5b22025580ea01e44ee24dd3c2290cfb0bcf5498fbaa4aa369ef1e62659`  
		Last Modified: Wed, 11 Oct 2023 02:53:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hello-world:nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull hello-world@sha256:e1c66f56cd584a6fc5f939fb8fc357b9c715830605056a9c1a9c9798f7029647
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104467623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18db4bcd78333c88f5881487d746720eceb250d08a939a96820c8d4fd04ed25`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 02:53:19 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Wed, 11 Oct 2023 02:53:23 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ef0991d147a381f0927e7a589380073551449c28a6ecabdffedb2f0d877c3`  
		Last Modified: Wed, 11 Oct 2023 02:53:46 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ac58c0cb712c15a72286fc4f400444677f8c045be918f73da000b869c63370`  
		Last Modified: Wed, 11 Oct 2023 02:53:46 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
