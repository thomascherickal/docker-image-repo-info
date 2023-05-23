## `clojure:temurin-20-bullseye-slim`

```console
$ docker pull clojure@sha256:268c33178a7b98ff3de5390c9b905ea35fd099a3ad79e142b42f40a004917ffc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:d5875d8a1421264852441f68ff8ae31c41a9285ed89ae86e14c319df5fea0f91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.7 MB (295713184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8007153b8ae8ef7d4a15c8e2c000a2ebb2242a680648c815c866e577c6a82324`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:43 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 03 May 2023 20:32:51 GMT
COPY dir:02736280d197ac4d1b6ebf68d948efb46e7eeffd579505356f8c94946dbcce6f in /opt/java/openjdk 
# Wed, 03 May 2023 20:32:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 May 2023 20:34:34 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Fri, 19 May 2023 20:34:34 GMT
WORKDIR /tmp
# Fri, 19 May 2023 20:34:49 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 19 May 2023 20:34:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 19 May 2023 20:34:50 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 19 May 2023 20:34:50 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 19 May 2023 20:34:50 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02720e2873c980e5fcc584b01ace091e5d4d05cd22a426e5b195f3d93f338875`  
		Last Modified: Wed, 03 May 2023 20:40:25 GMT  
		Size: 202.8 MB (202813964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb0abf726f5d0322c2875c22f54aeab06b946e90fa93e1222df003adc811ac7`  
		Last Modified: Fri, 19 May 2023 20:45:05 GMT  
		Size: 61.5 MB (61494688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6b018c378abca64344fb2c2a88427a5cae24c60d8d75616ee9e9c0206c3437`  
		Last Modified: Fri, 19 May 2023 20:44:57 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb8da39f4ebe094b83ea7d6b4e7be86b98427156cc694edde6d6c47aff84008`  
		Last Modified: Fri, 19 May 2023 20:44:57 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b4f7b0268d3d49ffd4bc49e8499b9c864dcb76fc7a8eb327bf0d2b71b1f8b260
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.8 MB (292820549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32ffd210f027d95f2b41ba8846ea988806319b9a83035cc58460d4e084322ee`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:32:09 GMT
COPY dir:f555428af67a610819205eec573e23f479077e0999818ee9dc0f3375599d21db in /opt/java/openjdk 
# Tue, 23 May 2023 01:32:13 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:32:48 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Tue, 23 May 2023 01:32:48 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:33:01 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 23 May 2023 01:33:01 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 23 May 2023 01:33:01 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 23 May 2023 01:33:01 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 23 May 2023 01:33:01 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a408f7150c3feef58c3abe2b486974c10a4d64c30a1c85440e6c6590693f6963`  
		Last Modified: Tue, 23 May 2023 01:39:01 GMT  
		Size: 201.2 MB (201157995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c0a54e84eac529981d2ebba55c2f0260e5443e50cacb3b766230fa05065f69`  
		Last Modified: Tue, 23 May 2023 01:39:32 GMT  
		Size: 61.6 MB (61608795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4f0b0df74fd7d891c2c8fc016b3e7969a36f051629f13299ff6f3113c89f03`  
		Last Modified: Tue, 23 May 2023 01:39:26 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4eae21936d8f8e7fea05c56908d5d3e7cd4712f4526f8aa45d95a7b9f1252b`  
		Last Modified: Tue, 23 May 2023 01:39:26 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
