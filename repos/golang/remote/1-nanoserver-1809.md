## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:b266d191f85c7bf32025f105e9dc54e593de87adf6774d1e65e10ad506385f9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull golang@sha256:86251e55305d5be8582ea2b9d5abf6dd853d9636c8a725f90ae308c48c965465
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.1 MB (264142167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e83cd398d3709751b21f3a27f07b440e439e956e3ac329d59e0bca51c3ea6d86`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 00:31:01 GMT
SHELL [cmd /S /C]
# Wed, 14 Dec 2022 00:31:01 GMT
ENV GOPATH=C:\go
# Wed, 14 Dec 2022 00:31:02 GMT
USER ContainerAdministrator
# Wed, 14 Dec 2022 00:31:44 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 14 Dec 2022 00:31:45 GMT
USER ContainerUser
# Wed, 11 Jan 2023 00:11:37 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:14:06 GMT
COPY dir:10c8e524c1346a2fb1d71240899f8be8a5c84e42a02e32a993c68761bb742a41 in C:\Program Files\Go 
# Wed, 11 Jan 2023 00:14:26 GMT
RUN go version
# Wed, 11 Jan 2023 00:14:27 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb1e4df1760e3de08ff30de6fd3f3acf348399853dab1aa1632ed4080cd102`  
		Last Modified: Wed, 14 Dec 2022 01:14:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6778b951d29f9735989650092ed207db9277298447f0162c8fe059a79fd71d`  
		Last Modified: Wed, 14 Dec 2022 01:14:11 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43efe6d3eed8dae1f414ff88e3af891aec01f30a91dd6f08b331c5f276ea670a`  
		Last Modified: Wed, 14 Dec 2022 01:14:11 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f35dd05107084e8e2076914c92cca0fb4a6c3413651c7c6ef8187d37e9ba83`  
		Last Modified: Wed, 14 Dec 2022 01:14:11 GMT  
		Size: 62.3 KB (62253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83fe57fefeebabec45f4602b2bd5642b9f242f21a3bf51bdd8ba353b3128ae9`  
		Last Modified: Wed, 14 Dec 2022 01:14:09 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54bbc79a8e572836543200b15e8e703d40871993ff4ccc5888984d9954cd250`  
		Last Modified: Wed, 11 Jan 2023 00:37:15 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81eda9943b8670bc8727e9ee5851b3572cb82e03640091fd4252743d06f3af3c`  
		Last Modified: Wed, 11 Jan 2023 00:38:09 GMT  
		Size: 157.3 MB (157330633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf3affbee8301901abacfe04125c3094c54fdb138781ce629108db2eeef72e2`  
		Last Modified: Wed, 11 Jan 2023 00:37:15 GMT  
		Size: 71.1 KB (71143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c281614e24021f13fed3f24ad45a7111e085441ed5d805b0737abe351fc138a`  
		Last Modified: Wed, 11 Jan 2023 00:37:15 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
