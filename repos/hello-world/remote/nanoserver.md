## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:13d2dd17c8e64887705713dee510b1a1d19dcd616bfab55945118d467de15416
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.643; amd64

```console
$ docker pull hello-world@sha256:156531cc3466371c4878b9fb5fcf36ccb58838de9dd9d528c531e0a02f939b06
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117582408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:517f77869f8db8aafa652695471925617d1f2543b1126169f0125593a5c7b012`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sun, 03 Apr 2022 05:29:07 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Apr 2022 12:31:58 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 13 Apr 2022 12:31:59 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:5ee98801bdad72bc36678d072c89f7dd482fee29086c1d9c8ad6ff0cb5afa385`  
		Size: 117.6 MB (117579416 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77a32385c2cba13b378cb3ed8505b79706fac54dbe0c57594daef92fc742abb4`  
		Last Modified: Wed, 13 Apr 2022 12:32:19 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1374b88ff460bd549c246b6cab07fa5fdc34c4ce7d7a709493b62dc08e318c8`  
		Last Modified: Wed, 13 Apr 2022 12:32:19 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hello-world:nanoserver` - windows version 10.0.17763.2803; amd64

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
