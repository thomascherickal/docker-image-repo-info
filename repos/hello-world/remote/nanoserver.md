## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:558b36019a3659cab2a87ab12aa891259008f6fb5afb94957fddf14934543db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.1850; amd64

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

### `hello-world:nanoserver` - windows version 10.0.17763.4645; amd64

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
