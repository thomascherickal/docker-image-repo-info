## `gazebo:gzserver11`

```console
$ docker pull gazebo@sha256:9db79b2a6732ada3f51b6957a9fa5ddd39a1446ffc8423b283ba76e8c2f18db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11` - linux; amd64

```console
$ docker pull gazebo@sha256:21dc590a8e5bf51a98c83b0ab23f3fe6fcd37791eb45bcf7c6e74d66aeb44df7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.8 MB (320830124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:482cb450a2a7476458432be66c3a5c32e175dd9a4603281cdd0daa4f0cae2bb9`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:03:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:03:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 01 Oct 2021 05:03:32 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 01 Oct 2021 05:07:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.8.1-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:07:05 GMT
EXPOSE 11345
# Fri, 01 Oct 2021 05:07:05 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 01 Oct 2021 05:07:06 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 01 Oct 2021 05:07:06 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc6e6d9419fa9dc8925c8ef5513c8b624ae911f333e21dd193d2b238ae510e9`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 16.2 MB (16168150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aa611f1de0da12c6d73920152d8cbce9c318169639e4ecb95d62a83406c442`  
		Last Modified: Fri, 01 Oct 2021 05:15:20 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc46b058b8fb9776dddeadb0ab830760bab8bebc42adc9b21c214fee670fdcb`  
		Last Modified: Fri, 01 Oct 2021 05:15:20 GMT  
		Size: 5.5 KB (5503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544162fa51ec2946fd4412e5fccd2da72397f73cebf8e8f82aef310e8d1d57bc`  
		Last Modified: Fri, 01 Oct 2021 05:15:53 GMT  
		Size: 274.9 MB (274902768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4890d9a0ac582f18d52f0230a5a5d13c690612ffe3f9076ad31e5f4d6b4f7336`  
		Last Modified: Fri, 01 Oct 2021 05:15:20 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
