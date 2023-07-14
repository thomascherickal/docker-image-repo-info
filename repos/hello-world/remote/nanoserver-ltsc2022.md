## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:9a0980d89ac8f0ff8f496f8656bf56dfc8036a4f88d87f7e5f6cf515fbdb12b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull hello-world@sha256:6f71ee7656f0d5af94fb271c296a5724d24db6c930be3367a9f00e29a3a2b5d2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120059503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:611d9f8e60c6fe24d4436a6d50c6b11b8055b05f0814c62eef446767f4ad9956`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Fri, 07 Jul 2023 21:00:40 GMT
RUN Apply image 10.0.20348.1850
# Thu, 13 Jul 2023 22:34:03 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Thu, 13 Jul 2023 22:34:04 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:cc0a26bd90fcc4d863317c36d7ffec77a0a82a905697204d4dcbc76ec13b3920`  
		Last Modified: Tue, 11 Jul 2023 20:10:45 GMT  
		Size: 120.1 MB (120056465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558193723ccf942b41f1d2e7394c0bb4584912e9be4a4d0bd52f5881bd01f419`  
		Last Modified: Thu, 13 Jul 2023 22:34:24 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e8240f7c6c5677ab33bb4efb4abd58364ea4e27fbc3a511c8a283281a7b453`  
		Last Modified: Thu, 13 Jul 2023 22:34:24 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
