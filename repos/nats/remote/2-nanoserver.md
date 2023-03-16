## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:e37929e6e16e54eea197ddd116aab3e276eff98032095765851fb52f7a05dc4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
