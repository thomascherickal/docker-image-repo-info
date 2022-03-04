## `gazebo:libgazebo11-focal`

```console
$ docker pull gazebo@sha256:10be87cafc6d924abcf1badb43cd1409857fe19692b166e8c5473480e6647722
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:85a86d6b318defbff6e1570a875cf8b7e01d9eb66e00cefea5734703128f8de3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **606.4 MB (606449771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446e1107f3e05b12c023889c948780058139f6b2ed48e0a37678546019207969`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 21:42:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:42:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Thu, 03 Mar 2022 21:43:33 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 03 Mar 2022 21:47:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.10.1-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:47:15 GMT
EXPOSE 11345
# Thu, 03 Mar 2022 21:47:15 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 03 Mar 2022 21:47:15 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 03 Mar 2022 21:47:15 GMT
CMD ["gzserver"]
# Thu, 03 Mar 2022 21:52:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.10.1-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806bc8c3926ddb263b6e70eea4ef851e3f5bd20b4b6b9c1735d783a6bf212115`  
		Last Modified: Thu, 03 Mar 2022 21:55:36 GMT  
		Size: 1.2 MB (1182245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777af385870cbde187884431606963e9e7da9006f37c45d53b09ea7aaa084857`  
		Last Modified: Thu, 03 Mar 2022 21:55:36 GMT  
		Size: 16.2 MB (16170690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1191de856a8b397c3e059ef7cdcffed99183c450f233823c942f60ebc65bf3`  
		Last Modified: Thu, 03 Mar 2022 21:55:33 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ed3fec4ea73903419c76599377d1ec5ff4f4a74d8fd1302e5295985686271d`  
		Last Modified: Thu, 03 Mar 2022 21:55:33 GMT  
		Size: 5.5 KB (5500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a47c2a676f86d2285c718db65746847191ed2bc067545b7018be9ef4bfdf88`  
		Last Modified: Thu, 03 Mar 2022 21:56:06 GMT  
		Size: 275.8 MB (275848522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c447641436fee143acbfad38085616e3780b529ac4b26b4750e15bbdb598d795`  
		Last Modified: Thu, 03 Mar 2022 21:55:33 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0238f1f3d12234533270f9e5abde336d20d749021996f470c3329823c35859b`  
		Last Modified: Thu, 03 Mar 2022 21:57:03 GMT  
		Size: 284.7 MB (284675434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
