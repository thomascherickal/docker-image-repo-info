## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:3f4cd5dbfdf51deda40d93963665037129a43000243e82ef5dbea74029c4a727
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:8c38c465b778e0ad410bf5e763fe5bca00b971b780034e4d5d1ae1fa1f6fcc1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62611285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d3a50e3517c4bf1dd62d1ab3d7aad388162a1853b6d146ddea09a58db305e6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:22:27 GMT
ADD file:5055617b757ba2ab1ac6772dc2ee4cfe2ba79dd3900150b470dc61e950b9ce78 in / 
# Sat, 01 Feb 2020 17:22:27 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:12:38 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:12:39 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Sat, 01 Feb 2020 22:12:40 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Sat, 01 Feb 2020 22:12:45 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32a93ca5e0379da8be0d576367bec537380c472d398bfe5587345c3b95c3bf4e`  
		Last Modified: Sat, 01 Feb 2020 17:27:53 GMT  
		Size: 51.5 MB (51549534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232bcd7acb0e27d6c579ee7c948f7a3a02dd84ed89c20ce5403379aa7d90e9d`  
		Last Modified: Sat, 01 Feb 2020 22:13:50 GMT  
		Size: 10.8 MB (10760979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5530d8ed94595343072192bfe92d86717a541a7deee266f26dfc66787a0595a`  
		Last Modified: Sat, 01 Feb 2020 22:13:47 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0473b53f726a19dd6b919beffe3434a103bebc4728b78d6991c4e1138462d6d0`  
		Last Modified: Sat, 01 Feb 2020 22:13:47 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb784041bc804ab0103e73165c982c49a454b4a1b73fd5b62ac7da48fb13bd6`  
		Last Modified: Sat, 01 Feb 2020 22:13:47 GMT  
		Size: 298.8 KB (298765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
