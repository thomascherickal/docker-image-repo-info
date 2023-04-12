## `golang:nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:8e6f16c0453c8e1dba6f334d4fb22c4360c8819321a44a8efba48c06241cef02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `golang:nanoserver-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull golang@sha256:6e11a3b3a4a933182286acdba04a4740ee0068ae4fb47f77298666ec98bd096a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.1 MB (231084984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b2b6a9db546cc8410046da1c25c97d21f4f14c4cad625ade92e28a75be00e0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:16 GMT
RUN Apply image 10.0.20348.1668
# Wed, 12 Apr 2023 00:22:09 GMT
SHELL [cmd /S /C]
# Wed, 12 Apr 2023 02:01:45 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 02:01:46 GMT
USER ContainerAdministrator
# Wed, 12 Apr 2023 02:02:37 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 12 Apr 2023 02:02:38 GMT
USER ContainerUser
# Wed, 12 Apr 2023 02:02:39 GMT
ENV GOLANG_VERSION=1.20.3
# Wed, 12 Apr 2023 02:05:29 GMT
COPY dir:7f53f5369bd810a38f3697430c98fd1ef31e62b6dbcf30f7fe02d334a38965f8 in C:\Program Files\Go 
# Wed, 12 Apr 2023 02:06:24 GMT
RUN go version
# Wed, 12 Apr 2023 02:06:25 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:e06b772d586b58466a653b72002aee7c59496110e9ae402ff58f026e44452506`  
		Last Modified: Wed, 12 Apr 2023 02:34:14 GMT  
		Size: 122.3 MB (122328782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329579f5fc95fa89293545a20f4e45221db45261002e7012b86c4d3233edd1f8`  
		Last Modified: Wed, 12 Apr 2023 02:33:39 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785015715e7f6f5df91d88dc81eb9ed7bc36ef9cfefd565bbf522dff9d2d481`  
		Last Modified: Wed, 12 Apr 2023 02:33:38 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee11e8fa20dea6ccdcfb21ddbbdb24441556806bcffdb534698b12f27ccf7a4e`  
		Last Modified: Wed, 12 Apr 2023 02:33:38 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c53d49ef28647b964bc9d5a90c2567c0a8e57189eaf101b2d26cecf98953de2`  
		Last Modified: Wed, 12 Apr 2023 02:33:38 GMT  
		Size: 83.7 KB (83741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed452e8d633078d3cbc8aa29b71cdb34650769d2a1b2c008738aafc6f4aed361`  
		Last Modified: Wed, 12 Apr 2023 02:33:37 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceaf18629c1160309d186cbcf6130d1f282a6b1be7d6bd8b5b8b932c972989bc`  
		Last Modified: Wed, 12 Apr 2023 02:33:36 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077ad45669e510a6d4e6448b11babea886bdc35765ac503ee92a2fa33c92ac54`  
		Last Modified: Wed, 12 Apr 2023 02:34:19 GMT  
		Size: 108.6 MB (108616165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778e3997e3900be02895b60513c53e1428e881c18e3c88af6228080e9265ed66`  
		Last Modified: Wed, 12 Apr 2023 02:33:36 GMT  
		Size: 49.1 KB (49104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881fa28b135d2d5d4092b67cfdbda7e1e52c8d9d4aa7aaff884b02756fd154f3`  
		Last Modified: Wed, 12 Apr 2023 02:33:36 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
