## `gazebo:gzserver9-stretch`

```console
$ docker pull gazebo@sha256:ed3abb45296162f3e9f01b17aa9332834f5bec3e830584acb29e70ff6fc38c18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:3e003070f91adc4ee1e1784d3798008a29ad41c3276e2dacb955301ad919bfbb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (265958745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0563d59b0956698c1b80e4b884ab41216ccd2b93a9a279171d77e0df83fb7688`
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
