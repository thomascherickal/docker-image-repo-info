## `mongo:nanoserver`

```console
$ docker pull mongo@sha256:299bddfeb4c950e01c2570590697496e42f67a0395ea3a0cf919e97018b428bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `mongo:nanoserver` - windows version 10.0.20348.643; amd64

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

### `mongo:nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull mongo@sha256:7ec6807a672ea0c68ef30f153538bfc278a8f34206548fb6e1e2108c35b660dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.8 MB (409784257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a12f83c9a94269e4adfa57e4a05bf2b2cc47f9559992e53cb3705dfb0f38d48`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 02:48:06 GMT
SHELL [cmd /S /C]
# Wed, 13 Apr 2022 17:35:28 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 17:35:35 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Apr 2022 17:35:36 GMT
USER ContainerUser
# Wed, 13 Apr 2022 17:35:38 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 27 Apr 2022 00:21:00 GMT
ENV MONGO_VERSION=5.0.8
# Wed, 27 Apr 2022 00:21:30 GMT
COPY dir:9aebb2bcb5bf84c811662598b13aa11118bce2074fb69895d906750a935d529f in C:\mongodb 
# Wed, 27 Apr 2022 00:21:41 GMT
RUN mongo --version && mongod --version
# Wed, 27 Apr 2022 00:21:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 27 Apr 2022 00:21:43 GMT
EXPOSE 27017
# Wed, 27 Apr 2022 00:21:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a1e4f80cd1f664faa50444f6850501c0035534cf86f2ed0b458586b9f4b5089e`  
		Last Modified: Wed, 13 Apr 2022 03:18:01 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19568f22509c76cadae091bbc3a9c4064c4d0c458b1c66b01af3820fe0d3f5e`  
		Last Modified: Wed, 13 Apr 2022 18:06:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686e0047ea9d2b545c4705a478cf3f5a8ba67594255da0a0794a75bdbd829339`  
		Last Modified: Wed, 13 Apr 2022 18:06:49 GMT  
		Size: 70.3 KB (70348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7042f8e1bb874fc050093e4073fc53cbfc0e7ac47c18a5c163f5c541181c96`  
		Last Modified: Wed, 13 Apr 2022 18:06:48 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14043e3c2c29d92551a552ccde6c8c9ca4a27a12b67eb4d95b9a99ff3cea0088`  
		Last Modified: Wed, 13 Apr 2022 18:06:49 GMT  
		Size: 263.5 KB (263523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff12fa42950ba951b70783aa2c92819153bb38ccad078a9f00246105c8f52fd0`  
		Last Modified: Wed, 27 Apr 2022 00:38:29 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb21e42c27802248fba381681a774eb75ab1d61312814aebd2ab964bec128f44`  
		Last Modified: Wed, 27 Apr 2022 00:39:22 GMT  
		Size: 306.3 MB (306302167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b5f905f763ba4cb32997d3c24cdc02ea1aae4ef2cf5608292786e8322aed38`  
		Last Modified: Wed, 27 Apr 2022 00:38:27 GMT  
		Size: 44.0 KB (44037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6f3e32281bd52aab3dbb6b9c32e3c0d8df729e0c6dc8fce69167c912a200cf`  
		Last Modified: Wed, 27 Apr 2022 00:38:27 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92e0b4eff8969f294b182271ad7417467730a1d275efc4292262c091a083d8e`  
		Last Modified: Wed, 27 Apr 2022 00:38:27 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c59206626f165f17eea75042255c5d3984a9025abe25617c889b715d28f83f`  
		Last Modified: Wed, 27 Apr 2022 00:38:27 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
