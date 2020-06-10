## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:4792d4e20ea6c81b0ac635d43e69819f9be4d34fc40c91d82490c2b5ea6897ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:a9adf4a9f9b6d7d8e45250ebfc8920d5e59cb3952da294f1188188be46d3aa9a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107099276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e2df9f4f523b8789f991392b9a959dc7cbb3b6312b43f424c677a7403092b4`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 18:11:05 GMT
RUN cmd /S /C #(nop) WORKDIR C:\nats-streaming-server
# Wed, 10 Jun 2020 18:11:06 GMT
RUN cmd /S /C #(nop) COPY file:d30725f7225d14fba35e88513adf63da18fc9fef9c4f6c817dff8f784f19a7c1 in nats-streaming-server.exe 
# Wed, 10 Jun 2020 18:11:08 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Jun 2020 18:11:09 GMT
RUN cmd /S /C #(nop)  CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52122f0b557b9386642a061a7b0f3af4ad8510fae2111d614c72d5127229770`  
		Last Modified: Wed, 10 Jun 2020 18:11:33 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaafa96b5b099b4d3677a5e29b41df4b9577348f6e96744e69ab7022bdd5c0da`  
		Last Modified: Wed, 10 Jun 2020 18:11:35 GMT  
		Size: 6.1 MB (6052119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca5fd49956db2c1bca1ba34567206c6a39257cbb4961b93d896f3d5093ea100`  
		Last Modified: Wed, 10 Jun 2020 18:11:33 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cbb1f97d12145539ac19374975dcaf38df5ee933d4a340ef40fde2ed44c079`  
		Last Modified: Wed, 10 Jun 2020 18:11:33 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
