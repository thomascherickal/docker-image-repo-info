## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9666436fc76ec939ffd8388a57f2593c71da1654a685edcf7f42e4f738221ad4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
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
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
