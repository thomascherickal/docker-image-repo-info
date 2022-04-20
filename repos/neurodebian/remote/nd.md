## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:2815d4a05337e97e3f7269bbd1dc1c28f74e0154aabe1ece071afd963798db79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:88c63be83ecb9172a678c518c96e1ac581a6805493f9e22389fa560341cb6f26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67729657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1aab69a806cc36ffb9865df44e439c970b23c79572bbc9c78af536ecc19f389`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:44:37 GMT
ADD file:859abf2d579747b132742454ad96e32dc879955afff8af84fab63dc41312a0e0 in / 
# Wed, 20 Apr 2022 04:44:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:09:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:09:36 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 20 Apr 2022 10:09:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 20 Apr 2022 10:09:40 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:212be0dc3a8ffdc400158a5e3a9812f7413dbb5a86269ff50e41b84b37fdb9f7`  
		Last Modified: Wed, 20 Apr 2022 04:50:51 GMT  
		Size: 56.1 MB (56112566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cea007a13810a5bdfef0ab507bcd7f7bd9a114e9046c091bdc03a8bb7aded55`  
		Last Modified: Wed, 20 Apr 2022 10:12:09 GMT  
		Size: 11.3 MB (11307358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bffc83c8ac78c14b6980d61ee782d950612d88ab4411f8d58912a259a110f5`  
		Last Modified: Wed, 20 Apr 2022 10:12:08 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68711a93b34c0c23b766d81aa742dfae9b1c6f169f9c3b53c41dce54ce61bab2`  
		Last Modified: Wed, 20 Apr 2022 10:12:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9685f8334a51b5ae7a5849af5e27ef66f92e556addb6a1b420ec8a57a1253d18`  
		Last Modified: Wed, 20 Apr 2022 10:12:08 GMT  
		Size: 307.7 KB (307729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
