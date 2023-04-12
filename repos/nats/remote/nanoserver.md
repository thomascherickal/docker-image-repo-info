## `nats:nanoserver`

```console
$ docker pull nats@sha256:1716e8fedea9b15759385f82c7c80d974a7a801afc4c2c28e1c21447f07f1f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
