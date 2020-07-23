## `gazebo:gzserver9-stretch`

```console
$ docker pull gazebo@sha256:4b670af9f10655501877e12cf0ba1409b90463851224b155f3f499aab9a8ad22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:cef5499d6759a861ec781da81c33138d462f73aecfd3964a3890f9609c5f2bc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.9 MB (265871238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33fd0cd38a912f0ba5e5ba98baf45bf5e08bb7fd13182662c688e3480cce0570`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Wed, 22 Jul 2020 02:06:48 GMT
ADD file:f98fe3d719ea765cb59da025d506d0bbd6db7a842b6b63c58c8d4d65b51bdb1f in / 
# Wed, 22 Jul 2020 02:06:48 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:07:24 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:07:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Wed, 22 Jul 2020 20:07:30 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 23 Jul 2020 10:23:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.13.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 10:23:49 GMT
EXPOSE 11345
# Thu, 23 Jul 2020 10:23:49 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 23 Jul 2020 10:23:49 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 23 Jul 2020 10:23:49 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7e6d8ed603557d9bf077a9ace4ee506501970a4938b9a704f040ad15f22bd4e8`  
		Last Modified: Wed, 22 Jul 2020 02:12:13 GMT  
		Size: 45.4 MB (45369674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4411483707592dcbac4314bc6194422b5b610683b5131926b750e3cbe20602`  
		Last Modified: Thu, 23 Jul 2020 10:28:29 GMT  
		Size: 18.5 MB (18514095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0dad0c2e98fc85f183e39744e915ce3092535269bc6dbad7a2c9c10f6db53b`  
		Last Modified: Thu, 23 Jul 2020 10:28:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10f94ffd189798ed034f2f550bfa7dc551f941f787e3d79b8e2a1d8b3e95e56`  
		Last Modified: Thu, 23 Jul 2020 10:28:25 GMT  
		Size: 5.0 KB (4979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11cdf511ee14cfb3e4d0d1f1d818a9c0697d7f1c26b2863d4e3150d10e4874`  
		Last Modified: Thu, 23 Jul 2020 10:28:52 GMT  
		Size: 202.0 MB (201980881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250ff4fbe3764f76e0b5c60de30521e67122cf9c39b8d5113e6c9755e1669435`  
		Last Modified: Thu, 23 Jul 2020 10:28:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
