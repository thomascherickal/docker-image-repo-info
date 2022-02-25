## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:6e43eecf010598596b218f3800a6d052426d875695ead9cdbf074e0653772142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
