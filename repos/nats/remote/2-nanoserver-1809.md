## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:679b0d8e5bafa2c6893078adf595ebd301d9df9258ca22d088788c40d6ca5d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:2861931a21dd96bdbd1686faf3a14c6927dc24203b8c04d30b2116ef4d670e64
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108299212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc0fee332755f830a4cef70df70da46a2cb2c28daadd327e68b97dbf22b35166`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:18:47 GMT
RUN cmd /S /C #(nop) COPY file:da89208003aed19cb9852334329c2f8b4dfdfe3218c3f05bba8fcb3247acc400 in C:\nats-server.exe 
# Fri, 30 Sep 2022 00:18:48 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6bda313a93b8c355d5adf6e15f4b805f705c3741b235a7e4644bbffe6a6af3d`  
		Last Modified: Wed, 14 Sep 2022 15:42:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c046270960bff604e9be6498c1c0ee8367958198004e91286a8252366f7185c`  
		Last Modified: Fri, 30 Sep 2022 00:19:41 GMT  
		Size: 5.0 MB (4958572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087232c1623e24e6883cc4c33bb9ff4926cfc24df9f4909f09db53185f2fe15`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e77ee18b12423f469199b766a08c031324d15169a9f2e690bf77ccbb796ecd`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4549b9baa74eb7ff07539b979f0966c66afb35858810779ec9d7572da5777e49`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee9032ad08c565fc85469a687bbaddfa40a6066692a113da46c758c5d591e4a`  
		Last Modified: Fri, 30 Sep 2022 00:19:40 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
