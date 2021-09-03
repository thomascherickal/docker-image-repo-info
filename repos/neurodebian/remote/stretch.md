## `neurodebian:stretch`

```console
$ docker pull neurodebian@sha256:b2c1dc38bb231148a3aec3613df52bad10520fc6fff94ad82b750fd85623f807
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:stretch` - linux; amd64

```console
$ docker pull neurodebian@sha256:86fb8131739321a5dfead481a328c73db8e648e4e57012f3b78b395bfe1fe79a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52247136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a75f80903a4cefae8c8780a698250dae7c03f3aa1b48d14346b5fe24070d52f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:33 GMT
ADD file:835effce8521d3a6cb00dc8bb358711e7a6ba1fd057b798681d9e006825dd3c1 in / 
# Fri, 03 Sep 2021 01:23:33 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 07:29:28 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:29:36 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 03 Sep 2021 07:29:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 03 Sep 2021 07:29:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c05d83e138cea8cb6ddd17442ab2138423db80e58408d93059f2ea25065952e`  
		Last Modified: Fri, 03 Sep 2021 01:31:39 GMT  
		Size: 45.4 MB (45379797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b690a65a1de78b974d2adf195c6e713a38dcd4c05318e953372b22480521fd4`  
		Last Modified: Fri, 03 Sep 2021 07:32:14 GMT  
		Size: 6.6 MB (6571673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f602d9a07d83fa396808288db51b836b54f145bfa596d5d8cc27c5442cb0f54f`  
		Last Modified: Fri, 03 Sep 2021 07:32:14 GMT  
		Size: 3.2 KB (3154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5324ee071aa65b850c6c17f2716811538fbeb80f9537fe7bf39b649fe1135042`  
		Last Modified: Fri, 03 Sep 2021 07:32:13 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47abf28f1a08d015ed9cfdef3fb1f69d81594f65fb0fa05f84c69b7bf0b97d38`  
		Last Modified: Fri, 03 Sep 2021 07:32:14 GMT  
		Size: 292.3 KB (292269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
