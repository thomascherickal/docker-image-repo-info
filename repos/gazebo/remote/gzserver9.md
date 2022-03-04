## `gazebo:gzserver9`

```console
$ docker pull gazebo@sha256:ee3a67cf8aaa528aeac469c2cbe415c11ae0172969270f5dff56bca9653d2b15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver9` - linux; amd64

```console
$ docker pull gazebo@sha256:58b9842d05bc8e333fa3ee6221e6a8910acf3cf30d649aa16e6ad896003860a1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268423252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75aecfde48d1e96e06555a6cdc4718f33dcd786b7345947fd8218ed65e0eacd`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:25 GMT
ADD file:dee0aa8497bd26ca41dffa17adff99be2523f66f9b2c557ba9ad2388ed052dca in / 
# Thu, 03 Mar 2022 20:19:25 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 21:30:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:31:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:32:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Thu, 03 Mar 2022 21:32:05 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 03 Mar 2022 21:35:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:35:41 GMT
EXPOSE 11345
# Thu, 03 Mar 2022 21:35:41 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 03 Mar 2022 21:35:41 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 03 Mar 2022 21:35:41 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:cf06a7c3161117888114e7e91dbd21915efae33c2dbfb086380f7b21946d6e59`  
		Last Modified: Thu, 03 Mar 2022 20:20:28 GMT  
		Size: 26.7 MB (26708326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb61ec94593913764bceda6f5225dfb36c85ab821bba51cfc351aee5c0d15bf9`  
		Last Modified: Thu, 03 Mar 2022 21:53:03 GMT  
		Size: 838.9 KB (838912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4276f0dc6a17f9c686c83b0f8bd215ea26181b7e996be720b289a73d88f7fb4c`  
		Last Modified: Thu, 03 Mar 2022 21:53:03 GMT  
		Size: 14.7 MB (14705904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452e35840d9e58b24add9182745649616884eb9ce52f9029d555c895b56d1edb`  
		Last Modified: Thu, 03 Mar 2022 21:53:00 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac90876537df1343981631ec200ff8fab2c628270af64c51db3ee121f681eaee`  
		Last Modified: Thu, 03 Mar 2022 21:53:00 GMT  
		Size: 5.5 KB (5461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e6ec62b4d2a618db8151e052adb9c7e9c890b629d36175d0a3f0a935e44bac`  
		Last Modified: Thu, 03 Mar 2022 21:53:27 GMT  
		Size: 226.2 MB (226163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f3848c1a84e1d09df9d99b121725690d2ee41217c95a2931c127906ec07efb`  
		Last Modified: Thu, 03 Mar 2022 21:53:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
