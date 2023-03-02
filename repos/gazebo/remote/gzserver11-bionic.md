## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:0074ec442929107dbd735cb721156fc2fceb8ae14885270c8e1844a2d949e15b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:75bb398abb4e2ab7620d9c656c7d676c5beb7d00595c0114d8f3e35e48daec4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.8 MB (277833171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0f1cb08a141a5330c2727dc687f7a82ad9bc1bc0ef21cbbcbe0f9255d2da89`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Wed, 01 Mar 2023 03:18:00 GMT
ARG RELEASE
# Wed, 01 Mar 2023 03:18:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 03:18:00 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 01 Mar 2023 03:18:02 GMT
ADD file:66eb2ef5574cdf80bc0cb3af1637407620c1869f58cc7514395e3f5aea45cc3b in / 
# Wed, 01 Mar 2023 03:18:02 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:14:06 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:14:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:14:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Thu, 02 Mar 2023 04:14:40 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 02 Mar 2023 04:17:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:17:49 GMT
EXPOSE 11345
# Thu, 02 Mar 2023 04:17:49 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 02 Mar 2023 04:17:50 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 02 Mar 2023 04:17:50 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:0064b1b97ec0775813740e8cb92821a6d84fd38eee70bafba9c12d9c37534661`  
		Last Modified: Wed, 01 Mar 2023 13:18:18 GMT  
		Size: 26.7 MB (26711153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778654c0b435df260fd94e3a713e5ac0391d850b1dd50fc06d28724d697fd461`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 819.0 KB (819000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede19f20c058f051b81244f7348c285e3937b97ba0364ae0de6f5d97e24281ff`  
		Last Modified: Thu, 02 Mar 2023 04:30:48 GMT  
		Size: 14.7 MB (14712820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0151dfa1ea581dd7205a96f7895b0df4983be251f7ae7a74e770c7362ce69798`  
		Last Modified: Thu, 02 Mar 2023 04:30:45 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f9c2ea1ce65952de4cc2bab676821713fa9de09930550dc2bd8fd036413f4f`  
		Last Modified: Thu, 02 Mar 2023 04:30:45 GMT  
		Size: 5.5 KB (5460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a2c6549d5fbc980849ae259f16e830df3d2b4380787dc38bf1b00107a6e45`  
		Last Modified: Thu, 02 Mar 2023 04:31:13 GMT  
		Size: 235.6 MB (235583111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c35139592827422355ab2ade88c65e350f63b824362ce2ee0fca4d100270c2f`  
		Last Modified: Thu, 02 Mar 2023 04:30:45 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
