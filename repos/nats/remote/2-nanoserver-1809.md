## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:63cbe4e8a745d068f30d1fc757f589ee984384dba70a21b06e599a3c503f3749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
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
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
