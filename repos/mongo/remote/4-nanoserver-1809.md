## `mongo:4-nanoserver-1809`

```console
$ docker pull mongo@sha256:18a903bfcb4fb09d4d0fe51cffdfac7638e1bf9e2448a6809ca07c92ad26f88f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `mongo:4-nanoserver-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull mongo@sha256:b1342f5268781f4203846e06c66a440ca5bbbedef41d4e0671e1a44b71e939d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.7 MB (336682072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a416a7a40f626cb66657169b4901708bc4eb533a7226395d324721e5e548e13`
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
# Thu, 30 Dec 2021 19:27:24 GMT
ENV MONGO_VERSION=4.4.11
# Thu, 30 Dec 2021 19:28:34 GMT
COPY dir:ac3dcf0e6bbeecc23af1858c2ccb3c1b4355678709a4966921cec081dbebc530 in C:\mongodb 
# Thu, 30 Dec 2021 19:28:48 GMT
RUN mongo --version && mongod --version
# Thu, 30 Dec 2021 19:28:49 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 30 Dec 2021 19:28:50 GMT
EXPOSE 27017
# Thu, 30 Dec 2021 19:28:51 GMT
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
	-	`sha256:0545a4ee04f69b88ed8f2b5d7df51034e75c532aec172eda427366a609b390c0`  
		Last Modified: Thu, 30 Dec 2021 19:42:36 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9126c5dabd56984fd8f530daef79f206e37bb89cb9aaddb4eb81919e2b7ddcd`  
		Last Modified: Thu, 30 Dec 2021 19:43:15 GMT  
		Size: 233.4 MB (233371695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b314bd1f57378b993ebce2cc58d01ac5c28ffaf9d312093b6e4cc520430bf35a`  
		Last Modified: Thu, 30 Dec 2021 19:42:34 GMT  
		Size: 49.3 KB (49270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee62abdfa9a6496b7b67597de1e30ca06257301af7a731c850f6f1104609087`  
		Last Modified: Thu, 30 Dec 2021 19:42:34 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64932f02e7c7262108874876500f8d8ddd2d81f99076073397a3da511c38901e`  
		Last Modified: Thu, 30 Dec 2021 19:42:34 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef859b8192c7cf348f569c327aa6342e1ac3e2b3cf838c44067f0c267cf39f8`  
		Last Modified: Thu, 30 Dec 2021 19:42:35 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
