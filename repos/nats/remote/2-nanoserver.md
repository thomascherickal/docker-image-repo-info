## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:c191c7461bc7697ee6222d70680b57a59fdbaf1781a32102ae29004c0ef2e1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
