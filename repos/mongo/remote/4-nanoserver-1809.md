## `mongo:4-nanoserver-1809`

```console
$ docker pull mongo@sha256:bda240dfff912882ad20517e434c68a2acb9ad3e2ebc431b5fc89ca368cc17d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `mongo:4-nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull mongo@sha256:1d4269b06d4ed306c56954871a7f949b99ebdb6015cf430adfaaaf5edff37c45
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.6 MB (344577218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ecf060e76d4056e1f221b16af57312cd9ff133331ca00d432cedf139a94f20a`
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
# Wed, 09 Feb 2022 17:10:18 GMT
ENV MONGO_VERSION=4.4.12
# Wed, 09 Feb 2022 17:11:04 GMT
COPY dir:ddb807c26f1974dd41c054a2bef12ff55fc257bc9af1f055410eea9e996a8481 in C:\mongodb 
# Wed, 09 Feb 2022 17:11:20 GMT
RUN mongo --version && mongod --version
# Wed, 09 Feb 2022 17:11:21 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Feb 2022 17:11:22 GMT
EXPOSE 27017
# Wed, 09 Feb 2022 17:11:23 GMT
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
	-	`sha256:a44ed5c3189dfaf8fb1ce615c118283e630685b20d377a0c45350faebd9935db`  
		Last Modified: Wed, 09 Feb 2022 17:56:37 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ab3801eac24f20e42b5dbb9a08700cef5e64ca467b4d58c003ae80dd2429ca`  
		Last Modified: Wed, 09 Feb 2022 18:00:52 GMT  
		Size: 241.1 MB (241064525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de793eafb2cf35e8d59ed494a47687a80e36488f0e7f3e020e141956c9625f2`  
		Last Modified: Wed, 09 Feb 2022 17:56:34 GMT  
		Size: 82.6 KB (82557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36960651112c6510279fecbd06327bdc06531a9005b03fa2cee92a052f4148b5`  
		Last Modified: Wed, 09 Feb 2022 17:56:34 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cadbe691b88bd72d2a4653683b853b4e085528fd37ed79581e83cf223b4a67`  
		Last Modified: Wed, 09 Feb 2022 17:56:34 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391db88e7537835fe919861e88fb1eb200c4ceb17ae7f9c5995b252a28f1e821`  
		Last Modified: Wed, 09 Feb 2022 17:56:34 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
