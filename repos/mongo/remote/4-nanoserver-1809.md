## `mongo:4-nanoserver-1809`

```console
$ docker pull mongo@sha256:9fbe736c213fdcc346fa1651bce6c29528207330fb62bd351c14156f2c5d53ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `mongo:4-nanoserver-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull mongo@sha256:ca8d70a9075d5ed658ffd04768bc23af1ebe206d8bb49522ac5371bcdc8f4e44
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335960307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5b95a186be291ff0f55d2cbfeb50d564e023b82cab0155e9fa329b9b6337d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 00:33:50 GMT
SHELL [cmd /S /C]
# Sat, 18 Dec 2021 08:16:34 GMT
USER ContainerAdministrator
# Sat, 18 Dec 2021 08:16:47 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Sat, 18 Dec 2021 08:16:47 GMT
USER ContainerUser
# Sat, 18 Dec 2021 08:16:49 GMT
COPY multi:0196f9e96f60ad3e2b92fd0773f8d0fe3a8235e1eefbb9ef1a1f0d672e6a711c in C:\Windows\System32\ 
# Sat, 18 Dec 2021 08:34:41 GMT
ENV MONGO_VERSION=4.4.10
# Sat, 18 Dec 2021 08:35:07 GMT
COPY dir:38b7137ed0744364da7d2052947e6bc819b65de66682c9d7639e51a11bc90cfa in C:\mongodb 
# Sat, 18 Dec 2021 08:35:52 GMT
RUN mongo --version && mongod --version
# Sat, 18 Dec 2021 08:35:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:35:54 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:35:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dac80fcd8aee90ad8a9145e0685b7c90d701307507ff32ffed6c86abc09c0f7a`  
		Last Modified: Sat, 18 Dec 2021 01:24:07 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ecafa7fdca0a8d9bbb541c6c503af8429d2b056d7ef10720fb63ee2ccd99df`  
		Last Modified: Sat, 18 Dec 2021 09:16:03 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1d19af80dba399d3a20765b575762747430f0cf5cc5d89e269a3a453340d26`  
		Last Modified: Sat, 18 Dec 2021 09:16:02 GMT  
		Size: 75.0 KB (75014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6472f76c36dc4c357b0583bd0592fee8c1568824ca166f1c8dbd66ad4c3cafe9`  
		Last Modified: Sat, 18 Dec 2021 09:16:01 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801875e2c17752512e14d76ddbedcd4b5b966101d38861c26a2567cc67f5282f`  
		Last Modified: Sat, 18 Dec 2021 09:16:01 GMT  
		Size: 274.1 KB (274067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6e8c449c5fd0d3fd413a4e606aa94e4c0b45c4471a918eb31d244d1307c247`  
		Last Modified: Sat, 18 Dec 2021 09:43:16 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5e57a8d79d545b4ad25d02feac910a6e744da4be73f91e9d259d0399e61f47`  
		Last Modified: Sat, 18 Dec 2021 09:43:58 GMT  
		Size: 232.7 MB (232656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2b6b6e7425df3b2846425b310a233058e31842f1d4694f682514ec59efe13`  
		Last Modified: Sat, 18 Dec 2021 09:43:14 GMT  
		Size: 42.5 KB (42545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e6f2c9f06130c89869fd0280f2912e17e92a7781a6f4819fd247fdc3fb1540`  
		Last Modified: Sat, 18 Dec 2021 09:43:14 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3372a6aa3b9e070fcedf060f7deeceee46c17a26fd6160d5421fcead2b9fb0`  
		Last Modified: Sat, 18 Dec 2021 09:43:14 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935d3dcbf335a5411685a540dc2cc8b60854aaa4b784def86b83aba6f323c07d`  
		Last Modified: Sat, 18 Dec 2021 09:43:15 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
