## `nats:nanoserver`

```console
$ docker pull nats@sha256:285df485f8d2b409343b431afda5f6145cb9fc179ab79fdd2183bac4bf444540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:nanoserver` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
