## `gazebo:libgazebo11-focal`

```console
$ docker pull gazebo@sha256:87015f3d9707a48baf135c6e2fc5cdd598c43abc4701114ca207d7a91934a4cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:c3873a165cb9e125377c60c9da33652af64bb550a961095708dcd8bc117eba9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **605.4 MB (605389796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:264c2fd030327ca513a8782e1ffd6ec49cbb4c0821b84f60db16ecd2d55a8d11`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:53:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:53:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:53:35 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 16 Oct 2021 02:53:35 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 16 Oct 2021 02:57:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.8.1-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:57:02 GMT
EXPOSE 11345
# Sat, 16 Oct 2021 02:57:03 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 16 Oct 2021 02:57:03 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 16 Oct 2021 02:57:03 GMT
CMD ["gzserver"]
# Sat, 16 Oct 2021 03:01:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.8.1-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3c993d4c25d2ec8adbe5b497acc2226d8b6b602f68679037b8993f53617e2b`  
		Last Modified: Sat, 16 Oct 2021 03:02:27 GMT  
		Size: 1.2 MB (1186176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f063abb73e10805d2ce88263411405ffb32082608644c3d370a371c08dd6dd4`  
		Last Modified: Sat, 16 Oct 2021 03:02:28 GMT  
		Size: 16.2 MB (16169048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a180d646a584a0bc397aab545307b4db9745d4486ffce857d810c9638cd3f6c2`  
		Last Modified: Sat, 16 Oct 2021 03:02:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cba0dd022182c042a1f9be8465aeb11cac4821d860a6fbbca9c2505b4768738`  
		Last Modified: Sat, 16 Oct 2021 03:02:24 GMT  
		Size: 5.5 KB (5500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcf4ee730793921e8ce920ebc6d7d26ad55ce2f49822b633d7e69e244f33675`  
		Last Modified: Sat, 16 Oct 2021 03:02:57 GMT  
		Size: 274.9 MB (274900503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407dcbb2239e56ffbd65ceff1af8946167ca783954c107dca1ab34d6964a2231`  
		Last Modified: Sat, 16 Oct 2021 03:02:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1e3f14874392b4567445ce3b20e46c937f49d36dd46d6d862f0c9d77a5cbaa`  
		Last Modified: Sat, 16 Oct 2021 03:03:53 GMT  
		Size: 284.6 MB (284559839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
