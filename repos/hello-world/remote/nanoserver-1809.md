## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:65933d14e67420901b30304f45444939baaaef6e57efc198bbf3e2c00af8250a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull hello-world@sha256:6a39434ec53e8ce7251d6fb8123cfc93c9306292035f130090bf6ca9a26010b9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104462452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bd71aa1d0395addad1d5bcd2a9f5161315b020216100d5be45264cceea6f136`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 01:07:33 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Thu, 10 Aug 2023 01:07:34 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13488e9375be8bd7dc3dbc70a6ec07b81b5b82594ff898059f08a4b851051a40`  
		Last Modified: Thu, 10 Aug 2023 01:07:54 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed4b8ef30c3415fd624352db5d876cfc70d4962abaf7c11b284483481557373`  
		Last Modified: Thu, 10 Aug 2023 01:07:55 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
