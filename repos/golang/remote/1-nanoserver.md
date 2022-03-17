## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:83e65b2035c0808b38714f3fcbda6e973cf715a8c6454f491537b422e0b7bf78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `golang:1-nanoserver` - windows version 10.0.20348.587; amd64

```console
$ docker pull golang@sha256:cfa868368cb26e7c1606908bf71a54351a7bc18a046f93a590b1f624eb9cfaf1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.9 MB (269875451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf3ebaf0db73d743b7e52bdf15fabc19bcecb6d903485040dd804dbfaebe6af`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 03 Mar 2022 04:50:34 GMT
RUN Apply image ltsc2022-amd64
# Tue, 08 Mar 2022 20:12:59 GMT
SHELL [cmd /S /C]
# Wed, 09 Mar 2022 13:24:44 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:24:45 GMT
USER ContainerAdministrator
# Wed, 09 Mar 2022 13:25:32 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 09 Mar 2022 13:25:33 GMT
USER ContainerUser
# Wed, 16 Mar 2022 01:21:30 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 01:23:47 GMT
COPY dir:874a103db63a9fa676dcd78fb311ebca18b661eaa8675e8e40c550d80d033b7b in C:\Program Files\Go 
# Wed, 16 Mar 2022 01:24:56 GMT
RUN go version
# Wed, 16 Mar 2022 01:24:57 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:dad81795ce109a7e20ebf80ad31925797ed97f9ba2a559f13f96ce3be5ea712b`  
		Size: 117.5 MB (117485491 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1c729ab19fa1794c04e2296ab2468daa560c676da6b333af3a86d94c1dc68b9`  
		Last Modified: Tue, 08 Mar 2022 20:39:41 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d268713d049d728054e11cf9c9306338ca1897c15a787ceafe9ee0fd8e305ac`  
		Last Modified: Wed, 09 Mar 2022 14:07:14 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcf1bdf8d65a7c4fcaf57246cc53c3f7f2aec0d0bdda306af3ab88084aa45b7`  
		Last Modified: Wed, 09 Mar 2022 14:07:14 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5fcf8d11464dbc6517a2f7808ad6c5c02360e3412d6b2881e9d61ef4eb3154`  
		Last Modified: Wed, 09 Mar 2022 14:07:13 GMT  
		Size: 79.5 KB (79469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55a006dc03085816dbdd7b07c4c2b36eeabf1dab04daec03901643c6461746d`  
		Last Modified: Wed, 09 Mar 2022 14:07:11 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b786f0b22ed0c6bd852091d0d26ea47bdfa5d6e0b9b3f4e9e86ede4d48403166`  
		Last Modified: Wed, 16 Mar 2022 01:33:10 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0100426cf81f4bfbd6f6b9652536a6741122c61ced57cf8cbe2fb49c2b8bee99`  
		Last Modified: Wed, 16 Mar 2022 01:33:43 GMT  
		Size: 152.3 MB (152252075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a1d95ff736751c3a77dd9f05bcb3d6ac27827a4bcf3e55e8d696164fcaad0e`  
		Last Modified: Wed, 16 Mar 2022 01:33:10 GMT  
		Size: 51.4 KB (51422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbff9faf036634ee83e131a37f673fa43a32335993dd54e8957a0bb9050ac3`  
		Last Modified: Wed, 16 Mar 2022 01:33:10 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull golang@sha256:f5d00ce7452f7416bfe44d544f616e318f329cd823e23552b32f5b639532665e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.5 MB (255489585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa30ec5ca0fb084b5e2030010344c709b42681a91e76fa6aec00762fffb0eec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Tue, 08 Mar 2022 20:14:56 GMT
SHELL [cmd /S /C]
# Wed, 09 Mar 2022 13:28:42 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:28:43 GMT
USER ContainerAdministrator
# Wed, 09 Mar 2022 13:29:14 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 09 Mar 2022 13:29:15 GMT
USER ContainerUser
# Wed, 16 Mar 2022 01:25:14 GMT
ENV GOLANG_VERSION=1.18
# Wed, 16 Mar 2022 01:27:25 GMT
COPY dir:874a103db63a9fa676dcd78fb311ebca18b661eaa8675e8e40c550d80d033b7b in C:\Program Files\Go 
# Wed, 16 Mar 2022 01:28:13 GMT
RUN go version
# Wed, 16 Mar 2022 01:28:14 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f64bdb56c2b15796c35e920619553b18bea7fbac60e4268edd3d421d55630a01`  
		Last Modified: Tue, 08 Mar 2022 20:46:00 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb485da234231f6c6bc790bde2fac723c254138ec71b37c4c56ad4594a753bd0`  
		Last Modified: Wed, 09 Mar 2022 14:10:18 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee61cb95026b98532cb3261086dd5675ed1824b9319e31666fd3d1ada84685c7`  
		Last Modified: Wed, 09 Mar 2022 14:10:18 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d19946c7ffba7bc5b5c6bfa65f290bf4e72be9e69b7f9737cd37ee085ab1834`  
		Last Modified: Wed, 09 Mar 2022 14:10:17 GMT  
		Size: 71.2 KB (71193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da14b80823ca390f9514f846c4f1e8ffc5c7fe1f6880a3e0bac73dd271d57f`  
		Last Modified: Wed, 09 Mar 2022 14:10:15 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb8760b629abd0b68497e99c8ef0662b78963d6236137ab86caa2347f6d54e8`  
		Last Modified: Wed, 16 Mar 2022 01:33:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80dfdb22bc0b1b20d42f99cf6165006e90fddbbb556bfd423a4c8d15ce823a1`  
		Last Modified: Wed, 16 Mar 2022 01:34:23 GMT  
		Size: 152.3 MB (152316376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12abe9ddb8706d2b3d4b7fc541835bba8dddcc07ab62bd9cf914a789c5257ce0`  
		Last Modified: Wed, 16 Mar 2022 01:33:52 GMT  
		Size: 40.4 KB (40398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b79e0b39265d2dece1ab8b8da146e40c1c5ad619ca5e837cd404f83ed927cee`  
		Last Modified: Wed, 16 Mar 2022 01:33:52 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
