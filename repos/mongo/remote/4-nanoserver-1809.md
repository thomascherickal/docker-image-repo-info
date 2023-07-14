## `mongo:4-nanoserver-1809`

```console
$ docker pull mongo@sha256:60bd24261117817b7efee14664291c6d4acfc18ed376ab42907267338d7741b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `mongo:4-nanoserver-1809` - windows version 10.0.17763.4645; amd64

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
