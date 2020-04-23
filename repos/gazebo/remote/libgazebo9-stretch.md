## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:403a8229790daa8c46e6ec925875a4c5ad7210f1d49b5aca69ebd4d13c7d6af7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:4d37d3d51460de5711c218290bc8ec70552d7027148c47db72e5ebe15ffbbaef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **651.0 MB (650966527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce9553c75eebdb5347cc8550f000e9bf3629783fd4b432c2eaed870e9b8d9b86`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:42:38 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:42:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Thu, 23 Apr 2020 01:42:42 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 23 Apr 2020 01:44:00 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:44:01 GMT
EXPOSE 11345
# Thu, 23 Apr 2020 01:44:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 23 Apr 2020 01:44:02 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 23 Apr 2020 01:44:02 GMT
CMD ["gzserver"]
# Thu, 23 Apr 2020 01:45:32 GMT
RUN apt-get update && apt-get install -q -y     libgazebo9-dev=9.12.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34502294a02bc4b5c87766699f13475a1f7403335fd2821ab6fc1b3ec5ba3d7c`  
		Last Modified: Thu, 23 Apr 2020 01:46:15 GMT  
		Size: 21.1 MB (21095000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f91f9850ce1646beddf2640422d469d00b3bf4e412306a90fcd63331adfb41c`  
		Last Modified: Thu, 23 Apr 2020 01:46:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983d13ecad407e0bb4bd2e197bbc7afa28e75467becfbd82e5e917e6c3b4793e`  
		Last Modified: Thu, 23 Apr 2020 01:46:10 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5406926b69455e0c8280ca6a3673804030a8979279d8200b701c8bab92089e`  
		Last Modified: Thu, 23 Apr 2020 01:46:53 GMT  
		Size: 279.9 MB (279871200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e5b376e643b770370ae9291c4bd1cab32b385fccfa0b5406f1cdcc13c82f8d`  
		Last Modified: Thu, 23 Apr 2020 01:46:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401a6bfd471f0a3ddfb51025e7934b97e9ca1a68e5a0c06b93341af1b5cb5c89`  
		Last Modified: Thu, 23 Apr 2020 01:47:55 GMT  
		Size: 304.6 MB (304617787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
