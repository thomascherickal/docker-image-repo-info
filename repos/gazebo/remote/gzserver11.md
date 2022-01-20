## `gazebo:gzserver11`

```console
$ docker pull gazebo@sha256:2cd7feb17d03c8a910eabe7d44ff2ff1ad448018c63313e03ba5a99c2cf899e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11` - linux; amd64

```console
$ docker pull gazebo@sha256:06e1dfc9f30e226cdf219ef32c39d33b4fc6309bfbefad71801ec551feec192e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.9 MB (320942974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a22aa9d9ffd767bf476eb2e024307b5c730c848eec1c151813e9d56f9d93d541`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 04:09:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 05:15:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 07 Jan 2022 05:15:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 07 Jan 2022 05:15:38 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 20 Jan 2022 03:39:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 03:39:28 GMT
EXPOSE 11345
# Thu, 20 Jan 2022 03:39:28 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 20 Jan 2022 03:39:29 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 20 Jan 2022 03:39:29 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d6b806a5eae974734f3df21a5799c46db4c8dc12ffc6bab4a8ca2f802d1b5`  
		Last Modified: Fri, 07 Jan 2022 04:34:49 GMT  
		Size: 1.2 MB (1182238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c0bba77aa7d24282d153e2a02032e5484ee8a5ca1879eb9ff0e473a7f3ff7c`  
		Last Modified: Fri, 07 Jan 2022 05:25:43 GMT  
		Size: 16.2 MB (16169890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fadef1dc985611b2e7adc1e486b110f8d89368e6e69b7393a4f7581b354ef6`  
		Last Modified: Fri, 07 Jan 2022 05:25:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae5a366fc56bde9f5c014cd333b5cd60218fddd6d1d1f03bb707df6c5acb7f`  
		Last Modified: Fri, 07 Jan 2022 05:25:41 GMT  
		Size: 5.5 KB (5502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670f0697cb7354802d7fecfcbe2777b10da37e4f6c179d79d3a742ae098872a4`  
		Last Modified: Thu, 20 Jan 2022 03:47:22 GMT  
		Size: 275.0 MB (275017292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40491f4f9540a8248011146698f9483d5a5116286d6791fbf3531e22deec5cae`  
		Last Modified: Thu, 20 Jan 2022 03:46:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
