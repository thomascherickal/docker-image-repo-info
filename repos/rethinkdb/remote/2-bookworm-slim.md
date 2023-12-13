## `rethinkdb:2-bookworm-slim`

```console
$ docker pull rethinkdb@sha256:4687d87f45675d704804b1b188ce895eecdf368d058d17b46e3949ccc7468f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2-bookworm-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8a41211b67e0a9ad1a6f9678f2da1440cb6d2b09bc2931b46c94d3fe7411f393
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425c04783e91453d2ffc48d0d4e28fbe415515b0c79ca46da83a7424d6ad5acf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:20:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:20:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:20:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:20:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:20:23 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:20:23 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:20:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:20:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c4b9f3d90f10afbdf95273f1c0bd904c1fc11c5588546bf19d597f47a5c9`  
		Last Modified: Tue, 12 Dec 2023 18:20:55 GMT  
		Size: 9.8 MB (9789060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8fa566039e71b2179938f635faaf0ed681a373ad3a3eeb27e64a0dfce4abc`  
		Last Modified: Tue, 12 Dec 2023 18:20:54 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941bb608cbc6aa331c60524e5aeee41e8d6b337da2feefa9aaae1e9098139eb`  
		Last Modified: Wed, 13 Dec 2023 23:20:35 GMT  
		Size: 10.2 MB (10198535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161eaac0e185db0872164cdb4f7ea3b9e36d6cbf5b8056cffe787b03bfe2c226`  
		Last Modified: Wed, 13 Dec 2023 23:20:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
