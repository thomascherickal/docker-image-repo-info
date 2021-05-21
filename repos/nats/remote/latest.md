## `nats:latest`

```console
$ docker pull nats@sha256:e7196d68027c9d81fd783b689c81bd8f9ba32b400088c2a3652a606855530eb4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1935; amd64

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
