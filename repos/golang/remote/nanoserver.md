## `golang:nanoserver`

```console
$ docker pull golang@sha256:ddd8f8681696356ca3e5e71116f263bffbf360119bc482a05ed54dd2198fc74e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.169; amd64
	-	windows version 10.0.17763.2114; amd64

### `golang:nanoserver` - windows version 10.0.20348.169; amd64

```console
$ docker pull golang@sha256:1a97647de56314891ca14dfe270617a3260a5466866f441c4503ed1e1cd5b07d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.1 MB (263136020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2d60dfa06ca080fd96826b247613f820638d09c67b0e600a1b4ee6de2492683`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Mon, 09 Aug 2021 15:12:42 GMT
RUN Apply image ltsc2022-amd64
# Fri, 27 Aug 2021 17:29:26 GMT
SHELL [cmd /S /C]
# Fri, 27 Aug 2021 17:29:27 GMT
ENV GOPATH=C:\go
# Fri, 27 Aug 2021 17:29:28 GMT
USER ContainerAdministrator
# Fri, 27 Aug 2021 17:29:56 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Fri, 27 Aug 2021 17:29:57 GMT
USER ContainerUser
# Fri, 27 Aug 2021 17:29:58 GMT
ENV GOLANG_VERSION=1.17
# Fri, 27 Aug 2021 17:32:01 GMT
COPY dir:a4b8016d8a17f147686e30107c9536eb6c4ced133f5d4ff9ff6a955ddb12ce2f in C:\Program Files\Go 
# Fri, 27 Aug 2021 17:32:51 GMT
RUN go version
# Fri, 27 Aug 2021 17:32:52 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:ee7a9c9193e3d9bee1b6c8ddddddd5356aed50f77c78d18d377241f4aee6d676`  
		Size: 118.0 MB (117979975 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f2143d365d9cdff8a0ff31859c4cded47f9b327c98d54a1126ade4e276599bc`  
		Last Modified: Fri, 27 Aug 2021 17:40:59 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481cea4152a197d02d076ddd228ba624bc50a3d4546e92515de3dab1c5c71b4`  
		Last Modified: Fri, 27 Aug 2021 17:40:59 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2462a2273d227fc6be10a3982aea1d1bfb3735bad7db8efc812b8a2c1b67f432`  
		Last Modified: Fri, 27 Aug 2021 17:40:59 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633872037529b39e741a6db33e57e6ac1b41efdf9c3b20c41df06e0ac618eb32`  
		Last Modified: Fri, 27 Aug 2021 17:40:59 GMT  
		Size: 78.1 KB (78124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0c8dc9ead4e278de41cdb88b8d704b6ca75b99b8a14a0b253f3a586f7516dd`  
		Last Modified: Fri, 27 Aug 2021 17:40:57 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d497b7589d9ce42f037a1037438bfdba63f99590751905a5e74971ef1363c4`  
		Last Modified: Fri, 27 Aug 2021 17:40:57 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1d612be1ac34f794a663ab43a1fcb0b27b578560daf7da330df587052b7e99`  
		Last Modified: Fri, 27 Aug 2021 17:41:24 GMT  
		Size: 145.0 MB (145020260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ce7508fced81b2192b0f41f009b2e3c849367d8f0afaaffcb5eb5a1d4d5f35`  
		Last Modified: Fri, 27 Aug 2021 17:40:57 GMT  
		Size: 50.9 KB (50855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09490b5d0f5c1ed1e5ca324cd7043ae608f9560b50548fa984ca8d633df11cf`  
		Last Modified: Fri, 27 Aug 2021 17:40:57 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull golang@sha256:34c0cdc2c423df69a9cf44657755c7c851b2102cdf971a0cba233ed7a186c24b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.9 MB (247946892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:730b78b7a9460773d70ad0d23946641966eda5638a81bc3091264be3b72e2325`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 13:22:41 GMT
SHELL [cmd /S /C]
# Wed, 25 Aug 2021 13:22:41 GMT
ENV GOPATH=C:\go
# Wed, 25 Aug 2021 13:22:42 GMT
USER ContainerAdministrator
# Wed, 25 Aug 2021 13:23:22 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 25 Aug 2021 13:23:23 GMT
USER ContainerUser
# Wed, 25 Aug 2021 13:23:24 GMT
ENV GOLANG_VERSION=1.17
# Wed, 25 Aug 2021 13:25:31 GMT
COPY dir:a4b8016d8a17f147686e30107c9536eb6c4ced133f5d4ff9ff6a955ddb12ce2f in C:\Program Files\Go 
# Wed, 25 Aug 2021 13:26:12 GMT
RUN go version
# Wed, 25 Aug 2021 13:26:13 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:72633ba98485460151f22e8084221e58c46cf1423b1ae99cf70a91bcd409a2dc`  
		Last Modified: Wed, 25 Aug 2021 13:40:36 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc1785bd046b44f66be3015e99d1614dfb3fbea263af87621af6c6fc1b96f34`  
		Last Modified: Wed, 25 Aug 2021 13:40:36 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a258bd0b66f48ebdb249f95a06ec1e526732f04152f28f6c37461e9b4bc51454`  
		Last Modified: Wed, 25 Aug 2021 13:40:36 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94199995894240f334fa8f377f3cbb662ba200bf9e5118935fddb142c4281fde`  
		Last Modified: Wed, 25 Aug 2021 13:40:36 GMT  
		Size: 69.4 KB (69419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508d30dddb17b20007581400c3f93b7e660737cd97fbe5d1ffd899a12da06b06`  
		Last Modified: Wed, 25 Aug 2021 13:40:34 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b23b84d5c581b810b38d27e4bbc4b410405e14d9728d874297ac738a3dfc046`  
		Last Modified: Wed, 25 Aug 2021 13:40:33 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068524937e9f64756a527203fb0c4e2db7e19dbdabb145a64eb0e517bb3ffc69`  
		Last Modified: Wed, 25 Aug 2021 13:41:07 GMT  
		Size: 145.1 MB (145054059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3ae5d4a7fd3927e86a194ccf33e145d975033fba76ad1b200376ae3cc2c623`  
		Last Modified: Wed, 25 Aug 2021 13:40:33 GMT  
		Size: 75.1 KB (75083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b358f24b46c13b9baddf4f2b92f4addc5298060a5fc05e2fa1ffbc594334f33`  
		Last Modified: Wed, 25 Aug 2021 13:40:33 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
