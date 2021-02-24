## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:5f6147bdfe252c0cb07264c9cf5353ac1e90348b36687de8a486a86932c43be8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull hello-world@sha256:20878f630ec1d9a8c85ff62ca7010e87ec7dc45d0c194ff6b7279bdbfcd43634
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101409192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9c7d0f24fcae1179033c8f217369ee0e2840ce36846b76697cbe475a8b55bd0`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 24 Feb 2021 19:27:20 GMT
RUN cmd /S /C #(nop) COPY file:dbb4e437ca342a79d5980fcb71c065abfe00353f696b1b54084e7c09d32ec085 in C: 
# Wed, 24 Feb 2021 19:27:21 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:91c1a7f68777dea5e02fb553732817bdc24675e43e6960e386d3ebf7f530e60e`  
		Last Modified: Wed, 24 Feb 2021 19:27:37 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b040806f0fb4abf2daebe7ede13ff58557c506af675decb7cb3ef3cd6e746ca`  
		Last Modified: Wed, 24 Feb 2021 19:27:38 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
