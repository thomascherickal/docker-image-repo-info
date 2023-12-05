## `clojure:temurin-8-tools-deps-1.11.1.1429-bullseye-slim`

```console
$ docker pull clojure@sha256:ba4fc9b400ef24a0bb675d02e66837857b823bec45e9cde9d65af20c2dabce74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-8-tools-deps-1.11.1.1429-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:181e512cc7c6f8a3783f69f48ce622727bf9028e5c755f86603dfce1b91db851
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.7 MB (196723316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6d070386205ba07a27ae281e199aa321726cca86852a19369627822e4c8e015`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:09:58 GMT
COPY dir:a294625293e4e40913c98181a9aeff55bc5e737b728d424dfdc884f576bd8f8d in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:09:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:23:50 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:23:50 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:24:07 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:24:07 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:24:08 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e607a1b241277667349406a3ca3eff66cf7b380f86e562b7d5416eccee3f02`  
		Last Modified: Tue, 21 Nov 2023 10:29:36 GMT  
		Size: 103.6 MB (103598267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016f0b757e04280c9da58629393c0252cc98a4589c20fac7d171a37b649d43af`  
		Last Modified: Tue, 05 Dec 2023 18:36:56 GMT  
		Size: 61.7 MB (61706604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc924bd883b29998d496e04d8a323b41c2a75b5a09b111c708965fb7487944b`  
		Last Modified: Tue, 05 Dec 2023 18:36:49 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
