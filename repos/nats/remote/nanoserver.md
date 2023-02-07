## `nats:nanoserver`

```console
$ docker pull nats@sha256:cf75db15a7a309da40d820366d4ca9bbf4f39bc06a401a060ccbc7f0618eea1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `nats:nanoserver` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
