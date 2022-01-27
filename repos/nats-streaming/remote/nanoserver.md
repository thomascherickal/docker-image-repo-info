## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:0bc54aed3d2e2459da32d7ef1a3164f6821554c52b87b1db08569eb3d4b83f61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:eba70e379f9ea1b23ec39a50e5389c381ebe084c632d1380eb8b50ec3e21e413
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110473642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21115b3d09cc52d655a15be1f0aef76f5df080bd9e05acda454342d454fe1b1c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 21:09:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Wed, 26 Jan 2022 21:09:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 26 Jan 2022 21:10:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 26 Jan 2022 21:10:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c1311cca68ba5a001257a3edb06ee2e37445ce0e3765a3027d2f33fb903427`  
		Last Modified: Wed, 26 Jan 2022 21:13:49 GMT  
		Size: 7.4 MB (7422486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df89cb2a6909f60696257a2dfef3c88878b6609f3773db8f592c27796660f42`  
		Last Modified: Wed, 26 Jan 2022 21:13:46 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4fd3978f80bc4ceed281702ec49a0b9ad7196848dde5c70f4393e311380480`  
		Last Modified: Wed, 26 Jan 2022 21:13:46 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9d1ed600dbd9fa469dc611820c4fe1388f306ad3dd87140b9ee960450d292a`  
		Last Modified: Wed, 26 Jan 2022 21:13:46 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
