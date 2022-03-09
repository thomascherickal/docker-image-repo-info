## `golang:nanoserver-1809`

```console
$ docker pull golang@sha256:88b65d0444a48b289e3b30d9022b4fe7812d3b14a093f9e0bdf1ce0f35dd618c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `golang:nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull golang@sha256:6f551b5ba4ccdb6c7cea2bfdfdaf709d39da2064a890f0a3b15fc3159ae4be50
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.4 MB (248368258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e221206f673b55c742a25afbe92abf2818c439bae7fa9066f3a6f129d965fc50`
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
# Wed, 09 Mar 2022 13:41:51 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:44:03 GMT
COPY dir:30287e5480cb94d00aba798bdf22cad49bb2ae2de25f97441d1d8401e0571f4d in C:\Program Files\Go 
# Wed, 09 Mar 2022 13:44:47 GMT
RUN go version
# Wed, 09 Mar 2022 13:44:48 GMT
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
	-	`sha256:6635846d9875ca04e252ddfb880fcce12e3df79234c8f515edaf83ffd2cdf199`  
		Last Modified: Wed, 09 Mar 2022 14:16:12 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1144d4b651366d6e45abdea14cae59c2b943da5581c22ad9474664907ad83b15`  
		Last Modified: Wed, 09 Mar 2022 14:18:51 GMT  
		Size: 145.2 MB (145193081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0894c9938292fb93ae302dc717c95908010613c61787d65575195dbe5e5260`  
		Last Modified: Wed, 09 Mar 2022 14:16:12 GMT  
		Size: 42.4 KB (42392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8da05f0255d93d35026c1d0282b73cd5734ba16b73701cf46e422a3bd138a3`  
		Last Modified: Wed, 09 Mar 2022 14:16:12 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
