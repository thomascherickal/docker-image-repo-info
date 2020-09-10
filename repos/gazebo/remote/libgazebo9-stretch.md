## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:6d6372f3586e3d32ff5f192c1fd38eb215e8ecf281adbd2821e8886a6ffedd34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:090ff736c1d4d3cc65fdc7b1a6b88ff406453787616aaf6b38fbcdbb0903a336
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.9 MB (569882453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:219fb259696f5eb81eae5a858b581a889c4b6748b7014522d4b02ee55fc7cdb2`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 05:40:25 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 05:40:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Thu, 10 Sep 2020 05:40:29 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 10 Sep 2020 05:41:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.14.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 05:41:31 GMT
EXPOSE 11345
# Thu, 10 Sep 2020 05:41:32 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 10 Sep 2020 05:41:32 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 10 Sep 2020 05:41:32 GMT
CMD ["gzserver"]
# Thu, 10 Sep 2020 05:43:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo9-dev=9.14.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dcc12496391485e9809615cfcd2938af53d7c813909bf3a4e27b71aaa81633`  
		Last Modified: Thu, 10 Sep 2020 05:44:30 GMT  
		Size: 18.5 MB (18515141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50266b329110929cbbaaed679354348702002842555979a900e8efb4ad8d8a10`  
		Last Modified: Thu, 10 Sep 2020 05:44:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261b81a9923ffb06a1aeea39dd3de22d7c9b36ab43604fa91fb71a2213651a02`  
		Last Modified: Thu, 10 Sep 2020 05:44:22 GMT  
		Size: 5.0 KB (4984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f14d12dfa8ee0385ac5c6f3d71ddeb6ba5fe158248c4237b838f402eda8c61`  
		Last Modified: Thu, 10 Sep 2020 05:45:02 GMT  
		Size: 202.1 MB (202070285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e655cb9e364ff32c993c304d598310a8a335e4259e147d967f6ac2d309b162fb`  
		Last Modified: Thu, 10 Sep 2020 05:44:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affeed96611110e679292558872ce45c2df9be416ea147b838d17418c8ad9f80`  
		Last Modified: Thu, 10 Sep 2020 05:46:12 GMT  
		Size: 303.9 MB (303923708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
