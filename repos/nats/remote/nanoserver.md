## `nats:nanoserver`

```console
$ docker pull nats@sha256:a51cf33b5a60f76e42ca151a63dcd64c5014d52741be152540b12678b5c5811d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
