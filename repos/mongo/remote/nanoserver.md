## `mongo:nanoserver`

```console
$ docker pull mongo@sha256:b04d48437f8292c69ae42325789cc888f33eb37c684e6d18fb8ed6c9a4fe81d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1850; amd64
	-	windows version 10.0.17763.4645; amd64

### `mongo:nanoserver` - windows version 10.0.20348.1850; amd64

```console
$ docker pull mongo@sha256:1fb0173172bdfab9278c2160eef21d637cfe423692a51c596ca0f68697317b5d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **637.1 MB (637054012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d62d81c56a139d24560283598ba1ee2969c4b7ae6d8b989ae80b934cbe8eb12`
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
# Thu, 13 Jul 2023 22:41:40 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Thu, 13 Jul 2023 22:57:22 GMT
ENV MONGO_VERSION=6.0.7
# Thu, 13 Jul 2023 22:58:01 GMT
COPY dir:6115b874c812adb9a4e4da58fe85482084095a26c49827ac1513416f28ff99f9 in C:\mongodb 
# Thu, 13 Jul 2023 22:58:15 GMT
RUN mongod --version
# Thu, 13 Jul 2023 22:58:16 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 22:58:16 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 22:58:17 GMT
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
	-	`sha256:7e4f862bd8d3921ac069f3d77465c09e893240d2097dcf9f298858f17bc60ad4`  
		Last Modified: Thu, 13 Jul 2023 23:27:01 GMT  
		Size: 267.2 KB (267212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9ceb17d80453c53640da8f895a8b33b6e05ed61ca023365c712e36b3b91a39`  
		Last Modified: Thu, 13 Jul 2023 23:39:16 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c068442554a2e47063609e7dfd006e6d28bf8ed0b55c08c358f5e7b23dab808`  
		Last Modified: Thu, 13 Jul 2023 23:40:32 GMT  
		Size: 516.6 MB (516588038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673f6d35af57ac18d6ac4a187f55deab63a86bb2d46dec09023cfab023817d31`  
		Last Modified: Thu, 13 Jul 2023 23:39:14 GMT  
		Size: 54.0 KB (53978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4608686fc9f7b60e382de094cb08d695affa19918a2ea3d67b2a1584f50e425e`  
		Last Modified: Thu, 13 Jul 2023 23:39:14 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495ec412828eadeade8a970546a565c209f46bb7247e2235003eea29c119896a`  
		Last Modified: Thu, 13 Jul 2023 23:39:14 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583d9d0a900a036ed9a7a39202ad6bee0671f9eb5e4b6b55dcb23e8db66647c7`  
		Last Modified: Thu, 13 Jul 2023 23:39:14 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull mongo@sha256:3871ea7e6fa8ed7e1f4e585524dbece58fb956884c0ff2efbc198c083ec03b27
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **621.4 MB (621416254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ed32816a3a84de1c2fdb48e99c960faf1806966547c5432ba8f0c3870a0d10`
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
# Thu, 13 Jul 2023 22:43:06 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Thu, 13 Jul 2023 22:58:24 GMT
ENV MONGO_VERSION=6.0.7
# Thu, 13 Jul 2023 22:59:00 GMT
COPY dir:6115b874c812adb9a4e4da58fe85482084095a26c49827ac1513416f28ff99f9 in C:\mongodb 
# Thu, 13 Jul 2023 22:59:13 GMT
RUN mongod --version
# Thu, 13 Jul 2023 22:59:14 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 22:59:15 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 22:59:15 GMT
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
	-	`sha256:4022eb1ac7f21a3a4d4f640ce85aead9f625653c11bc05eb3929118d0e799544`  
		Last Modified: Thu, 13 Jul 2023 23:28:41 GMT  
		Size: 267.2 KB (267186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ec8843ed890a7fdb870f278e82f69654c15dafcc8699557db7917835f61719`  
		Last Modified: Thu, 13 Jul 2023 23:40:48 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae27ccb7c97782ab18c3976401ddfb4f5ca6ad0512756255189c973e0cc6363`  
		Last Modified: Thu, 13 Jul 2023 23:42:03 GMT  
		Size: 516.6 MB (516588106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac89c6418a9aba3aa882e502df98fd52effd4636bd48331fc5803e248a5dbd06`  
		Last Modified: Thu, 13 Jul 2023 23:40:46 GMT  
		Size: 75.8 KB (75841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce14c3490c0f95ed7bf96419bf250f8531482a8c07ad925ad7b38c8251397433`  
		Last Modified: Thu, 13 Jul 2023 23:40:46 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3270db456ebae6dfa00f0421c29c94819eb5feb824b6f1c9afbbe823f7cc86e5`  
		Last Modified: Thu, 13 Jul 2023 23:40:46 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864ae9dd317011f6054feb229d867e74b0b0d5fff5198ac41c133752f626f7eb`  
		Last Modified: Thu, 13 Jul 2023 23:40:46 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
