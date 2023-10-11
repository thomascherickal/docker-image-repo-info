## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:d2017f7731ec6420f52e2633c4567934fc67c6b1466820f14cf57a737f77433c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
