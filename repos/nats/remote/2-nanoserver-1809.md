## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:ec6b3505bf01f1bdcd96d7f858771ad6e53c16075defda5d8046c83998c3a251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats@sha256:85fc53257b869566352af427b00b1e4eb3be4d9c158473d05955a95358569c49
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107420117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efad7f25530c39976e06f9cd49e8bf8ccf60e961cf32e240771c3311fa8ecb24`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 17:03:08 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Wed, 10 Nov 2021 17:03:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Nov 2021 17:03:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Nov 2021 17:03:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Nov 2021 17:03:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd8a5c6e6a53ddd4f3cdd7ae34bbe9c780fe53c7245304716909425bc26f7bb`  
		Last Modified: Wed, 10 Nov 2021 17:06:31 GMT  
		Size: 4.6 MB (4630764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7360e968604c4d5db8c901e6f52100633b1b227a9ac4c29b0308c424910d02`  
		Last Modified: Wed, 10 Nov 2021 17:06:30 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c245f1add19193bc4fd407354089b6c244fe2d37ea9a0c7f3b55c4cd0abf678`  
		Last Modified: Wed, 10 Nov 2021 17:06:30 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4949fe8ad7bd6aa73121e77f2feb4a983ddb04e9a8b68110350fe11533fd556`  
		Last Modified: Wed, 10 Nov 2021 17:06:30 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5345772ce5a94a4d4b36bcc445defff481e83b2af0be6506b3bb8865ef9de4`  
		Last Modified: Wed, 10 Nov 2021 17:06:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
