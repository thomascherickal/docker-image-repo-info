## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:10cdbe8b77248b0dc115ccceaadeab601fd2645d6d141e56a6c660dabb9cb7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
