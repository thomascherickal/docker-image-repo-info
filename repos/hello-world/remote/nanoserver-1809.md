## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:11668744a8d8f6b60c1a1cc9fcda8898987a38056c50300b827e2ea6946fdb02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull hello-world@sha256:3b9bc61325891f9203f7b3a88b989781cb2da3f01fc489b171ed84e8c7a986d3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.0 MB (101022338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3af4d651cb22fbcd1714c9cffe075f3ac54f1e4489ffdb69a85b98a15df47f9`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:13:43 GMT
RUN cmd /S /C #(nop) COPY file:0afaffc2fa64462107b7178b2ae7d20404ff12f637eabe3a8046192b9d9a0338 in C: 
# Wed, 13 May 2020 12:13:44 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:030bb2557106405a77e15e5ee845017c004afad91d5c383aa8dbc2aed0c807c7`  
		Last Modified: Wed, 13 May 2020 12:13:56 GMT  
		Size: 1.6 KB (1600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a43d08f9d1f0878f57192c4f30e21134f69752add1d19ec546b9107b4ba0aba`  
		Last Modified: Wed, 13 May 2020 12:13:56 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
