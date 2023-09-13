## `mongo:4-nanoserver-1809`

```console
$ docker pull mongo@sha256:7d94ab337993ab54bad4e90fe4b3da3d73bb22b642e6b649194b9257265b0aed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `mongo:4-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull mongo@sha256:b6bcad08b5c0810bc9fd39a080c3804cae5e297d9feb3291cf0b7c749f935a98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.9 MB (349936114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c94df2b566880b51649152364a3a49a59f3590ffed56667083b4e4cdd8c42e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 01:47:57 GMT
SHELL [cmd /S /C]
# Wed, 13 Sep 2023 04:01:38 GMT
USER ContainerAdministrator
# Wed, 13 Sep 2023 04:01:43 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Sep 2023 04:01:44 GMT
USER ContainerUser
# Wed, 13 Sep 2023 04:22:12 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 13 Sep 2023 04:32:50 GMT
ENV MONGO_VERSION=4.4.24
# Wed, 13 Sep 2023 04:33:11 GMT
COPY dir:1066042ae200f96ac2fccaeb2deab7c0e3f03606d0c552a57bf93bf4149d79fb in C:\mongodb 
# Wed, 13 Sep 2023 04:33:18 GMT
RUN mongo --version && mongod --version
# Wed, 13 Sep 2023 04:33:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:33:20 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:33:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbcbc05a0b3c240fc185ae93c7d844ad01c0d60ef9429ad4d230a78065a9ce`  
		Last Modified: Wed, 13 Sep 2023 02:18:48 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8461d082f0027d9ed1cd74ee8e9e1dbcb1250ea330332f1459c3a74a59e242`  
		Last Modified: Wed, 13 Sep 2023 04:39:52 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d24e4e27b8237cb6af207bc6c651cf8397fd4f0bd0e14d7fea42327ea04aa6`  
		Last Modified: Wed, 13 Sep 2023 04:39:51 GMT  
		Size: 70.2 KB (70185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0a145cf1519e52c048521ae1f199df2b6cba60425d6ed0fda7071a4785269e`  
		Last Modified: Wed, 13 Sep 2023 04:39:51 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9a3648bd9e446adfa30a5a41133aedd1a84e0ac88bb23fc3d50edffd64ba03`  
		Last Modified: Wed, 13 Sep 2023 04:55:15 GMT  
		Size: 263.4 KB (263400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e5d3cad8557340d2fcc5b3bf58b8cd7b329365b425ee74c514705a05843a26`  
		Last Modified: Wed, 13 Sep 2023 05:02:55 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b042a447f08da918949fcff2666b88c4316bd8a12dadb6a52023a4ed55bc2ad`  
		Last Modified: Wed, 13 Sep 2023 05:03:36 GMT  
		Size: 245.0 MB (245046073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e3f92faabbdc7315642e28d4d26ea5b48ca0452a89f927168dd84577aaffe`  
		Last Modified: Wed, 13 Sep 2023 05:02:53 GMT  
		Size: 56.1 KB (56131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b14a1e4b40f2c3e3067c270ab73381781749902da31dd74132596f024a58e`  
		Last Modified: Wed, 13 Sep 2023 05:02:53 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acbdd94c8ea20805bf95d6cd1950c0259e843b58edc96ddf0c32332f8bb605b`  
		Last Modified: Wed, 13 Sep 2023 05:02:53 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e834d692f2f9e9bce6784acba232bdcc10f69b6121c6892ac1970f2a1bcba4ee`  
		Last Modified: Wed, 13 Sep 2023 05:02:53 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
