## `nats:nanoserver`

```console
$ docker pull nats@sha256:59e153a1f1aef558eaa9de625d2f78b899eb4a4d7fc364c1aaae197da3bea34d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `nats:nanoserver` - windows version 10.0.17763.3046; amd64

```console
$ docker pull nats@sha256:5296a47c0b8acbd64b0ac15fdd8c58c4cc732ed86f9e15d51cb3b9efe3874e61
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107793012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd46a9a6be0e2987044c53968e1c52f5c3ac67c4e7880073056d7d551d97767f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Jun 2022 19:20:11 GMT
RUN Apply image 10.0.17763.3046
# Wed, 15 Jun 2022 16:58:11 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jun 2022 16:58:12 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 15 Jun 2022 16:58:13 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 15 Jun 2022 16:58:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 15 Jun 2022 16:58:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jun 2022 16:58:15 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d555a7e4de4dd775379d5c43c1419374bff7908670dc7444be5e8e8f386f3d26`  
		Size: 103.2 MB (103153235 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d50fad9fd53cbbc8472c6168de3c7729cebe33d6db42f0e3180a379903f746`  
		Last Modified: Wed, 15 Jun 2022 16:59:09 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7d26d1ac683260cce7cb453aa50ff0ec2a4b087794e4826eaa814529874502`  
		Last Modified: Wed, 15 Jun 2022 16:59:12 GMT  
		Size: 4.6 MB (4633293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449f49003f693f202a656945f5479122112a232b9b0eaf5099a003d09c1ca09b`  
		Last Modified: Wed, 15 Jun 2022 16:59:07 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb73c50fe3d2518ac2e175f67b9d0199ef7bdea515eb2b825180304bd931e20b`  
		Last Modified: Wed, 15 Jun 2022 16:59:07 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e1a325a6d94b12835c8d4878e07814b18798ea267695bd2304ad71c5cc7d0`  
		Last Modified: Wed, 15 Jun 2022 16:59:07 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd107651a3b669ae06a4f2374516b649bcdaba5a112bf95468d1db82774f5521`  
		Last Modified: Wed, 15 Jun 2022 16:59:07 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
