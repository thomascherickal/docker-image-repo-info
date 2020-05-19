## `gazebo:gzserver9-stretch`

```console
$ docker pull gazebo@sha256:d0c84e50fa22cf547ddf4256bd7bb16f91f0c86e6d0c66cd7834a1f63b64fda0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:1ce3d360e0b99fdcf6cdbe4617b00824368e943c66d381367cdc391fa04cab4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.1 MB (265143527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f075aa93d4ae708cbd2ec70cca8a06591e3273161578b4860c8ee1bc8aea25b9`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Tue, 19 May 2020 18:33:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 19 May 2020 18:33:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 19 May 2020 18:33:08 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 19 May 2020 18:33:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 19 May 2020 18:33:58 GMT
EXPOSE 11345
# Tue, 19 May 2020 18:33:59 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 19 May 2020 18:33:59 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 19 May 2020 18:33:59 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66a765fbaaf8ff7989f8adb4b2c5ae40e1f2c3ee4bb7787a5b88552d69ce732`  
		Last Modified: Tue, 19 May 2020 18:55:16 GMT  
		Size: 18.5 MB (18500678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b578d2d70235a4773c93b8218c23abae72a96bb767ff83cb3cdbb8efaf45e0`  
		Last Modified: Tue, 19 May 2020 18:55:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7fecabd356acfd5b759b0ad53029f74ea65bf1583599b479a5e27b777d1a82`  
		Last Modified: Tue, 19 May 2020 18:55:05 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a6674522b93136cd89dcb7cdab1b5bca5ff31e0989850361a710e69e0d6a8c`  
		Last Modified: Tue, 19 May 2020 18:55:53 GMT  
		Size: 201.3 MB (201261056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e814a418d8b45d025f63f56514fe9d55dad3660969ebd3801e837ce9111e69d7`  
		Last Modified: Tue, 19 May 2020 18:55:05 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
