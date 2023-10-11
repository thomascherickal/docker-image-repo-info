## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:f2de196b2dec15609b46a872f8ac471f6c05bf82bdf25376134cda5f3847d66d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.2031; amd64

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
