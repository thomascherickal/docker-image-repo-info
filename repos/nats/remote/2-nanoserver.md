## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:cd72550bc0dc297ac0d40dc272ab9bc9cba7d2b51aa4ea87af8a8ceb00af4b9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:5f52c2aec4c9f9a92ae1e8e805a2ded0c1d8707d78b83f8fdf5c4a347716d1b6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108295170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30633d2cd44487d17f0c39e152e8b6dd7ae7365e88fcba7fafc7dda07775eeb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 15:41:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Sep 2022 15:41:38 GMT
RUN cmd /S /C #(nop) COPY file:58259134bc4aec3b0bb4a01151c496cd2e557bf985d41d1838cb10c3492958d3 in C:\nats-server.exe 
# Wed, 14 Sep 2022 15:41:38 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Sep 2022 15:41:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Sep 2022 15:41:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Sep 2022 15:41:41 GMT
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
	-	`sha256:379f80368def8337624f5e8a84b520751678f207da4a626cdf50cf3d7392f04c`  
		Last Modified: Wed, 14 Sep 2022 15:42:29 GMT  
		Size: 5.0 MB (4954549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acc7fb6dac7daaf12ea799fabe64082aa832976b80fee0dee151e228715c9d1`  
		Last Modified: Wed, 14 Sep 2022 15:42:28 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3594ed92c60a9025482778f60a98c08bdb781c381811612ab20748b21a5430`  
		Last Modified: Wed, 14 Sep 2022 15:42:28 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6012bd45501ace7b93d72b0d441a60aac54f5890ade1c8c669469a1adb820a`  
		Last Modified: Wed, 14 Sep 2022 15:42:28 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e87860897c14f00959ece616cd0716df15e5d22fdfe25eeb2d1c15f80b162a`  
		Last Modified: Wed, 14 Sep 2022 15:42:29 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
