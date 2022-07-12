## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:cefb3f05884720d3cd619e5ec49bbbb20ef45cb6c7037afbb958513597c8d63c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:15c08a7eebb4ac7ad2defae9a9f18446e69f966df3178d1074eb641f6da219ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61246676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7bce77ffb73c4a7fce8cc12d92a648f9332681bf4c074c0555de528b9748660`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:20 GMT
ADD file:d738977543f4afc4c3040c6fca3e3f15388ec3b7263a29a6aa83f9a4bf05fed1 in / 
# Tue, 12 Jul 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:57:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:57:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jul 2022 04:57:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jul 2022 04:57:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:80b89a2b88b24e7be7c8038e2cbff99ad4fd2f07ad914da4bab80dabaadf8a99`  
		Last Modified: Tue, 12 Jul 2022 01:24:55 GMT  
		Size: 50.4 MB (50440555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1bb727ae5cc63673d5342ec489e7aee57931d9e6de2c617a89c9139ac5c518`  
		Last Modified: Tue, 12 Jul 2022 04:59:09 GMT  
		Size: 10.5 MB (10501270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d66cf32c72db9113bd20abadfd1a0b36a76055b82e235e6327fb40f5256a1`  
		Last Modified: Tue, 12 Jul 2022 04:59:09 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85ed81a17f7b9b4ee03b03f6de9adae8aab9d9be69c76362c5e50e968b09a4a`  
		Last Modified: Tue, 12 Jul 2022 04:59:08 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dbe1eb4c30cbdb3ff00a0211d643fa48649a7ad9e1c70c58abaa44a0efab0d`  
		Last Modified: Tue, 12 Jul 2022 04:59:09 GMT  
		Size: 302.8 KB (302841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
