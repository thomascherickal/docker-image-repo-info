## `mongo:4-nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:e5fc4eb602fc16349bd00e4f84139c866b1e4d0df19aea9cccca7d4d6120e579
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `mongo:4-nanoserver-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull mongo@sha256:a8ec9b93d08bca940c8f9b46a219d58cf208a5ec007ca1a559d7f184c8bc92b6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.5 MB (360529842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:012b33ee3a71519ef8ca5dc04c2e1f0474f927fe33aff93d1b1d1508bbd8d8ae`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Mon, 04 Jul 2022 17:25:17 GMT
RUN Apply image 10.0.20348.825
# Tue, 12 Jul 2022 19:39:12 GMT
SHELL [cmd /S /C]
# Wed, 13 Jul 2022 16:28:24 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 16:28:48 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Jul 2022 16:28:48 GMT
USER ContainerUser
# Wed, 13 Jul 2022 16:28:50 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 13 Jul 2022 16:35:10 GMT
ENV MONGO_VERSION=4.4.15
# Wed, 13 Jul 2022 16:35:33 GMT
COPY dir:11442d39c1a8be57a2edf36307e3c0f90a74de72a5c1c7d47a958b8e789a5794 in C:\mongodb 
# Wed, 13 Jul 2022 16:35:47 GMT
RUN mongo --version && mongod --version
# Wed, 13 Jul 2022 16:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Jul 2022 16:35:48 GMT
EXPOSE 27017
# Wed, 13 Jul 2022 16:35:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3719b23d309b17276277110a008a58133c9fc92465d2519f2f32c9961c39887d`  
		Size: 118.0 MB (118046090 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:86ff096ef8c908f52d6e505ea5d69c2a28332387f40883a0d9a119dfbf999132`  
		Last Modified: Tue, 12 Jul 2022 20:22:56 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90852679a7cbb8c1d1ba917e286f6665947318d28c2751e88db8f7fab20149b`  
		Last Modified: Wed, 13 Jul 2022 16:52:58 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4bfb15c0d978be52a798be5e90b31d8a3969ac275da1fc925d611e8bb16157`  
		Last Modified: Wed, 13 Jul 2022 16:52:56 GMT  
		Size: 77.5 KB (77547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36d2940b52cfaed8cb958f5c87253d43bf2c3fbae377411947b5cc7eba86aec`  
		Last Modified: Wed, 13 Jul 2022 16:52:55 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d926b36ade9a3dd6582f243e745b49184363f19a1e1085aafad96c60f2caf8`  
		Last Modified: Wed, 13 Jul 2022 16:52:56 GMT  
		Size: 263.4 KB (263437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3259b4854970608ac709ea7fca90df633a5121c23d26cb83a36967c5800623`  
		Last Modified: Wed, 13 Jul 2022 16:57:05 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aedeb4f36c7328e41521de8cb0ba41f1dc4d1021b80ae626719fbeb3bb433f1`  
		Last Modified: Wed, 13 Jul 2022 16:57:44 GMT  
		Size: 242.1 MB (242081636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6308efa284bb9ff1da9af5d43d9a9472a181882cc837ceb6c290a1675c4758c`  
		Last Modified: Wed, 13 Jul 2022 16:57:02 GMT  
		Size: 53.0 KB (53024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de6af75774b8b3933505ed490a6517e03c23e148fd109b8c8f3704d6c281ab6`  
		Last Modified: Wed, 13 Jul 2022 16:57:02 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ef1d605f3b64b52af18caa3b8ac964a685f41b51c23e90a26e69f150a30c0c`  
		Last Modified: Wed, 13 Jul 2022 16:57:02 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd66d63f78bc5bda6376a493682c851c839fcac9b2182fc8e1e971d3221aed8`  
		Last Modified: Wed, 13 Jul 2022 16:57:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
