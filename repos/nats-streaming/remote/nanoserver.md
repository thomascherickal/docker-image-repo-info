## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:2ea85a60361e0774ce1913ef12baa8fc87bfa4a837a811e89a0a32988b40ed14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull nats-streaming@sha256:5c39267b2e159ad82e792287b1086208f57dbf20ef18e40b553f3b377b337545
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef72ff049bb8cd1e4d7c65b5e46d477eccc664570d1a61e14b52bfc1faaa98f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Fri, 14 Jul 2023 00:03:16 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 14 Jul 2023 00:07:54 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Fri, 14 Jul 2023 00:07:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Jul 2023 00:07:56 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 14 Jul 2023 00:07:57 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bad9bf846d07362d8295a4479f8f2965dfb5934a9a032b335ce3cb086bdf7`  
		Last Modified: Fri, 14 Jul 2023 00:04:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94b9b520f177b081bf712ba074ba66cad6139b8164f8e18de5be8ebd3ae7382`  
		Last Modified: Fri, 14 Jul 2023 00:08:34 GMT  
		Size: 7.8 MB (7786370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03838a3679d351be263b09d3a5c6b9c44c73bd67df1a32d00364b15614d8b4c`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7169624bc074e90056b7387038bd434dc1bc770b6ac612f0d295d8db6b10f`  
		Last Modified: Fri, 14 Jul 2023 00:08:31 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ef31773aef63c527f320ae07bc5b102bd9f4f448f3b8d21c3e339e30db10e1`  
		Last Modified: Fri, 14 Jul 2023 00:08:32 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
