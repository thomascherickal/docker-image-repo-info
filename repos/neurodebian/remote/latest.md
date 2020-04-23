## `neurodebian:latest`

```console
$ docker pull neurodebian@sha256:5ae7db0574a599b487f06d1e3a0325d0f394e25f2812ea6e29dc1e3e836d7a81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:latest` - linux; amd64

```console
$ docker pull neurodebian@sha256:0b43324ece61613f8adde1498a488f4fde918124291beaa6f946f9a162dbec46
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61184237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f25ef14a94631b7a0ed76695d6f37e02dc548e2d42a93ea1f2518887714c157c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:17 GMT
ADD file:f086177965196842af3c15f50a7f6ad7912aaa7bf73a60b1d00e3129265eec9a in / 
# Thu, 23 Apr 2020 00:20:17 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 02:27:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 02:27:48 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Thu, 23 Apr 2020 02:27:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Thu, 23 Apr 2020 02:27:56 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90fe46dd819953eb995f9cc9c326130abe9dd0b3993a998e12c01d0218a0b831`  
		Last Modified: Thu, 23 Apr 2020 00:24:56 GMT  
		Size: 50.4 MB (50382927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2075069e74d1454ca7606aea8a4c837d5a4a48bbbeec7db4902f315c30a065f6`  
		Last Modified: Thu, 23 Apr 2020 02:30:08 GMT  
		Size: 10.5 MB (10496952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d55a52976dcfb368d912bbb9bf5b585d77b47a3ae22724d84dd4a5b58817b95`  
		Last Modified: Thu, 23 Apr 2020 02:30:06 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3284dbc5e3c7c1fabf65ccf0f8ddba60f43a952c376673d638a786091d5e3870`  
		Last Modified: Thu, 23 Apr 2020 02:30:06 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db3310ee504a8457c7d447abc1ec524f04b8ed05e1eeca779c6357eadb07ba6`  
		Last Modified: Thu, 23 Apr 2020 02:30:06 GMT  
		Size: 302.3 KB (302345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
