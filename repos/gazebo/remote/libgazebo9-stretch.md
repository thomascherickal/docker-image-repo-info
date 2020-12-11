## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:5531bb8cd76ce10c6280bc956fe8054389557d619b2ffc84d74fb12c3316b9ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:6f1ec463e37307c6493ea9ca64f48a3fe484c636fba26ceae5d89760a03ae794
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **570.2 MB (570167020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1aa9fc0fac5ec3df6e3d1c15e168f3f77ddf067db5d2dd255882f589b5b8706`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 11 Dec 2020 02:08:43 GMT
ADD file:c3a852d22b3aac160ba028af69d56b491a2a9419f32a459c4b9b2cbd9129c004 in / 
# Fri, 11 Dec 2020 02:08:43 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:34:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:34:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 11 Dec 2020 16:34:04 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 11 Dec 2020 16:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:34:49 GMT
EXPOSE 11345
# Fri, 11 Dec 2020 16:34:49 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 11 Dec 2020 16:34:49 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 11 Dec 2020 16:34:50 GMT
CMD ["gzserver"]
# Fri, 11 Dec 2020 16:36:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22f9b9782fc328ea8192a309b7517c33b1c786697804153ed52a03005919f659`  
		Last Modified: Fri, 11 Dec 2020 02:15:19 GMT  
		Size: 45.4 MB (45377606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eff6b4d6547602661dde82fe6e7bc2bface2cf3acd1d3c9dfa1373408bc3b69`  
		Last Modified: Fri, 11 Dec 2020 16:37:22 GMT  
		Size: 18.5 MB (18508215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65750c7c3a67ec7fb698c9e08f2a48da2a511beeec59a15dcfcff9566db9dc69`  
		Last Modified: Fri, 11 Dec 2020 16:37:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bd07458d4c03b374e1cd43ed87aea4cb222df3a1a078aea068c42711a36e7a`  
		Last Modified: Fri, 11 Dec 2020 16:37:17 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893bad2bda146582aaf3843c3f38c007e88297a00446216a1ed87eea6402203f`  
		Last Modified: Fri, 11 Dec 2020 16:37:45 GMT  
		Size: 202.3 MB (202270856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54dfaca2cb4a9da7427455de84dbffbadeb58cbcda893ab274d4dcad0f62b17`  
		Last Modified: Fri, 11 Dec 2020 16:37:17 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf2f7995d0e1f26ce84c476796e9b9f5d1219ff9ef869c2a181de153004b980`  
		Last Modified: Fri, 11 Dec 2020 16:38:39 GMT  
		Size: 304.0 MB (304003753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
