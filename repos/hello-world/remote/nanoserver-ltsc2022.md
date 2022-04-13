## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:783a035d488104e3fb00e9319a169ad332739a23d9543eaa0abae0eef6fa5628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.643; amd64

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
