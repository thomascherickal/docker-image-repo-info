## `nats:nanoserver`

```console
$ docker pull nats@sha256:347c71d5b7499fda4c79d015de6e2b9da4a28374147b6901e02f8e135e482bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:baec10f85f099b828313ff821f20b005907591e2f4fb414c7a240b5944f1292a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109785996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3654d1c2e7ef6e2297c519fd991a4a49b4d9928375a1142ec2af9cc55358ee84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 06 Sep 2023 23:17:32 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 06 Sep 2023 23:17:33 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 06 Sep 2023 23:17:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 06 Sep 2023 23:17:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43534c571f8fdc71038e0f4b4c33a30adb0bbc8b292454d35930557ced33408`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eade3f0d46f534a5d639c78b1e85a1b0ea96d271fe2c3e706142d2f8d0aef7`  
		Last Modified: Wed, 06 Sep 2023 23:18:18 GMT  
		Size: 5.3 MB (5320148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeab0b725b185bf02913419c636eb70964ad972b883ef43006bbf75b1320ece`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11e5f8af7811e39cecedb8bc4f4533b8f362e497bfe37a943209e0ce0d0bd5`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806fff52469c9a918b10aa2ed383885dd30e5763ab2157c5440e425ebdccd3`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8c118167fb4c0339d4078748da065ff698f06d9373f7acaa5c42db51dfcdff`  
		Last Modified: Wed, 06 Sep 2023 23:18:16 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
