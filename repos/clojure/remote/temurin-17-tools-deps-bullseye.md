## `clojure:temurin-17-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:4b626812cb1f6bfe1fb2127ee2179a19a3c7f262926f5bf250bbae6da9b8cbae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:be72fd6e2b32e94f5426d2f52d826c83e64ad39163897dc74558165bc5053406
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.4 MB (319371846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353a5e71d191579bf0b922ab9335af5c68adc190d0e9352dbf4e9a411ea043f5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:10:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:16:11 GMT
COPY dir:d90c8d6564183f8aad11f93ecfb2f7e0eeff18588ff2b62d7ca3d8d30672bc2c in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:16:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:18:02 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 08:18:02 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:18:19 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 08:18:19 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 08:18:19 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 08:18:19 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 08:18:19 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc37eb9b838f833285a35e624da1bfed81e650837c6751e8a6812e51ef22b6ba`  
		Last Modified: Wed, 12 Apr 2023 08:24:36 GMT  
		Size: 192.4 MB (192438264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7cb12bcfd2f511d719bc87692a96443d02a7a423cf542739e7b76a81c4f021`  
		Last Modified: Wed, 12 Apr 2023 08:25:38 GMT  
		Size: 71.9 MB (71879829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120ff4b53d5ca84591aa88ceaa59f5c1fc1a5cc2d7f70fd02632003795ece81b`  
		Last Modified: Wed, 12 Apr 2023 08:25:30 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6a2a2fc31515f0fe71369d2a2ab3714d7a789e6eedce682b39c3e7fed06a5a`  
		Last Modified: Wed, 12 Apr 2023 08:25:30 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:009278883e2e195b93c1e4e57bf5c9ec40198f0fc542224117b2b8685b1b4d84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (316963349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29fc16da990f36fe29512b80eb49194ac70b9863fd63cd9aefb99145e8329a1d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:23:04 GMT
COPY dir:44544f5117ae50af040f98b1979efcc18f4c9f0c7257bfc4a37b80697337361a in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:23:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:24:55 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 01:24:55 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:25:08 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 01:25:09 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 01:25:09 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 01:25:09 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 01:25:09 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6911e57ac771aafcbe41270c1285de884dc5ce0d79a1b3069ec89c3a65e4a6c2`  
		Last Modified: Wed, 12 Apr 2023 01:30:58 GMT  
		Size: 191.3 MB (191260417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16db0df5dd0c7f540af3ac1bc3af1e99bbe667409046b8617313f4ec259d8da1`  
		Last Modified: Wed, 12 Apr 2023 01:31:53 GMT  
		Size: 72.0 MB (71996390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed925c6a2510c607fe50be2b6397b9722f7197fc4f2e094875cd3fdf5103d5e`  
		Last Modified: Wed, 12 Apr 2023 01:31:47 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fed5c29ef66a36494e8fa1397dc627ea683df98a69a93255b9099e7c7afe3a`  
		Last Modified: Wed, 12 Apr 2023 01:31:47 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
