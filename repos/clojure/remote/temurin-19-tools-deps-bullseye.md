## `clojure:temurin-19-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:b711acedff3ea114a852619c8c3a805f042fb23cafe6c6e01ef0b02e2833bfaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:be0a746a3da26da288e3e874cc13b1ceb28dc0b38d7da810bb3af4e053fb2343
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303192188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d3734e2c044ca0f8c3c58975ab627b7b0a423605547dd6ba085d65115051d8a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:42 GMT
ADD file:26702ba2c3e94cb21cdb3c550cf01cf848823d160f3417b559116d4c718e5df0 in / 
# Tue, 25 Oct 2022 01:43:42 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:32:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 02:42:31 GMT
COPY dir:49a4548ab030e4d26793e92b4d74537cf530961ce7b4083b8d383585c96415d5 in /opt/java/openjdk 
# Tue, 25 Oct 2022 02:42:33 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Nov 2022 20:27:31 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Thu, 03 Nov 2022 20:27:32 GMT
WORKDIR /tmp
# Thu, 03 Nov 2022 20:27:47 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 03 Nov 2022 20:27:48 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 03 Nov 2022 20:27:48 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 03 Nov 2022 20:27:48 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 03 Nov 2022 20:27:48 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:17c9e6141fdb3387e5a1c07d4f9b6a05ac1498e96029fa3ea55470d4504f7770`  
		Last Modified: Tue, 25 Oct 2022 01:47:28 GMT  
		Size: 55.0 MB (55046332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b6cdd3c4f04a6a611badcb0210b13df1430faf9e1bcbb3d09c250db0335722`  
		Last Modified: Tue, 25 Oct 2022 02:54:15 GMT  
		Size: 200.8 MB (200843786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c69df88bc8fd397166bf82f3bbb32885f3ba0c8aba35c08630715dd529a0ded`  
		Last Modified: Thu, 03 Nov 2022 20:38:23 GMT  
		Size: 47.3 MB (47301050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c36f399270d34652e0107e997c34cda979e47cf36eaa7ba397164d9e07f49f`  
		Last Modified: Thu, 03 Nov 2022 20:38:17 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe0605178871bb25485bed2c0f6a0586e6da0d0b4ff0ce83e9740777bce6887`  
		Last Modified: Thu, 03 Nov 2022 20:38:17 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:2f1157b4a3c9884c33e585e454b3752b43e3c67f4e5b448ce567dcb1a81f3281
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300579774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ac097753d505928af8aa59e8401b1d907156d6e73ebf4815f49c5a1bc744299`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 25 Oct 2022 05:45:55 GMT
ADD file:b16745ece8ef84c028d7e9ac4bf026ac64f885d4170bfcc9d435f237144a1b99 in / 
# Tue, 25 Oct 2022 05:45:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:53:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:48:52 GMT
COPY dir:2fc3a52010e404362374a6fbc2449d1ef85a3bc7bb00efe969cabc1864797789 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:48:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Nov 2022 19:48:01 GMT
ENV CLOJURE_VERSION=1.11.1.1189
# Thu, 03 Nov 2022 19:48:01 GMT
WORKDIR /tmp
# Thu, 03 Nov 2022 19:48:13 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1afd91b165776615eca84cce2271e5fe5d5818c55dee0f082b1304bb1464b3e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Thu, 03 Nov 2022 19:48:13 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 03 Nov 2022 19:48:13 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 03 Nov 2022 19:48:13 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 03 Nov 2022 19:48:13 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:8e1d92e7d04d2a9a9880cb45dc3c32c2805912cd86abed96d0ada3ff28748205`  
		Last Modified: Tue, 25 Oct 2022 05:48:40 GMT  
		Size: 53.7 MB (53701966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997f9b1128d353add7d065052afcf1047aea6a037bed4d3396015998ab5e3ca`  
		Last Modified: Wed, 26 Oct 2022 16:05:23 GMT  
		Size: 199.6 MB (199582421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6e2d7ce1462acce62065ae3ea910168a5d9d8ba2726a3eb7765ae9785a134e`  
		Last Modified: Thu, 03 Nov 2022 19:56:49 GMT  
		Size: 47.3 MB (47294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e61d3ecb673b70316e30472f553c042a6a6e4e1d4ae8cba5eff9d3563a27a85`  
		Last Modified: Thu, 03 Nov 2022 19:56:44 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b32daf1c4f1b60ca0120f0e5582d496401869ddac810bb4034dc399167fe525`  
		Last Modified: Thu, 03 Nov 2022 19:56:44 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
