## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:089f1003c28ef5e80a16a558155a581473b77e6d540a50934cc9d7fd5ca6a71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
