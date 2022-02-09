## `mongo:nanoserver-1809`

```console
$ docker pull mongo@sha256:4dda3a5545360a34795ba54842ef06123d767e9b5c2d3cfb6b77dfa5179d4d78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `mongo:nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull mongo@sha256:c5f3c568de3486f30d56b5423631ed97a7ca3fa8486807fedd3cf23002c16830
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **405.9 MB (405908411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c32afe2e8f7a9ac1b75a1f6eafce953a8066e5aa34c75f28c1b6f90047d0752`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 13:53:17 GMT
SHELL [cmd /S /C]
# Wed, 09 Feb 2022 17:00:40 GMT
USER ContainerAdministrator
# Wed, 09 Feb 2022 17:00:57 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 09 Feb 2022 17:00:58 GMT
USER ContainerUser
# Wed, 09 Feb 2022 17:00:59 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 09 Feb 2022 17:01:00 GMT
ENV MONGO_VERSION=5.0.6
# Wed, 09 Feb 2022 17:02:19 GMT
COPY dir:8054396aef21c43e8eb1e82c0d52daca301fb548900656fb893eece57b5d6e88 in C:\mongodb 
# Wed, 09 Feb 2022 17:02:34 GMT
RUN mongo --version && mongod --version
# Wed, 09 Feb 2022 17:02:35 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Feb 2022 17:02:35 GMT
EXPOSE 27017
# Wed, 09 Feb 2022 17:02:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4cc9ef1ef09cb03b1e0bcf4dd4f522871216249d6274e1708e2d4ac554954f34`  
		Last Modified: Wed, 09 Feb 2022 14:37:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83246e4eb618ea62668053a19d786c3ea566cacf278f6d14b4417b0d49de2b0d`  
		Last Modified: Wed, 09 Feb 2022 17:44:18 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bd4b9bbeeb5c874bf14d57afee1e54393e42b0d4386c53969921d3bbb53afe`  
		Last Modified: Wed, 09 Feb 2022 17:44:16 GMT  
		Size: 71.4 KB (71373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ca51556baa0c9dd1d87223d60567d5a9385802591401231b68b4dd37f2057a`  
		Last Modified: Wed, 09 Feb 2022 17:44:16 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508991573a06beb208b68f368bd0d9e643f01f4149f8d51a7c92c6cf808df659`  
		Last Modified: Wed, 09 Feb 2022 17:44:16 GMT  
		Size: 263.5 KB (263457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74e9f79a036e6fbd8797ec2547681007eccabd803cb15613472e34ef1b5184e`  
		Last Modified: Wed, 09 Feb 2022 17:44:16 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b957a61edc0c4631e3986db37f1a78e511dd6fc16aa723059d9a377563e3b9`  
		Last Modified: Wed, 09 Feb 2022 17:49:43 GMT  
		Size: 302.4 MB (302389591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c382df20165afa4fc0b10f7c5ad2bd15449f44b0891c5f6d7b806c7d745734fe`  
		Last Modified: Wed, 09 Feb 2022 17:44:14 GMT  
		Size: 88.7 KB (88742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c802f13f4ebfb39e9bd70e43636f0bb8f9b197d4969bb1af6b5b792479f36a`  
		Last Modified: Wed, 09 Feb 2022 17:44:14 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178653741809a85481a686e198255694d5eaf50e442e11cf2f2cd6970992f8d5`  
		Last Modified: Wed, 09 Feb 2022 17:44:14 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f457b32563cf4d660179464281fe241320d6b1e150ed9f07bce8d58dc3eb2546`  
		Last Modified: Wed, 09 Feb 2022 17:44:14 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
