## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:a4405e3de6217f83473b1d6ef42206dbd3054f445807afe70003c794ca6a80fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:345e44acfef0241eb8aca22715a84f6e7ee738538d0106cb9aaab2045ec4a974
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.8 MB (277801581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4fc099b2b015e111f07cac73b9b0d24c30b4526e9439d6624869a0f98bc7bf`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:55:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:55:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 02 Sep 2022 02:55:31 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 02 Sep 2022 03:01:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.11.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:01:20 GMT
EXPOSE 11345
# Fri, 02 Sep 2022 03:01:20 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 02 Sep 2022 03:01:20 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 02 Sep 2022 03:01:20 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c2f193a51cd0afec561c749fe8ca94db1dbd5dd0889044530e2e627ea87d63`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 14.7 MB (14709235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364bd7888a65fc5650010670936211e76efef4b32bb6316216e3a86d40c69e2b`  
		Last Modified: Fri, 02 Sep 2022 03:12:59 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadb91965c06a226e79402d88cba56f1c093e69450135088903042cfe9da2a7`  
		Last Modified: Fri, 02 Sep 2022 03:12:59 GMT  
		Size: 5.5 KB (5460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5f6f00d00ffde17e746e5192a435464bd62f4e354809783e72deafb6a26ea1`  
		Last Modified: Fri, 02 Sep 2022 03:14:41 GMT  
		Size: 235.5 MB (235544185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774affbe83c47dc0f529328d31abeecf9b9806303574180b040aee313fd367e`  
		Last Modified: Fri, 02 Sep 2022 03:14:13 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
