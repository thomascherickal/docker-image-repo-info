## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:8407af82564828d613edb1e65aedfa7d022699303898c4c33b02f71106e85700
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats-streaming@sha256:8b058c3d2bf71043f26b6b58702562c13724bb5594ceebad3f49b4f539c3c227
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bedda8d4d57688f52e1b97404c0dd1ecd0d7823e3f5e07a6f0214ee01d7853`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 16:52:04 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Aug 2021 21:19:29 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Wed, 11 Aug 2021 21:19:33 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 11 Aug 2021 21:19:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 11 Aug 2021 21:19:39 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3aa4a9dea1e2eabb29e2100fd699f3e3acbcabd85f360a3799b2505a5f74e5a0`  
		Last Modified: Wed, 11 Aug 2021 16:57:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2422c6b202cf35a718dc80ef76006199902c019414449d929f2538d72106be7`  
		Last Modified: Wed, 11 Aug 2021 21:24:43 GMT  
		Size: 7.3 MB (7293397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1c9060adc003485accbb3848bb825c0b555a9e064d8ee4861937d781f4fb6d`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb7419f921a924ca580e9c32580b82f2748e7759754b74686a3778fd920843`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413188a47dae1e13011a4e6d4ef5a31f5e680e350820d0b968981bc816827aaa`  
		Last Modified: Wed, 11 Aug 2021 21:24:35 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
