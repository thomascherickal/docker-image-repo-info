## `clojure:temurin-20-bullseye-slim`

```console
$ docker pull clojure@sha256:e4529f31ce60ca3db049e31dbc3d696c862ee53af9bc764ce3e3afb1b6643938
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:d40594d089db55ace34335139c9cdad6fe331c22d1a5a5a91062daf04b54c228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.7 MB (295715511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630d70468d6a0971dce87ece6fe0a65c0eadf86f631cbfdd24154d794893f7cb`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:19:17 GMT
COPY dir:0f9b663d61413099f20817ab55258941c09987290b8ce360d0fb2fab00ddddda in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:19:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:20:01 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 08:20:01 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:20:17 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 08:20:17 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 08:20:17 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 08:20:17 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 08:20:17 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b32b49a5ad9ee1b838c8a414680cfb573b6bf63d15cefb9f67402b317700b6`  
		Last Modified: Wed, 12 Apr 2023 08:26:44 GMT  
		Size: 202.8 MB (202800600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf8a1991dc4ebccacc4def55f8357b7f493066404b46feb7e949aaad4541ed9`  
		Last Modified: Wed, 12 Apr 2023 08:27:19 GMT  
		Size: 61.5 MB (61495667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8fceff7d75f3fd90d62a576d014ffc1a0b794566390dd47b33923ea3b29a03`  
		Last Modified: Wed, 12 Apr 2023 08:27:11 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc54e66be8e145a43dc6bc9c3b0050121dfa6bb3c9905e1342e1302a63d0b05e`  
		Last Modified: Wed, 12 Apr 2023 08:27:11 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:887cd59378a58e56fa37044cee1b17f4a48fb02ca93dcde275f9d6d4afb9bd2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.8 MB (292835396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eacac59b916290a3a0e8db1cc3f3e3844cec9261f5f9aacebbe41cf76a937b87`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:25:57 GMT
COPY dir:66b65f1974fed4b5bc3675e6b378c93a3ba9feeabfec7eeabd6d1d0b07fd5fa4 in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:26:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:26:44 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 01:26:44 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:26:57 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 01:26:58 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 01:26:58 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 12 Apr 2023 01:26:58 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 12 Apr 2023 01:26:58 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ac14b41f3aaaeba0605fc04f599b4365bfd232c1b3f11a8c1c5c7c4cceaa9b`  
		Last Modified: Wed, 12 Apr 2023 01:32:54 GMT  
		Size: 201.2 MB (201160129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efa70c1f1b0b5738ed715809bbd678ad022957dfb4546bdca8c99a56c9c7a24`  
		Last Modified: Wed, 12 Apr 2023 01:33:26 GMT  
		Size: 61.6 MB (61610427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504854ca047e7a125b059e55a0430ee9b90e3b0ae6bc6a79d34b5737d9fbf72e`  
		Last Modified: Wed, 12 Apr 2023 01:33:20 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c02d605e6116d870b98e71af8686474aede8e1eadb57e7a594b31bd81655818`  
		Last Modified: Wed, 12 Apr 2023 01:33:20 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
