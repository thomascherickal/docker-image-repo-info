## `mongo:4-nanoserver`

```console
$ docker pull mongo@sha256:f9223c11850fc4b6c7cdfc4725a0d6c097ce2c1d208a4c78af4e9ee33bf57745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `mongo:4-nanoserver` - windows version 10.0.20348.1850; amd64

```console
$ docker pull mongo@sha256:d3df2ae7310124c1b337a8ccf24594ac237e579769fa99fa0decf9a5f1300531
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.5 MB (365513111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb6d3ab06284c632dad49be59b549ccf7cad54104666caf9788d425490bacb3`
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
# Thu, 13 Jul 2023 23:20:19 GMT
ENV MONGO_VERSION=4.4.22
# Thu, 13 Jul 2023 23:20:41 GMT
COPY dir:ba7da3b127dd995e6b5f5a8e9cc5f87caa3174d8a03e6b82fdeaa7d4f4b54ce8 in C:\mongodb 
# Thu, 13 Jul 2023 23:20:54 GMT
RUN mongo --version && mongod --version
# Thu, 13 Jul 2023 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:20:55 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:20:56 GMT
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
	-	`sha256:f5703510071ac4efc5343e46fe31f41ad515d4c5453a02a0951736a17d334253`  
		Last Modified: Thu, 13 Jul 2023 23:56:28 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff60cd183b69212eba05d4bd324dd05ba8d74fd55a25abbc3f1e6500e91a0ad`  
		Last Modified: Thu, 13 Jul 2023 23:57:09 GMT  
		Size: 245.0 MB (245043176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36583dbbacdc0ab5c6374a49ddefd4dcf2eacbd27c9f1cf09c4e18b998bc38d9`  
		Last Modified: Thu, 13 Jul 2023 23:56:26 GMT  
		Size: 61.8 KB (61839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69c795c93a92387e50f843864b645f9686e69412657d7b9208790e155e38b3d`  
		Last Modified: Thu, 13 Jul 2023 23:56:26 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad0d23d01ba2a7392c8b56079fe542e457a91b58f524face0b95039842be066`  
		Last Modified: Thu, 13 Jul 2023 23:56:26 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa874083639e85f37d176f6f18d5924724fb6199a76fd25ced82d6ca3072a7`  
		Last Modified: Thu, 13 Jul 2023 23:56:26 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull mongo@sha256:5bf1bd69d3ff1f35446eb9114a06b3c60c14ac2eda15705e7d13f002ebfdd037
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.9 MB (349874339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4122809a59483ff7f3ab0040aa97fc30e598a712903736971bb74f6a4c1895d`
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
# Thu, 13 Jul 2023 23:21:04 GMT
ENV MONGO_VERSION=4.4.22
# Thu, 13 Jul 2023 23:21:26 GMT
COPY dir:ba7da3b127dd995e6b5f5a8e9cc5f87caa3174d8a03e6b82fdeaa7d4f4b54ce8 in C:\mongodb 
# Thu, 13 Jul 2023 23:21:38 GMT
RUN mongo --version && mongod --version
# Thu, 13 Jul 2023 23:21:38 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 23:21:39 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 23:21:40 GMT
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
	-	`sha256:f24f180e0535395602759ea6a1e7f12e1d9b8405505e684962538a0b74121f27`  
		Last Modified: Thu, 13 Jul 2023 23:57:22 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c0a1ac0b49e61fd8488d3ea54b7d1a0f2a91e5e00ff3e20b0a445e802e0429`  
		Last Modified: Thu, 13 Jul 2023 23:58:03 GMT  
		Size: 245.0 MB (245044651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1180729edf1ff50359185f89ba04e6c8c4d635c4c885a94a9e9a66a1308b5e04`  
		Last Modified: Thu, 13 Jul 2023 23:57:20 GMT  
		Size: 81.0 KB (81028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d87ffc799a67f7c83624c8f6f72477050cb9809a7b9be0b12a283858c0142bd`  
		Last Modified: Thu, 13 Jul 2023 23:57:20 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac1a5938a30219d4661207fec8740011048ea4ee9b552c3b15a94ae87bc5832`  
		Last Modified: Thu, 13 Jul 2023 23:57:20 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a3cc2fea3322f767ba0dab3db2b81f04b9159427b4da41844b713ad94d4b83`  
		Last Modified: Thu, 13 Jul 2023 23:57:20 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
