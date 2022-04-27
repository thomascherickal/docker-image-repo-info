## `mongo:nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:c169791e78af31b594c12df76d90d9dc6d5cbe9c4e22e72da773bb28775bab17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `mongo:nanoserver-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull mongo@sha256:f8e0b9ee28fc088df38530682a575f77aeee5010c2f86e468ef03e5cb887c178
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.3 MB (424289689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea1a6500fd5b005d9662ea16444fb59832fc64c4ea4c0cec504129669753b736`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sun, 03 Apr 2022 05:29:07 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Apr 2022 02:43:38 GMT
SHELL [cmd /S /C]
# Wed, 13 Apr 2022 17:34:27 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 17:34:36 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Apr 2022 17:34:37 GMT
USER ContainerUser
# Wed, 13 Apr 2022 17:34:38 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 27 Apr 2022 00:20:07 GMT
ENV MONGO_VERSION=5.0.8
# Wed, 27 Apr 2022 00:20:36 GMT
COPY dir:9aebb2bcb5bf84c811662598b13aa11118bce2074fb69895d906750a935d529f in C:\mongodb 
# Wed, 27 Apr 2022 00:20:47 GMT
RUN mongo --version && mongod --version
# Wed, 27 Apr 2022 00:20:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 27 Apr 2022 00:20:49 GMT
EXPOSE 27017
# Wed, 27 Apr 2022 00:20:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5ee98801bdad72bc36678d072c89f7dd482fee29086c1d9c8ad6ff0cb5afa385`  
		Size: 117.6 MB (117579416 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0ae7f8fcefe8f9cd0745bf20258e1950e1c72b8ca86cc031fca90ec3e24203e`  
		Last Modified: Wed, 13 Apr 2022 03:16:38 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f6eb35034542f1e8cda3b15fc48faf88551e753d68db2a9567d62a8b2f4139`  
		Last Modified: Wed, 13 Apr 2022 18:01:19 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a897233ecb418719699d59c61a5a680dba34aed5b55156109835b7c7979972`  
		Last Modified: Wed, 13 Apr 2022 18:01:17 GMT  
		Size: 87.6 KB (87595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222eec50270ee0d80f5d695a57ac3acb77fcfa12b827d5b72852aef4e28990bd`  
		Last Modified: Wed, 13 Apr 2022 18:01:16 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0e50b581be23686aad76397f0b3d3325837a54885da2740b7414e7de1ceb79`  
		Last Modified: Wed, 13 Apr 2022 18:01:17 GMT  
		Size: 263.4 KB (263435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c9aa6aab7882424ec5ac593d2fdb149c355cea30ca960dfa73ae443cf52311`  
		Last Modified: Wed, 27 Apr 2022 00:37:15 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804defd1eab76e32bec970a4456975b63cd9febf758fe1f3ebf3dfa71dbb6632`  
		Last Modified: Wed, 27 Apr 2022 00:38:10 GMT  
		Size: 306.3 MB (306302245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988126b2b25dd2740b316b48b879b53c663c8fc918a801e5c566951929f3eec1`  
		Last Modified: Wed, 27 Apr 2022 00:37:12 GMT  
		Size: 48.9 KB (48924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280dfcafbdcc334b61085800ba6c46906358d426f30f5a05eeea4aaf5dc78351`  
		Last Modified: Wed, 27 Apr 2022 00:37:12 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0c3a6d0c718a7af30e80d4e229fe2ab000d28e51e383cf1813b9515466128e`  
		Last Modified: Wed, 27 Apr 2022 00:37:12 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d604a41f062833dfa0852c3e2f91a1b506dffbd4665068960e972e4718eed55`  
		Last Modified: Wed, 27 Apr 2022 00:37:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
