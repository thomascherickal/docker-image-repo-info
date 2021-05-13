## `nats:latest`

```console
$ docker pull nats@sha256:1e73835df48665074bbfe2d19c82563c6adc3ee0fcdd5b40a98e6722a3e9959d
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
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1935; amd64

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
