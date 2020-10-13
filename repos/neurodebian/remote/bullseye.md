## `neurodebian:bullseye`

```console
$ docker pull neurodebian@sha256:9aa790b9dc9744deb1ebe9e06eb356e47ada6f4dd2a61ffc258e84618e0fdae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:bullseye` - linux; amd64

```console
$ docker pull neurodebian@sha256:22454e0de5913e166e0f026266b37b96537a179df065cebef6fc329f9abb911c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63928095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0cce883fde5b7ccc4c88aa40062c586d785d8a1b096fefce1b5ab6283d4470`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:37:11 GMT
ADD file:96a5f24c28b0ba6960064c54e4643bc56eb6890db2c214c7d54bff6a00f9f049 in / 
# Tue, 13 Oct 2020 01:37:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:36:36 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:36:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Oct 2020 08:36:38 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Oct 2020 08:36:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:831751213a615bc3a20e0080e123bd3a2f1f1eef137b680b3101f3127cdff08e`  
		Last Modified: Tue, 13 Oct 2020 01:47:33 GMT  
		Size: 52.6 MB (52579873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3b506877f4751c16c445a95f357e42f4bc417f01665f4659ddb038779b26fc`  
		Last Modified: Tue, 13 Oct 2020 08:38:21 GMT  
		Size: 11.0 MB (11047402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa3863a74b5543a83b2f4a13a368499ec229d2c1b19b513cde16ad6bd2ac156`  
		Last Modified: Tue, 13 Oct 2020 08:38:19 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23610860e084fb362dc286a26fb1838faf2924c361f4a8e28ad647c0aa295289`  
		Last Modified: Tue, 13 Oct 2020 08:38:20 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b862733b536d7f59c0f2da8ce7fb681bee92fb88f43c6a38185414c872ab29c9`  
		Last Modified: Tue, 13 Oct 2020 08:38:19 GMT  
		Size: 298.8 KB (298808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
