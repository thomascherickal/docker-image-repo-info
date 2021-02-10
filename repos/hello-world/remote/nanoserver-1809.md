## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:753aad4ad8735de7e6f27b52c4c1744c48a1aaa712a28e9c3c4bc26995ec526f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull hello-world@sha256:f18513a718d2588b48f7e193b373ab4f22ef711f4adc1227821d07ae96d8f885
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101409125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e58cfe4497ee5b9f6aa6cc287ddad3d071617793f2e78540ca23297e3fadf35b`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 13:13:15 GMT
RUN cmd /S /C #(nop) COPY file:0afaffc2fa64462107b7178b2ae7d20404ff12f637eabe3a8046192b9d9a0338 in C: 
# Wed, 10 Feb 2021 13:13:16 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:264682c513c11b55828f5b49b6e06573305b2ee31920b8d48ab4e3a8b7de55e3`  
		Last Modified: Wed, 10 Feb 2021 13:13:31 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeb77aec790591a44b2b73c80fca376b9d281f3c88c90e2d9c45bfc97415c25`  
		Last Modified: Wed, 10 Feb 2021 13:13:31 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
