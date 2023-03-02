## `gazebo:gzserver11-focal`

```console
$ docker pull gazebo@sha256:d068f8569f1d7fb04718c1d8d65b0bfa27e24e60c1999bbbb2558b14bf82e6d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:c303a3ca23afaef13214e0f4ee169a4cf26523166613b4d7151b99e89c15bc5f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321936547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ac37df6bcce767df745353d8705dbc7225e26621cbb6f2e26ca50dc378f9e5`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:22:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:22:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:22:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Thu, 02 Mar 2023 04:22:34 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 02 Mar 2023 04:25:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:25:44 GMT
EXPOSE 11345
# Thu, 02 Mar 2023 04:25:44 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 02 Mar 2023 04:25:44 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 02 Mar 2023 04:25:44 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f28384e69de3a0ea100a44034714a15f9f49315877d90900c17f82a44ad96`  
		Last Modified: Thu, 02 Mar 2023 04:32:04 GMT  
		Size: 1.2 MB (1154579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a482f33eafe48f47fef0612e78afc14bfc54e6a6b635c3449c84b6ef6efe0941`  
		Last Modified: Thu, 02 Mar 2023 04:32:05 GMT  
		Size: 16.2 MB (16177976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b928a439c7363b6bd0942ea8cd50ad331e1e5dfacaa64d70710427130b606c2`  
		Last Modified: Thu, 02 Mar 2023 04:32:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39117f99fadbf50aa22249839c901651488c04ec44c52ba5ad38013143597d3`  
		Last Modified: Thu, 02 Mar 2023 04:32:02 GMT  
		Size: 5.5 KB (5505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb610ecbec9d61eba80d3d769728a110c2a4c2a0a0c2c46daf78d336f482710`  
		Last Modified: Thu, 02 Mar 2023 04:32:33 GMT  
		Size: 276.0 MB (276018859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fa1eb5bc41d068fcae5c9392af16818b701a65f3f82566f1cd125a75f1333b`  
		Last Modified: Thu, 02 Mar 2023 04:32:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
