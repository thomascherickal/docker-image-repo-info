## `mongo:5-nanoserver-1809`

```console
$ docker pull mongo@sha256:7d7ceed2ed33893856b687e136f6f75a67f64eace8d8bdcd4e4d8e437b8696e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `mongo:5-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull mongo@sha256:a7756fce8da848d93bf87e05da2366a3c23e10bc8b724824810fb1eed0643766
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.5 MB (412485433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:006c1c5dc5c31c2a0eef5a0033b35f2433913a6612108ba0cc16a91cc921b33e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 13:03:35 GMT
SHELL [cmd /S /C]
# Wed, 14 Sep 2022 18:18:09 GMT
USER ContainerAdministrator
# Wed, 14 Sep 2022 18:18:21 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 14 Sep 2022 18:18:22 GMT
USER ContainerUser
# Wed, 14 Sep 2022 18:24:40 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 14 Sep 2022 18:24:41 GMT
ENV MONGO_VERSION=5.0.12
# Wed, 14 Sep 2022 18:25:07 GMT
COPY dir:1f61faf303cd820ab7433128927f1aecf4a58f41aaa7c480a9fa473802fcc6c6 in C:\mongodb 
# Wed, 14 Sep 2022 18:25:21 GMT
RUN mongo --version && mongod --version
# Wed, 14 Sep 2022 18:25:21 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Sep 2022 18:25:22 GMT
EXPOSE 27017
# Wed, 14 Sep 2022 18:25:23 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0668477bacdfc2e7df1cd4268b246175ed9b30cf07ccb4bcfcb258d8bee830e`  
		Last Modified: Wed, 14 Sep 2022 13:26:19 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ada06039b3dceb53c91ed6d7bd2d77d0abd90acba1883744d947d1ccee8349`  
		Last Modified: Wed, 14 Sep 2022 19:03:38 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d170c6bf2fd2a53a952e69b17f97ce92dd39dd7294e4b1c6ae6e11adc613210`  
		Last Modified: Wed, 14 Sep 2022 19:03:36 GMT  
		Size: 69.7 KB (69673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d16b6830f5e893640af2e263523f5ff88334d46d1a2d69d91cddf1f70f62790`  
		Last Modified: Wed, 14 Sep 2022 19:03:36 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98574a2f866f60f51f05d43d7e4e9d7e62e346b27ff83266400261170b141e2b`  
		Last Modified: Wed, 14 Sep 2022 19:08:41 GMT  
		Size: 263.5 KB (263502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179b520da4f2a57b29004c74923dcb6980427843553f5d8b8faf3d2035c0c39b`  
		Last Modified: Wed, 14 Sep 2022 19:08:41 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49b9b90c4173398fdefab5fbfc4bf2b2e4515f67f75f2e9ecff97454b1ec894`  
		Last Modified: Wed, 14 Sep 2022 19:09:33 GMT  
		Size: 308.7 MB (308729585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7198b31b9f5cd080c3fdfe7494f0e0cd18dcd6142b612f2d23e5e23d0f7b81`  
		Last Modified: Wed, 14 Sep 2022 19:08:39 GMT  
		Size: 80.6 KB (80566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1063921bef347bf03152e1c58792f7e9d0939fa4bb3be8a12e1f6838ab56f7ac`  
		Last Modified: Wed, 14 Sep 2022 19:08:39 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc58d5cac278ee62a86b96be0cddd1747b2af2768915c0ce2b9b4b4e10d81518`  
		Last Modified: Wed, 14 Sep 2022 19:08:39 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672dda70948516221a8be083ee9eb7e3e8ddfebbab16200283575d3a5897ada3`  
		Last Modified: Wed, 14 Sep 2022 19:08:39 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
