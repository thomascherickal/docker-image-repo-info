## `mongo:4-nanoserver-1809`

```console
$ docker pull mongo@sha256:41a9ed6014f02b13db29a408fc1120447e8c20111732bddc407e0baf6b44c619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `mongo:4-nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull mongo@sha256:d7af9c43d378768128825d5ef462fc64b965622115afc63d5a73356cf7e915e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.3 MB (351337239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f901a4cfecaa821ee24b105f3c425eb01cb0e4849a3e000801806e9fefcea972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 00:31:01 GMT
SHELL [cmd /S /C]
# Wed, 14 Dec 2022 01:37:26 GMT
USER ContainerAdministrator
# Wed, 14 Dec 2022 01:38:03 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 14 Dec 2022 01:38:04 GMT
USER ContainerUser
# Wed, 14 Dec 2022 01:48:58 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 14 Dec 2022 01:59:15 GMT
ENV MONGO_VERSION=4.4.18
# Wed, 14 Dec 2022 01:59:45 GMT
COPY dir:f47c837744091598673c1e98795dbb20d206784d286c7f5d0e937f34d552568a in C:\mongodb 
# Wed, 14 Dec 2022 02:00:29 GMT
RUN mongo --version && mongod --version
# Wed, 14 Dec 2022 02:00:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Dec 2022 02:00:31 GMT
EXPOSE 27017
# Wed, 14 Dec 2022 02:00:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb1e4df1760e3de08ff30de6fd3f3acf348399853dab1aa1632ed4080cd102`  
		Last Modified: Wed, 14 Dec 2022 01:14:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbb42ac6a3096f2047a475c0c86cb9b35024f73b26ce0e2c0449895724123d0`  
		Last Modified: Wed, 14 Dec 2022 02:18:24 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b83062061825d32cc34037cc0175220e130f9f3d0c86e79ff42affc2376cdd`  
		Last Modified: Wed, 14 Dec 2022 02:18:21 GMT  
		Size: 73.2 KB (73169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60417ca99e1256191d2c6e4453104f0c48edc4251a02981488df3a3ce9be5802`  
		Last Modified: Wed, 14 Dec 2022 02:18:21 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c002f12039eae15e804c5b2fdfd193fb0622d907f1a5f462d73514cff54e8ee`  
		Last Modified: Wed, 14 Dec 2022 02:25:07 GMT  
		Size: 263.5 KB (263504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a8bd783ccb365472364dfb78ed8c3acd5fb598a7d1dc8c16eedab5d2cd3394`  
		Last Modified: Wed, 14 Dec 2022 02:29:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ec590f592e0291b21ace5ba73c278153e91cc303d5609ed6f2437e6848b4ea`  
		Last Modified: Wed, 14 Dec 2022 02:30:07 GMT  
		Size: 244.2 MB (244246919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb32f02694bc85d059984a5cfae98bdb12687a3daa89fc513020d71cb3b466a`  
		Last Modified: Wed, 14 Dec 2022 02:29:16 GMT  
		Size: 74.4 KB (74434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddfbb299ec46f4c568e1de4e9089757a962308d73622839bc673029fb9efad5`  
		Last Modified: Wed, 14 Dec 2022 02:29:16 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c2bcf67e091bb3192933948d8a997200c660b9e395d59c359263d4512c2707`  
		Last Modified: Wed, 14 Dec 2022 02:29:16 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3108dfc2cee3db408c44d1108c13cf945f8bcc9a414d1bb718b1c6712965e808`  
		Last Modified: Wed, 14 Dec 2022 02:29:16 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
