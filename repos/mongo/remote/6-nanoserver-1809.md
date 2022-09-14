## `mongo:6-nanoserver-1809`

```console
$ docker pull mongo@sha256:0b4eef244b68f6d118ec93c40995dfe0e46f861e9b2726231dab1c2547c3d08e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `mongo:6-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull mongo@sha256:82e892a0d5ed7439670dd27e2dd714142e4b887b0872dc921ea89ed68d11ae31
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **613.0 MB (612978261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14d3a60d55709cd9b2dea895de680cb9e0cf536ed2607f89f8f7cfc09a81c215`
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
# Wed, 14 Sep 2022 18:18:23 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Wed, 14 Sep 2022 18:18:24 GMT
ENV MONGO_VERSION=6.0.1
# Wed, 14 Sep 2022 18:19:11 GMT
COPY dir:9bc3bf7ac427acc5da2a94db90fd2f879ea935b4a3cfd676cbd1fb49e16c8f3c in C:\mongodb 
# Wed, 14 Sep 2022 18:19:21 GMT
RUN mongod --version
# Wed, 14 Sep 2022 18:19:22 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Sep 2022 18:19:22 GMT
EXPOSE 27017
# Wed, 14 Sep 2022 18:19:23 GMT
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
	-	`sha256:85506cad2fde8d32c24db2c875bf6985f88404029a892afe534fa01b72847539`  
		Last Modified: Wed, 14 Sep 2022 19:03:36 GMT  
		Size: 267.1 KB (267096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56bf616811e89fd0a36ecb3cefb49026b4a140f19335bc0caff3da59b51e8c7`  
		Last Modified: Wed, 14 Sep 2022 19:03:35 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3bd4a3886900c83e3ffa62dbc4a259eb412bf3e305f03705220d1f3036e0ae`  
		Last Modified: Wed, 14 Sep 2022 19:04:56 GMT  
		Size: 509.2 MB (509224251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ce9fc87f09e0c56d62cb67ea775848b899a7d2a683dcc56649ad2eb08d2ae3`  
		Last Modified: Wed, 14 Sep 2022 19:03:33 GMT  
		Size: 75.4 KB (75407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c816124c571c88a02e2bfd86989f7ad0fdc4216e9255a1222a37a201a335d7`  
		Last Modified: Wed, 14 Sep 2022 19:03:33 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c037bc921a2fb8d6e01bf8e29eae5c35632f9027bbae1626399d02caf581e4f8`  
		Last Modified: Wed, 14 Sep 2022 19:03:33 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29afc05b5032e98697ea535f8e7d597e38a221e600062ad30f3980afc089d8dd`  
		Last Modified: Wed, 14 Sep 2022 19:03:33 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
