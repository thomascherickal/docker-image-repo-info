## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:3deb3e84ece2e334a28e4b46853567baf661fb0d6e9965cb297783565c5c96c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull nats-streaming@sha256:e5a5c9eee1f4f76f236ebf6a7049dd1956e9db04ae49b2b50c960eb7b51bfb17
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110458174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86f5bfb309b8634f75a1184a8b349dc72fbe6750e195fa87c4ee3b7220ebc253`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 Jan 2022 22:25:06 GMT
RUN Apply image 1809-amd64
# Wed, 12 Jan 2022 15:13:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Jan 2022 16:36:12 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 12 Jan 2022 16:36:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Jan 2022 16:36:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Jan 2022 16:36:15 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3a78847ea829208edc2d7b320b7e602b9d12e47689499d5180a9cc7790dec4d7`  
		Size: 103.0 MB (103031066 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db05d2e76671d91772a070867bf6f050343319070602a0f8239706d5d4d98387`  
		Last Modified: Wed, 12 Jan 2022 15:14:49 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d32b598636a5d24f0e2fed2dcea425de4fb29e48ffe747b16de7d34ba96d44`  
		Last Modified: Wed, 12 Jan 2022 16:37:10 GMT  
		Size: 7.4 MB (7422473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655251a8c00e62468ac138e6498ed5003026017f9e3aaa8a0890c8e4573e3e5d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce1684628b1c7cadb6b52866c3be12d063636d962797df7454acc55806596d`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489b687ddd94c7a64a680862d4341e41ad8fd93a41455a22da84feac26690169`  
		Last Modified: Wed, 12 Jan 2022 16:37:02 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
