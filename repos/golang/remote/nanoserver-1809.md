## `golang:nanoserver-1809`

```console
$ docker pull golang@sha256:ea4dffd70c0bf4983ccc984cc3758afa662c484db416b956bd7725d8ae448703
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `golang:nanoserver-1809` - windows version 10.0.17763.2686; amd64

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
