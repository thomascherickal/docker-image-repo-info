## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:604edd044517e6a3ba82db2d8ae0e77072db4ea74a9cac8069e67d3d183caaf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:2966f71c003b332fca55d8afe0875bbea90625c45bb3ad1035de62af18df7225
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61181178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b7d4d4af130f431267307cb257afdfbddf121e8e5d17569dde4d9636e107d40`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:11:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:11:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 01 Feb 2020 22:11:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 01 Feb 2020 22:11:52 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:11:59 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee4867ba1646c5cc314467db63703fb92f8927937fe7519c86d44922b6e5817`  
		Last Modified: Sat, 01 Feb 2020 22:13:23 GMT  
		Size: 10.5 MB (10497135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00eca0098f189f0efc6dcb473a580eaf5d5f8832372174a3c19040d25bd42048`  
		Last Modified: Sat, 01 Feb 2020 22:13:21 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d799fd5749161c23c3e8b4edf6b8cadde4d5e8da880a0ecb9c72ed00dbd0b25`  
		Last Modified: Sat, 01 Feb 2020 22:13:21 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4634a3de97569c08a8fe939e5fb3a1f52e78f6d30a4502aaa5dedc9cf9854367`  
		Last Modified: Sat, 01 Feb 2020 22:13:21 GMT  
		Size: 301.9 KB (301900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5fd9ea722c63b12646b52b0ebfa3375525455f6679c04e946ce803d2132b0d`  
		Last Modified: Sat, 01 Feb 2020 22:13:34 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
