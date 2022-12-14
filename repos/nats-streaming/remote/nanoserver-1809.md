## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ab9236d137e3eebdb5117eca1e9d49e4d8f1a56d38b2db676b5be5c13ef89118
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
