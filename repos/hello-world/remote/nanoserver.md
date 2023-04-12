## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:d9ceead5fc5a77cab2d9b9dd2f1ca3a61f89c562950806b364681de2f8f18eda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1668; amd64
	-	windows version 10.0.17763.4252; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.1668; amd64

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

### `hello-world:nanoserver` - windows version 10.0.17763.4252; amd64

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
