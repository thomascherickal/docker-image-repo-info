## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:d2f7f2b6e7ef60042e06a03f94573e6aab5cd1f073f476f9efec62f527a59689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats@sha256:23c3043b7d852c7a960b62141f08843223754582d236eb2e9610b349c110ce30
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105104931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d94790e871ec07154936db07dcf840f87ed91dbe648823dd3ab3bfd35cee85d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 16:04:16 GMT
RUN cmd /S /C #(nop) COPY file:18561b827240029ad80d0e3d25142efae62905c30cc520fc37cfc68e7d889848 in C:\nats-server.exe 
# Wed, 10 Jun 2020 16:04:18 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Jun 2020 16:04:19 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Jun 2020 16:04:20 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550b5fdbee6a185b325bc673ac4059474353d34cc82ee5722edc4dca721c3c5a`  
		Last Modified: Wed, 10 Jun 2020 16:08:52 GMT  
		Size: 4.1 MB (4056494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ee7df3dace6c97838bc1bdecdff255d7e67bbec225868420ce6f188538c17a`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db8b53011d85727f476a78b4ad3a21cad54684c2ce7dac2011db5f3be7a2312`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9cac1f94d61b8883bdd4f0af6741b02ba9bb5df9bc58fa289e792f40f25310`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306722d16f58c9f328a577068e5aea75b105b9d09dc8ad19a48734418ee276b`  
		Last Modified: Wed, 10 Jun 2020 16:08:51 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
