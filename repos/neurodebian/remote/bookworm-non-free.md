## `neurodebian:bookworm-non-free`

```console
$ docker pull neurodebian@sha256:f2d8ae2275d0d9844602a6a85af588f2f322ec0b78b1b91c0e246ce5e708ad6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:bookworm-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:6a9de2fb901912716b06d8e23e8ff0349b7602e756b15b596b8cdc39ee65b957
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65253617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4058d62fa9bf741fde7e580b6a91c18ac1f57aeb96b3eaad54cb73bf059105ee`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 May 2022 01:19:44 GMT
ADD file:daaac4875b34dee73ff062c17a4763b2cf5726753df4e9700bbcefa0f88153e6 in / 
# Wed, 11 May 2022 01:19:45 GMT
CMD ["bash"]
# Wed, 11 May 2022 10:06:33 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:06:35 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 11 May 2022 10:06:35 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bookworm main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bookworm main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 11 May 2022 10:06:39 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:06:43 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:d68396ae84f0ca729923a79943893f43492725d77e7b329170777a2bdbb6752b`  
		Last Modified: Wed, 11 May 2022 01:24:08 GMT  
		Size: 52.9 MB (52944400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc375d5bd0e34f68f784d5104bc9e98e7bf1f46fe30eb8edc038f7312b920c00`  
		Last Modified: Wed, 11 May 2022 10:08:53 GMT  
		Size: 12.0 MB (12015278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c81188af5b9a209da0d74485d6152111a6b2e0606644f544e5fb5a85eb58e8f`  
		Last Modified: Wed, 11 May 2022 10:08:51 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dff947c0d9100d4710776a70557bcc6e64fad607cea30296f31e7f8d800a96c`  
		Last Modified: Wed, 11 May 2022 10:08:51 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7380c36dee2e15247b58a7006a71e6aa046ddac8a99092385cd1b84c2316e113`  
		Last Modified: Wed, 11 May 2022 10:08:52 GMT  
		Size: 291.6 KB (291568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cc9abefa173cc506b2758398b64cff02db8ad416d85f50b8db2ec68de7255c`  
		Last Modified: Wed, 11 May 2022 10:09:02 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
