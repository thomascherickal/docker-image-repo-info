## `neurodebian:hirsute-non-free`

```console
$ docker pull neurodebian@sha256:b5f3c226abe922021cdcb1e744b5a94c0c4b65be136dabccb8282edbae580cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:hirsute-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:81b3a3123df2603b9ce4cbb3d1fdec69b27ca53aeb6c41ffb40910144d5b4d55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37554731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6985a21285ae6da663e43d4eecbc753e01432b501ca9fa3b3a7fcdac1c45e4f8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Dec 2021 02:20:56 GMT
ADD file:b94883edb5db8add88bbf8934deeda5ddd0acb4e2ce2a19a774de29ee04b7399 in / 
# Sat, 04 Dec 2021 02:20:56 GMT
CMD ["bash"]
# Sat, 04 Dec 2021 02:59:22 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Dec 2021 02:59:28 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 04 Dec 2021 02:59:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian hirsute main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel hirsute main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 04 Dec 2021 02:59:34 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Dec 2021 02:59:38 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' /etc/apt/sources.list || sed -i -e 's,universe *$,universe multiverse,g' /etc/apt/sources.list
```

-	Layers:
	-	`sha256:9e6a0d5477cff31ce49b4d3bc07409ebd27609574e968043d0b9c10acf854ebc`  
		Last Modified: Mon, 15 Nov 2021 05:13:30 GMT  
		Size: 31.7 MB (31703945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef9556fcf19d3b7d4333da5b775d44c1d1e0aa456f7515eaf9343fd13c3d69b`  
		Last Modified: Sat, 04 Dec 2021 03:00:35 GMT  
		Size: 5.6 MB (5598440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ea04fba427a22f0a2de886516090acf23e8fcf2c017d35fa44e3e036438bf3`  
		Last Modified: Sat, 04 Dec 2021 03:00:34 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12849c4eab0b59041f69c489f0638e574de3019f823e4244f3277d8f82823476`  
		Last Modified: Sat, 04 Dec 2021 03:00:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec0a2e521c337704c2d0c574d8c92f5ac48236699bc69fe559d717b2339842f`  
		Last Modified: Sat, 04 Dec 2021 03:00:34 GMT  
		Size: 250.1 KB (250075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b91cbca5dab572a96fdaad4ec0469a552624163186ce3891e1d9fb2e3a5212`  
		Last Modified: Sat, 04 Dec 2021 03:00:44 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
