## `neurodebian:stretch-non-free`

```console
$ docker pull neurodebian@sha256:2cf0deca9ea504c2206e63ffeb2312d7edc509e8bb2a7cd582d28e94c64c9d3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:stretch-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:fdd83a6f5ef34f31485f0e396dd1942c3a5d82f5721c448231dcc767807176e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52242371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe35165902a9928d2c3766b24ead0d17e650486d0a5e7c891c7d2c4869a423a`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 17:12:27 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 17:12:30 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 11 Dec 2020 17:12:31 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 11 Dec 2020 17:12:35 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 17:12:40 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6153b9908ddb81584cd82100f9820fd5776de9a2f6eecf3db92c8d87ba6275`  
		Last Modified: Fri, 11 Dec 2020 17:14:58 GMT  
		Size: 6.6 MB (6568887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede09df97d3fdd31fa406d0f493fd97a0133549433df75de6019255fe65f268b`  
		Last Modified: Fri, 11 Dec 2020 17:14:57 GMT  
		Size: 3.1 KB (3149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfc2078fc7931a0a6e61bb82ed841e6bbcdc5b77c709958a2379546d5d8ee9a`  
		Last Modified: Fri, 11 Dec 2020 17:14:58 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b937354e0832143c74a23955ff6ac45f53e69a323c7c5bf5eb37a2a02520b21`  
		Last Modified: Fri, 11 Dec 2020 17:14:58 GMT  
		Size: 292.1 KB (292119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabc3457747b85e85449126789d8fba257dd134e2e3d36aedc0dac257e9d1d52`  
		Last Modified: Fri, 11 Dec 2020 17:15:04 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
