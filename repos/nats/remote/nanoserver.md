## `nats:nanoserver`

```console
$ docker pull nats@sha256:8f26c87d964b3426a16e546857fc7873a8acc6ee97786a9366744ae849a4825d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:b69aaf3d5200a1cb93e65a79acaa950d17ee0b0e88be899c4c3ecd6695cf9529
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111704287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f827f381afa49f7b9d69a162222472931dd2aad1ebbac2b60a8155e798028`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 17 Nov 2022 20:19:19 GMT
RUN cmd /S /C #(nop) COPY file:d6b547504effc3514ee13384db156b8c7df287eadd44c86f4e5f5eabb6646c1d in C:\nats-server.exe 
# Thu, 17 Nov 2022 20:19:20 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 17 Nov 2022 20:19:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 17 Nov 2022 20:19:22 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5d7747e73374a2c02473deb4bde157dddb2835cb5e66800cfba5842c1fd88`  
		Last Modified: Thu, 17 Nov 2022 20:20:12 GMT  
		Size: 5.0 MB (4974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d427408549420b1666d1a85d3ff1bd3132f4e61dd9a7bd4e75a7c5adc32ee`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4682e51d5cc8bfadb600b57559df30d236b94223a5e9b1c3d2468f6acb1ee3f3`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8223b92ce81db067bb8ee9eacbf53e251b0dcd29dd1af6aa3a519768f0a7b44b`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f050378e256630049566bfcc0cf782533a8f961bcae8b6d9421ef19a8a780f`  
		Last Modified: Thu, 17 Nov 2022 20:20:11 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
