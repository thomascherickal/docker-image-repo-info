## `clojure:temurin-8-tools-deps-1.11.1.1429-bookworm`

```console
$ docker pull clojure@sha256:2ec719f3b00d2dc27be85076666a6d4dd17dfcfc686117face34acd0ec10507b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-8-tools-deps-1.11.1.1429-bookworm` - linux; amd64

```console
$ docker pull clojure@sha256:e5c3d7b12feee7e09497d5ca29f34f726009188c02bc2e50c7225cb4f3d88b34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236760695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914a0b54fc75ca4fb7ab103ff5df5a6fdc354798ff5a89f2ee37e4c5fbe9ecde`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:07:35 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:08:27 GMT
COPY dir:a294625293e4e40913c98181a9aeff55bc5e737b728d424dfdc884f576bd8f8d in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:08:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:22:37 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:22:37 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:22:56 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:22:57 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:22:57 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafcc59647295681d6450f088ef58ed34e24d6971f2f1e50b101f7692733d612`  
		Last Modified: Tue, 21 Nov 2023 10:28:45 GMT  
		Size: 103.6 MB (103598261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b1a3e1478e38de75a1d9d9e200c40359b502133aa4aa9723c9a9ce58a4e499`  
		Last Modified: Tue, 05 Dec 2023 18:36:01 GMT  
		Size: 83.6 MB (83579592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13601bb83171f06de96af08dea2244dc351ff30637698832ce03910f188fb7d2`  
		Last Modified: Tue, 05 Dec 2023 18:35:51 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
