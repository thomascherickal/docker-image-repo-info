## `mongo:4-nanoserver-1809`

```console
$ docker pull mongo@sha256:b51bea8de3062d731049f1e9d9188bd6f4dbf0b68f135442f2196db8df2ce310
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `mongo:4-nanoserver-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull mongo@sha256:acc93a5a7355fa233a103eb4fa664818dcdffeb4709858fb3df1f52fc9b1daed
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.3 MB (349346149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6191750ff53dc9233e3f70185b22d2a948a3ce60521cfb4ef2239a9a3267ad6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Tue, 12 Dec 2023 23:48:09 GMT
SHELL [cmd /S /C]
# Wed, 13 Dec 2023 01:03:37 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 01:03:49 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Dec 2023 01:03:50 GMT
USER ContainerUser
# Wed, 13 Dec 2023 01:17:44 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 13 Dec 2023 01:28:15 GMT
ENV MONGO_VERSION=4.4.26
# Wed, 13 Dec 2023 01:28:33 GMT
COPY dir:c994cd7865d1b394f7e8a8c4a110ab2ce4ac2888cb8ffc9938a14314ee791f72 in C:\mongodb 
# Wed, 13 Dec 2023 01:28:45 GMT
RUN mongo --version && mongod --version
# Wed, 13 Dec 2023 01:28:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2023 01:28:46 GMT
EXPOSE 27017
# Wed, 13 Dec 2023 01:28:47 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9220949774e2034b6ae56093a689807cead41d7e03c112bf212d6fd6ffc3451`  
		Last Modified: Wed, 13 Dec 2023 00:06:17 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c8f290e0a52b1a1207bbc16c42a49bc83e084bceed3092c33b15e46934249`  
		Last Modified: Wed, 13 Dec 2023 01:35:09 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe19dabfcc726b3c17c7b578b312c3a55079210aa312af4e7442f43135bc464`  
		Last Modified: Wed, 13 Dec 2023 01:35:07 GMT  
		Size: 69.1 KB (69055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5f0fee4d518cae1fc80b12a10357bcc04b4d37e8f5ebf9692fb09f7cbf93bc`  
		Last Modified: Wed, 13 Dec 2023 01:35:07 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba085fd3eb484095b1b2d19aaf6c1a218fc58651af0287fbc88915dd21a4677`  
		Last Modified: Wed, 13 Dec 2023 01:45:52 GMT  
		Size: 263.4 KB (263439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56247f7f467e44ea72cd14f42e4631b2a0cc70e2c8201328826f6e2b203e3ad5`  
		Last Modified: Wed, 13 Dec 2023 01:53:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ee54a8489a0d971fa25528e1dbc292cf2046890ad08fe5348a6612a07e45f1`  
		Last Modified: Wed, 13 Dec 2023 01:54:25 GMT  
		Size: 244.4 MB (244413698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c569788d3bbab5bd3b026bf741bde8ddb01c5cad857ffc241f6043cce5dc72`  
		Last Modified: Wed, 13 Dec 2023 01:53:34 GMT  
		Size: 81.9 KB (81857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2f28caa193d48846c66100494857998e4bf1bd06e9aa7ac1ecee2675cafcad`  
		Last Modified: Wed, 13 Dec 2023 01:53:34 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa9dc4052c2149d92d312419b8a9a0195b4e8b3d37c621a5ab4fe3c13b5c44`  
		Last Modified: Wed, 13 Dec 2023 01:53:34 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c331eb3232a3b34c571bfcfc73df066c177521a4218f9f07cbe19d6c2881aeb`  
		Last Modified: Wed, 13 Dec 2023 01:53:34 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
