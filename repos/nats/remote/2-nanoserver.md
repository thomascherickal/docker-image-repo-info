## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:1507f0f2963897740a12da7508fd1bc6ebea7ebdad76eb111d235fb15a1a7f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
