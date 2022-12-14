## `mongo:6-nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:ff4424caa91ef139dcce719d23a23d76916461a5c12d8e44c4b4d70d8101805a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1366; amd64

### `mongo:6-nanoserver-ltsc2022` - windows version 10.0.20348.1366; amd64

```console
$ docker pull mongo@sha256:66266fe2222ee30bfda557489a8c54506b4091ce92efc76beb17a0a3cad8a00e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **634.5 MB (634488527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a86fbdecc1a1aed443c26c8ca2df96bb0560f96d8a0d9c2efe1b386b1fee78`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 09 Dec 2022 09:19:21 GMT
RUN Apply image 10.0.20348.1366
# Wed, 14 Dec 2022 00:26:31 GMT
SHELL [cmd /S /C]
# Wed, 14 Dec 2022 01:34:41 GMT
USER ContainerAdministrator
# Wed, 14 Dec 2022 01:35:24 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 14 Dec 2022 01:35:25 GMT
USER ContainerUser
# Wed, 14 Dec 2022 01:35:26 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Wed, 14 Dec 2022 01:35:27 GMT
ENV MONGO_VERSION=6.0.3
# Wed, 14 Dec 2022 01:36:32 GMT
COPY dir:504ba3c422010154364f85a9b7f5ebcd0252fe3e628d277d138a4248175996a9 in C:\mongodb 
# Wed, 14 Dec 2022 01:37:16 GMT
RUN mongod --version
# Wed, 14 Dec 2022 01:37:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Dec 2022 01:37:17 GMT
EXPOSE 27017
# Wed, 14 Dec 2022 01:37:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:70d3e1cc3b0ea172dcc93064fe6fb9f1f2c8fec6962c90e39991fe89a3c1ca03`  
		Last Modified: Wed, 14 Dec 2022 00:08:13 GMT  
		Size: 122.1 MB (122108200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f9e07f68da133ce8f348b35ab3af5ec6b757880ed6c11fe2b1e180d9cc11d2`  
		Last Modified: Wed, 14 Dec 2022 01:13:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d3b1161f2b7036bb43459a6af412876d2a637ec8d5b6e577bc716e7bfa5156`  
		Last Modified: Wed, 14 Dec 2022 02:16:21 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b200bac9ac821d6933d970c2189ae6cd614821fb8e21eb0554d0397e7d05e552`  
		Last Modified: Wed, 14 Dec 2022 02:16:19 GMT  
		Size: 87.6 KB (87636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e55b8fe1450fe0db2aa7a335c3ca845893a02c9ecf4cc750fa295b10d33035`  
		Last Modified: Wed, 14 Dec 2022 02:16:19 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338a2300adb6e75844ef16eb12a881cd075333e67fa42e8163e5f56bf126086e`  
		Last Modified: Wed, 14 Dec 2022 02:16:19 GMT  
		Size: 267.2 KB (267198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe17f2d8f83b7a79ae89342b66b576caeb738c246f09e731c9ac9bab83e6c719`  
		Last Modified: Wed, 14 Dec 2022 02:16:18 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beeb2234dd923b63e9136ca33f29a84545958731246bce7b636e21e9c54368d0`  
		Last Modified: Wed, 14 Dec 2022 02:18:02 GMT  
		Size: 512.0 MB (511967858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5c55a687bbd29930ad7b103fb2298dbba1a7599743701b5c24e244d3815104`  
		Last Modified: Wed, 14 Dec 2022 02:16:15 GMT  
		Size: 49.5 KB (49453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057cf1425e25dfb318c7214836df86b4edbdd70f06d88bc4e723e2ca5a7058dd`  
		Last Modified: Wed, 14 Dec 2022 02:16:15 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f27855568ca8a42788d2f857e9122b15c3310b8ebb2049dbb8794d2d06ebb0`  
		Last Modified: Wed, 14 Dec 2022 02:16:15 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585da1dbc624f21209fd4ced61792b4a85c8f0c3dc0362355bd082f44d50df28`  
		Last Modified: Wed, 14 Dec 2022 02:16:15 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
