## `clojure:temurin-8-bullseye-slim`

```console
$ docker pull clojure@sha256:eefbd52b96d606e6313b2256a3f7b49f55815d755e259f684c679de8e4c77179
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-8-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:fa424753c26d4b23393200c6421157a5a18467d42599abcfbb9095e726abee30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147550132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6c0f65f56c86c08af5909cbdb43b8717c040488ab3a38a2821fe8224ee8af80`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 08:11:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 08:11:18 GMT
COPY dir:bbb84183d7ea38d81d8401f01e29d08935ee4c8bf6f90c6527579a1554c3bde1 in /opt/java/openjdk 
# Wed, 12 Apr 2023 08:11:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 08:13:02 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 08:13:02 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 08:13:18 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 08:13:18 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 08:13:18 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f4a27a9e344c488df290d18697fb80bdb4bc2f7e4f2e7cb55c5f8b8c5b416b`  
		Last Modified: Wed, 12 Apr 2023 08:21:40 GMT  
		Size: 54.6 MB (54635556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d3136533247987ef00c4d993e0880d0197150d30055bd1e7c71a291b5d119d`  
		Last Modified: Wed, 12 Apr 2023 08:22:32 GMT  
		Size: 61.5 MB (61495732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e0c8957108f9a3184f6de643419b0ee8d7e6132b7fe7f7acf125fcec9780ed`  
		Last Modified: Wed, 12 Apr 2023 08:22:25 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-8-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:bf65830ce80768226e37658fc3831f49f92499bec29f423af74c2a183c8325e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145403016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef7af9c5f2c8a7e3abe5b5aef2869b6d536825611bc8ac9d87ed77cedf3a81f`
-	Default Command: `["clj"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 12 Apr 2023 01:18:46 GMT
COPY dir:b6d7e5613532d986930216de9e0fece0632e82564ce7a6a98baf63b4115f840d in /opt/java/openjdk 
# Wed, 12 Apr 2023 01:18:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Apr 2023 01:20:18 GMT
ENV CLOJURE_VERSION=1.11.1.1267
# Wed, 12 Apr 2023 01:20:18 GMT
WORKDIR /tmp
# Wed, 12 Apr 2023 01:20:32 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c949c9ba24ee46a2c57c6e6aeff262ebb0ff8112ee2367b3dbabd2f2df75380a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 12 Apr 2023 01:20:32 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 12 Apr 2023 01:20:32 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beeaea1bb320b3b40a83a6b31783cdc7af5081dd6683ffd28ef3a3b39f888ff`  
		Last Modified: Wed, 12 Apr 2023 01:28:11 GMT  
		Size: 53.7 MB (53727937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ce63753086f6e0643dffc71d44e76b23a7919a4766babd2de1f4d5c984a6fc`  
		Last Modified: Wed, 12 Apr 2023 01:29:01 GMT  
		Size: 61.6 MB (61610641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ca3e776de4ae5cb0af36572f4e00d670205b9592000d673aafb2915b168aae`  
		Last Modified: Wed, 12 Apr 2023 01:28:56 GMT  
		Size: 612.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
