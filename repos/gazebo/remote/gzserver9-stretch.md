## `gazebo:gzserver9-stretch`

```console
$ docker pull gazebo@sha256:4a1329b2442382ade2673c2ebb2a6d5cb2b48541a490401c4b49a0eb94722e07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:9b1e77d96d0134e6ac8b7cf00b73668d25444c94749164bcd0cf2e553045f112
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.3 MB (346348740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94346110a6c3c013e03f5462f48c74107a18d5ba76fe5f2c27bd27b4c99f3be0`
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
