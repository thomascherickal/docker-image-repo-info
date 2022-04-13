## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:4ecfcb83d3001c2f97d38574f85679b760d5a9c9f890c3a36b93e4ce76e56c57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull hello-world@sha256:da03ca87e3a87e604bbb98e655d788c0b2004aa94f5d122c2156be5694f80d3e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103099217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b276c1536eb5f660a5be58f7a1ed2e194881af65c7992d30ab461f43d7fbf73`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 12:32:04 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Wed, 13 Apr 2022 12:32:04 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a741b3521f262fa0352ad4ef55f96066176632202ca489dd37b9a39276272891`  
		Last Modified: Wed, 13 Apr 2022 12:32:26 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941916a323b2e1ed371320204d90bbc58a9166fbc0cc245085a4756923aca44`  
		Last Modified: Wed, 13 Apr 2022 12:32:26 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
