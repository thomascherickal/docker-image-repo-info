## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:4a013f6e621b040ed030861cb0bd02d96ef23c7a5fbf2019841921e255379ebf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
