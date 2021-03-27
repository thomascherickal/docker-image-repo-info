## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:3656199c59f7e03b6eb3b2b1f76079e9a157dab1b9f05ae597af7cf8db512313
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:cf7072fca9df25c2f1447098ca4a69285414ad36cabd553e5a216285692ce411
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **570.3 MB (570253015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1946a4e5ab2ce443c2d1d2911c8a0636ed70194d93888de0253dc2299f717140`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:17 GMT
ADD file:f7a6b2066de76eb559d8ab8bf8972d519c3b4dcafc62e46253227559091f7c8f in / 
# Fri, 26 Mar 2021 15:23:18 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:50:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:50:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 27 Mar 2021 04:50:36 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 27 Mar 2021 04:51:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:51:48 GMT
EXPOSE 11345
# Sat, 27 Mar 2021 04:51:48 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 27 Mar 2021 04:51:48 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 27 Mar 2021 04:51:49 GMT
CMD ["gzserver"]
# Sat, 27 Mar 2021 04:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dfe7e1e1bffb84b5330514880896199259b01ebe2b9d531dd88f7ce7db8cd18`  
		Last Modified: Fri, 26 Mar 2021 15:32:18 GMT  
		Size: 45.4 MB (45379513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6991bbdde750310014591f0ea38c3948d0b10b17a4335ca0534cc4b13755be`  
		Last Modified: Sat, 27 Mar 2021 04:54:57 GMT  
		Size: 18.5 MB (18512473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80080bc5a77ef0d0fda04203730723bf5857aba6e596a0eeebccb945c05e396`  
		Last Modified: Sat, 27 Mar 2021 04:54:48 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53418e5a6f29f8a6095df153332b47554745496dec0c43648bcce335d47323d`  
		Last Modified: Sat, 27 Mar 2021 04:54:48 GMT  
		Size: 5.0 KB (5016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b77d68449be56c1d29621c8af6185c7192ec98f666d953aa28f2d2be823f1f`  
		Last Modified: Sat, 27 Mar 2021 04:55:15 GMT  
		Size: 202.3 MB (202283482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc45f698bf4302981fc5e7c0dce3d519b2b3640f6889bff40622555c32cda954`  
		Last Modified: Sat, 27 Mar 2021 04:54:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224bc61ac07ce76ff4aeafb7c24d7fd15b4f8f265e164e684b6af38da402c998`  
		Last Modified: Sat, 27 Mar 2021 04:56:29 GMT  
		Size: 304.1 MB (304070923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
