## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:20f2a6d4ac8deb5ea7cedec1ebc36387dcd6d78bf352378ef23fedf5f0b0e5a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:c71285036b58af39ba54be6c60fe40690e87664a7ac805a1607b1ccf5403d1d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34294894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59528226ced5c705a9d16038a02b08a06d423d443464bdd9c91e2c1edbadd94a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:04:34 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:04:36 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 06 Apr 2022 00:04:36 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 06 Apr 2022 00:04:40 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bdedabcf956ec00067ab12f31abe70b007c7bdab240a7b3f7366a31a1a1925`  
		Last Modified: Wed, 06 Apr 2022 00:06:49 GMT  
		Size: 5.5 MB (5488557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfbc331c94f534cc3e7306395fd1d6c9c51ff17c5ca799ddb3cf8f4914bcac0`  
		Last Modified: Wed, 06 Apr 2022 00:06:48 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d39fbb2041431c6635e53dfa2335cf2c31fb6cd0d398469ec9c3332decb38f2`  
		Last Modified: Wed, 06 Apr 2022 00:06:48 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7d6d0860b74179b37593ae4f1d13c0fbbbf348c2945293da4f80daa2941b43`  
		Last Modified: Wed, 06 Apr 2022 00:06:48 GMT  
		Size: 238.0 KB (238036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
