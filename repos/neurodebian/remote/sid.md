## `neurodebian:sid`

```console
$ docker pull neurodebian@sha256:73efa1484d276cca355c35fdcb32188120b91ab3f4c285cb80eaf0c6d5a7ce12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:sid` - linux; amd64

```console
$ docker pull neurodebian@sha256:0ab94fba0b73e7a820edc4a17ece79a57bec008c1c74cb162a1413f66e7c6771
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.9 MB (63936531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce94c7c74d77d5450a686fb6eef703f352ed9629aa674ac908a2e72814472ab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:22 GMT
ADD file:9463b73933c9a0f2df3bbfaa2805027794a0e3a0cca69453b066ebc4644b6f06 in / 
# Tue, 13 Oct 2020 01:42:22 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:37:00 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:37:01 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Oct 2020 08:37:02 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Oct 2020 08:37:06 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ead5025e4e59e53184c941889a91b90e4e7af750b6f2e005952c8484512851fe`  
		Last Modified: Tue, 13 Oct 2020 01:49:57 GMT  
		Size: 52.6 MB (52587404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6690926adddd90a5e3a1c4a57368f13303875757915ef569d3962379e68ac1f6`  
		Last Modified: Tue, 13 Oct 2020 08:38:32 GMT  
		Size: 11.0 MB (11047678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4843bba0024646af25ba31f8dd6c17c3f959ae2ff3202a8358b6533a65affb6c`  
		Last Modified: Tue, 13 Oct 2020 08:38:29 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e12687c9019296574980fc3215620d457d54f378bf49b0c5361c61e5617559`  
		Last Modified: Tue, 13 Oct 2020 08:38:30 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a762df0c19316fe85809dfd40fcd1ebf03a2f2099fadac9ab208939c12e50806`  
		Last Modified: Tue, 13 Oct 2020 08:38:29 GMT  
		Size: 299.5 KB (299452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
