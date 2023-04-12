## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:658e4681473ea9eb3cee69534ed5af06f26be3ef8556c20a2226ec12d08014d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull hello-world@sha256:5e022189f7e57e0b8b59d87a7c8d448eef7fc7a94418395ca8f0ffbed1d4cb84
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.3 MB (122331838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a3d96f0f4768ec39fdc77f3bf90e6415df140d18f05c93821095f8c27169fea`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:16 GMT
RUN Apply image 10.0.20348.1668
# Wed, 12 Apr 2023 02:40:15 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 12 Apr 2023 02:40:16 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:e06b772d586b58466a653b72002aee7c59496110e9ae402ff58f026e44452506`  
		Last Modified: Wed, 12 Apr 2023 02:34:14 GMT  
		Size: 122.3 MB (122328782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a8ad720ecf984f195a78c29f280f295a85ec6352f2e03aa8b62111f7a12ccc`  
		Last Modified: Wed, 12 Apr 2023 02:40:40 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e558bbc7fa8ce1efe7a035c9177f0c36f4f631b8a00efe18dffca7c1108608`  
		Last Modified: Wed, 12 Apr 2023 02:40:41 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
