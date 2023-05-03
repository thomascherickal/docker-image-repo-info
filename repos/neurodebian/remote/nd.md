## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:e4401f9e4c26635545e07c44b905f34749ba1c3e7de887b7a123dc775cdf64e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:bfe67002364838700c76c1c3a2f8ceaf639c6a6298213f3518a0dc9635906c92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61305792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7628118084f66e224ab75edf762667e0641ead33e66b059e71a6299bd2c7eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:42 GMT
ADD file:6261ecb921e04d2b3f6fd44e5dcb5683154bc0beee4f26913c2be9395a060489 in / 
# Tue, 02 May 2023 23:47:43 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:26:06 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:26:08 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:26:08 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:26:12 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ae396e350f30e1defad1bfa67a84b97389d42cf3442551e39a0e2bab6b53a50c`  
		Last Modified: Tue, 02 May 2023 23:51:56 GMT  
		Size: 49.3 MB (49299270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07001fa6af159175c58303f7752dd97019fd06951e7055bcb076e5194afa064f`  
		Last Modified: Wed, 03 May 2023 21:27:50 GMT  
		Size: 11.7 MB (11719904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdf86d32a3b26b1c1bd693d70bc6115b98a87379e31ff8b6f6b9f7ed9009fe3`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dee1f3f9a40aee303f152160ad22cf80424301d6e75afcd194d8f83d27543`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745484e4809d3b3760d3a506060c0d4454cf63ff0de190c172235e7f825eaa2f`  
		Last Modified: Wed, 03 May 2023 21:27:49 GMT  
		Size: 284.6 KB (284611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:6c7d30b8353ea0568c57abf602fec60303e70ecb6ef960d7fe0bcb4312d5dffc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61316334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a92e4f68720f370fa2a65f5fc53ce804514a1a0c5465f55e42fe83ca113af96`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:23:28 GMT
ADD file:cb107aa90220a9fc72fe1e3aa26878752691d6e9eb04696738920b5834c6d9e2 in / 
# Wed, 03 May 2023 00:23:29 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:07:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:07:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 19:07:11 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 19:07:14 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:77a3c1a83d83f65ef8fd579d19879f09a4018e384f42cfa55f82d426f32ff840`  
		Last Modified: Wed, 03 May 2023 00:27:15 GMT  
		Size: 49.3 MB (49345262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6755ed7d6b8b6a23dd3196274569cbf3269257dbd028e147daab4e68ab5b6226`  
		Last Modified: Wed, 03 May 2023 19:08:47 GMT  
		Size: 11.7 MB (11684076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850fa57dd587cc4293a39c6cc79ea0bcb825b944153b9916c33653f4cfd4199`  
		Last Modified: Wed, 03 May 2023 19:08:46 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f7ee09f9f60b5be173a36b9fcd1a7f7324d22afdb71424edb21e402ddeda5`  
		Last Modified: Wed, 03 May 2023 19:08:46 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671bd4d94aea2475c1870b94643b61f243f879a9ba5296070aff0744f303acd1`  
		Last Modified: Wed, 03 May 2023 19:08:47 GMT  
		Size: 285.0 KB (284989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:3b6b8e4d74f7b2e0588e78d57f42804b1199658d79edb63d4318bce88ee9a8e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62736224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a79bfdf9ea9569761583f71c192d487fe5e2b28c1b2d02afec5c88a11cdc50`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:51 GMT
ADD file:31710a830769b5e1f2612e1cd05380f677714bf52f61a54adbc7424087fd1378 in / 
# Wed, 12 Apr 2023 00:39:52 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:07:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:07:05 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 12 Apr 2023 05:07:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 12 Apr 2023 05:07:10 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35e4af56b8bda58bf958814bc36c8e3a9a1d719c8582c0f33d7d69cc5b416211`  
		Last Modified: Wed, 12 Apr 2023 00:44:24 GMT  
		Size: 50.3 MB (50310899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6fe85e96c8c420958512f9b7f261930a6843f926183876a2ab71040b63c6dd`  
		Last Modified: Wed, 12 Apr 2023 05:08:23 GMT  
		Size: 12.1 MB (12141289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c6736f7382ead0267b27d16a5f707666c92d8a808590c95172291047b1c9be`  
		Last Modified: Wed, 12 Apr 2023 05:08:21 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be953d69007bced41ea3811e8f0ec4593f0a19fa20f03e948e70cc9ddeefb87f`  
		Last Modified: Wed, 12 Apr 2023 05:08:21 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56de3369c632f2e489198a1090dfdc1db235dde1a2deb239cc07eb0c9006ece1`  
		Last Modified: Wed, 12 Apr 2023 05:08:22 GMT  
		Size: 282.0 KB (282032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
