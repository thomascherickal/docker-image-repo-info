## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:e1cd08756767b3c71dd69e3a54e5c07795348788b1df3d08cc0e37df34774c85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
