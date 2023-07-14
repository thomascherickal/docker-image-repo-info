## `mongo:5-nanoserver`

```console
$ docker pull mongo@sha256:7bb88140dc23b688de2e4be86bcf805d80eb9ea799c992e43686fe7896ace4fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `mongo:5-nanoserver` - windows version 10.0.20348.1850; amd64

```console
$ docker pull mongo@sha256:0b7935ce696507b408f2eda010a00bd71512f93a2930e177e63a9ebe5a50d7cf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.0 MB (433010063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce301a3e8dd292b1d758b7344de54802a32ee11b06163986f0ddfd601f627548`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 07 Jul 2023 21:00:40 GMT
RUN Apply image 10.0.20348.1850
# Thu, 13 Jul 2023 20:38:35 GMT
SHELL [cmd /S /C]
# Thu, 13 Jul 2023 22:41:28 GMT
USER ContainerAdministrator
# Thu, 13 Jul 2023 22:41:38 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Thu, 13 Jul 2023 22:41:39 GMT
USER ContainerUser
# Thu, 13 Jul 2023 23:03:40 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Thu, 13 Jul 2023 23:09:49 GMT
ENV MONGO_VERSION=5.0.18
# Thu, 13 Jul 2023 23:10:16 GMT
COPY dir:ab74dbf9ad27d2154a3f270894c5c95f10fe56a2d5ec4c1875a57c2afdba8cff in C:\mongodb 
# Thu, 13 Jul 2023 23:10:31 GMT
RUN mongo --version && mongod --version
# Thu, 13 Jul 2023 23:10:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:10:33 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:10:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:cc0a26bd90fcc4d863317c36d7ffec77a0a82a905697204d4dcbc76ec13b3920`  
		Last Modified: Tue, 11 Jul 2023 20:10:45 GMT  
		Size: 120.1 MB (120056465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262f95c9ffc2400b306c39bdd21ab1ee5e02c305fa1895921355e39b04ef5049`  
		Last Modified: Thu, 13 Jul 2023 21:09:57 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c68dafb672cd72b022af598465e06fd23042d9e29348ccc200530e5b35d9bdf`  
		Last Modified: Thu, 13 Jul 2023 23:27:03 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1171b244f6f6515a32b709bf3ce287a50845db3a64ddc64026d75947c2af63`  
		Last Modified: Thu, 13 Jul 2023 23:27:01 GMT  
		Size: 80.2 KB (80237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943c2ea6e887132d6348c7c470e1eb8c8f31d8de00201b789ae3683c1d616638`  
		Last Modified: Thu, 13 Jul 2023 23:27:00 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ee32a4b650d1a8c59877c26864f499651e23cebe4c8258dd847dc3c8748ec3`  
		Last Modified: Thu, 13 Jul 2023 23:44:30 GMT  
		Size: 263.4 KB (263369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2c86261ed286153f0b83826b26c9422769e7dbc78fbfca52c528f57a7144b`  
		Last Modified: Thu, 13 Jul 2023 23:48:57 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836ead9022a197cc846944a295d787336565e6853b292ca6da52cdd49571b633`  
		Last Modified: Thu, 13 Jul 2023 23:49:50 GMT  
		Size: 312.5 MB (312540297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc9cd4cb485668c706c63f65e53d8451a4ad6d3d234c061e7e1e9b4be9925fb`  
		Last Modified: Thu, 13 Jul 2023 23:48:56 GMT  
		Size: 61.6 KB (61639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9061d76bc88e43d79fe75fd76d346b980666f5c9159dbafe72e03c127cfda6bf`  
		Last Modified: Thu, 13 Jul 2023 23:48:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debfaabf43fe35aa1142237c1765fb8515732b7bfc3cbc201fe7f7245b554af9`  
		Last Modified: Thu, 13 Jul 2023 23:48:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa5f1e8875d580cf5dad36c126103981586e9f5067fc1c8b9c97b10e1f42b4e`  
		Last Modified: Thu, 13 Jul 2023 23:48:55 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull mongo@sha256:6b7d7337cbc18cefe684c55e70a18ba2358f7cc6ae5f2e3adce0b23464e9760d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **417.4 MB (417365289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b16dff5b3dd464f40f6489391b594ebb775e204d86279796eafe3e1e142a67`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 20:41:18 GMT
SHELL [cmd /S /C]
# Thu, 13 Jul 2023 22:42:56 GMT
USER ContainerAdministrator
# Thu, 13 Jul 2023 22:43:04 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Thu, 13 Jul 2023 22:43:05 GMT
USER ContainerUser
# Thu, 13 Jul 2023 23:04:43 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Thu, 13 Jul 2023 23:10:42 GMT
ENV MONGO_VERSION=5.0.18
# Thu, 13 Jul 2023 23:11:07 GMT
COPY dir:ab74dbf9ad27d2154a3f270894c5c95f10fe56a2d5ec4c1875a57c2afdba8cff in C:\mongodb 
# Thu, 13 Jul 2023 23:11:18 GMT
RUN mongo --version && mongod --version
# Thu, 13 Jul 2023 23:11:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:11:20 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:11:21 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48271163dd58fddb2ff623ae3c53cac64a29148ad84e995c93073602f68793d`  
		Last Modified: Thu, 13 Jul 2023 21:10:35 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25653f1b79488d51860f4c39a7b5cb89dcde67e655debe7f7c2175ac330de2c`  
		Last Modified: Thu, 13 Jul 2023 23:28:43 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9847941203abbe97818feb1f724af0fd19021fcdc2b4bed652803609b6ee4a8`  
		Last Modified: Thu, 13 Jul 2023 23:28:41 GMT  
		Size: 68.8 KB (68839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257289d6eacacb75cbf84765b6355a008ee35bdf481b5b2b7989bbb19502ddb7`  
		Last Modified: Thu, 13 Jul 2023 23:28:41 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5546df12599902e639126688271cc1e2eedf2cb07fee83cfc7c18ac2bdb8bba`  
		Last Modified: Thu, 13 Jul 2023 23:45:35 GMT  
		Size: 263.5 KB (263502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8b34dccf548a9924a4baa7b489de45d5d4b6ffd2e729c7dd71f3cfb6ef9d0a`  
		Last Modified: Thu, 13 Jul 2023 23:50:04 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f11d086b405fd04c5910f63f37288f6ead45df1b610cb6f1770f75b737b5c`  
		Last Modified: Thu, 13 Jul 2023 23:50:56 GMT  
		Size: 312.5 MB (312540301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a96c93027aedc70e556d08c885e8c3b382abb9b85df586f8dec47f7da8ea984`  
		Last Modified: Thu, 13 Jul 2023 23:50:02 GMT  
		Size: 76.3 KB (76336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595f1c6797112004e5e37f2ab123324f908440bc95ecefa413e8816e2b285226`  
		Last Modified: Thu, 13 Jul 2023 23:50:03 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74f897eac1cb7558ab7e041e3f84449f0640c259763aa841fd60f1ab7f9c7d8`  
		Last Modified: Thu, 13 Jul 2023 23:50:02 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac5d90cb4b9244e0b7d6a02d127a9273b7e1b023e3eccf0ef03c116e0351b94`  
		Last Modified: Thu, 13 Jul 2023 23:50:02 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
