## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:0b9646472a3d88906cae4468e64aa579ecc702b1abc87fbb09f9bbf4a8712665
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats-streaming@sha256:cfd77a52c292b4041cbb0a76a55f488d022224bb85271d9f92a8a4fc5c8f5fa4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111143785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f200df236cb835ed205e49e6d4fbcccf4922bb86621a3b84212afe6637b10b7`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 11 Oct 2022 23:18:05 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Tue, 11 Oct 2022 23:18:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Tue, 11 Oct 2022 23:18:07 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5ead999142ecce15e02523c49706a633fa708374d94bb65a254e3a3c117d609b`  
		Size: 103.4 MB (103377244 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3d4d61d6915ceca5246fbd620385fae02dbdc535a097c3aaf0350da86042b9`  
		Last Modified: Tue, 11 Oct 2022 23:18:51 GMT  
		Size: 7.8 MB (7762223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86779f9773546ae6441977745f02c8b15acce03afb229aeb57dac89c93b90b4f`  
		Last Modified: Tue, 11 Oct 2022 23:18:49 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6af5e059014bb8bacfed4a8002178e0b114a4e4a7ee13f910188094e20e3b8`  
		Last Modified: Tue, 11 Oct 2022 23:18:49 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb940ae6eabc5c3bd86a4b8566e1788bf84fb2687dd0fb027ce5b9cbb73fe80`  
		Last Modified: Tue, 11 Oct 2022 23:18:49 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
