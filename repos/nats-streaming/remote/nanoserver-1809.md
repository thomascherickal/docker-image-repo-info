## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b661b1af7d63f50e0550e23204e3a544e5c351a613a832386aee365bcce484d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull nats-streaming@sha256:2f645551c661a9bdfa1f098de630c345560b42b46ea4f86e4358496fdb7e2c44
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112283602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6811dea88de0d1562552c6c359244361ee425743d9227dd15ab5dc36b22a88f1`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 05:08:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0e2c8ba21e47adc90962b46928c928315462bcddaefcbc01f98113f4f66cda4a in C:\nats-streaming-server.exe 
# Wed, 13 Sep 2023 05:12:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 13 Sep 2023 05:12:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 13 Sep 2023 05:12:34 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9930674eb6676a1690e63a275d0da517ab8b8aeab7ccd20591f76f7c69a5`  
		Last Modified: Wed, 13 Sep 2023 05:08:48 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b636690ea2cc8ecb38fcf9cec506c8c908ffe8096160b8549693ae2b6d1aab6`  
		Last Modified: Wed, 13 Sep 2023 05:13:10 GMT  
		Size: 7.8 MB (7786448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b0f65c350b20f8ac4d372a7e811aff70b8dbcba45d5850be6e80259d1c8544`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e9541dcd4167889f09d7139f64341ad22ff535be6578fbc55b09600bf8777`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e99090f84ed38c5eac15db96cb5f1e79ff34ddf90739902a0e20c7c5a49280`  
		Last Modified: Wed, 13 Sep 2023 05:13:08 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
