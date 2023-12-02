## `nats:nanoserver`

```console
$ docker pull nats@sha256:cb6e962ac8351dd9c57425e277ee4df9a1891ceb36b91f96de71bcb32e5b7f74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:nanoserver` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:69a4fec7f771c424c06edd875a229e083dd25097b9bb34e625152f305284ccb0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110107540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e656d7f8cde6eaa8d68cbcb8f122eadcfb8bda9fefaf0850f0a5bd80d10746b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 01 Dec 2023 22:18:45 GMT
RUN cmd /S /C #(nop) COPY file:5822e02f9917394b0000f014548d93cd57cb360bcdf713fba371db474a65bde9 in C:\nats-server.exe 
# Fri, 01 Dec 2023 22:18:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 22:18:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 01 Dec 2023 22:18:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95140ae86e514b73c89e0e172c4fcd2e0afb3837246b19633c645730682adb73`  
		Last Modified: Fri, 01 Dec 2023 22:19:59 GMT  
		Size: 5.6 MB (5604103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabee63b67234b08d0dba7ee8e55507762a7a8283a94d9bd7a900777810c9ea3`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801c9c5c26b0bb09e73c30952bf8b26b775e6c0ae4f8645931c3be834ca56281`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba541071f125d7b8c9955e517d2c5010fd923689c139f6bed141577884530a52`  
		Last Modified: Fri, 01 Dec 2023 22:19:57 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611bc0dd56df7698801deb6cb1d0ee3927c7f156e34422ee15dfb7c88c13b762`  
		Last Modified: Fri, 01 Dec 2023 22:19:58 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
