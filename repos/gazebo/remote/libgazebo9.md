## `gazebo:libgazebo9`

```console
$ docker pull gazebo@sha256:f8c4d273244e8cb44cd38f10464762739da78f5d96873c3f07eb206a77358704
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9` - linux; amd64

```console
$ docker pull gazebo@sha256:2b72d7397bb03ab5cec17fe89c50e924c4c1663e4e1acc073f5d191757f929ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.7 MB (413688094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d08c9ff58594acb840e35f6f6a9777bfb9c85dc2cc9b0687ef49c59e8fddf28f`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 18 Jun 2021 01:23:35 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 24 Jun 2021 19:26:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 19:26:48 GMT
EXPOSE 11345
# Thu, 24 Jun 2021 19:26:48 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 24 Jun 2021 19:26:49 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 24 Jun 2021 19:26:49 GMT
CMD ["gzserver"]
# Thu, 24 Jun 2021 19:30:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c9bccca2de788969af6d6e387abb084c66ce0679c41ca4712bf3787173a3b8`  
		Last Modified: Thu, 24 Jun 2021 19:43:56 GMT  
		Size: 14.7 MB (14702322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97918488cc093177c1052f8a9ec4c7729f138fe79a40137d1a3198f8ac2de6e`  
		Last Modified: Thu, 24 Jun 2021 19:43:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389903f5c318711646c39cd700afeaea7d7beac2750a1953f8325917e500ffcb`  
		Last Modified: Thu, 24 Jun 2021 19:43:53 GMT  
		Size: 5.5 KB (5459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d833541b4efd32f93e931bbd138973f3c6c173113266144ecbd116aed542732`  
		Last Modified: Thu, 24 Jun 2021 19:44:21 GMT  
		Size: 226.2 MB (226164197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9bb6f615487f4190e53e2c0cc522ed3cce6e58609199f751d42af761c383ca4`  
		Last Modified: Thu, 24 Jun 2021 19:43:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec36b18c0ff1c64d2853e54a021fc831cac767c5833b4e32cfe0c2723637850`  
		Last Modified: Thu, 24 Jun 2021 19:44:57 GMT  
		Size: 145.3 MB (145272531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
