## `clojure:temurin-17-tools-deps-1.11.1.1386-bullseye-slim`

```console
$ docker pull clojure@sha256:0b8d8766b6bb48f162aa40bf0eaa3c70e971eb3d104821a6e9295ecaeb3cae83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-tools-deps-1.11.1.1386-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:9e93a1a15a3c411078cf98e3f0057688d6f84869e6a0acf34e9b2e0363a58c2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.7 MB (237693598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683c988577dd0e9e45d09fd179cd1c6900b16733b71d0da29f136c7d9d5ef5b5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:22:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 20:17:57 GMT
COPY dir:8ea3eea47bd8b9d37ce2403b2d64b2cdc0fec836a119c10ec3e4ff0bcca8bb4d in /opt/java/openjdk 
# Tue, 08 Aug 2023 22:37:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 23:24:48 GMT
ENV CLOJURE_VERSION=1.11.1.1386
# Mon, 14 Aug 2023 23:24:48 GMT
WORKDIR /tmp
# Mon, 14 Aug 2023 23:25:04 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "3a09e2df4d3abd89b5b1286af0133a36a525ff3acfe1432f98b5c24b170940e8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Mon, 14 Aug 2023 23:25:05 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 14 Aug 2023 23:25:05 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 14 Aug 2023 23:25:05 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 14 Aug 2023 23:25:05 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8050892377b9a47e9c3a9ef290967338da628f34d31341e0efc181a16a685401`  
		Last Modified: Tue, 08 Aug 2023 20:20:46 GMT  
		Size: 144.8 MB (144773775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7c071f28219f66b0d7a2958f782c8367203befe9f3020c997b8dfca8f82698`  
		Last Modified: Mon, 14 Aug 2023 23:32:51 GMT  
		Size: 61.5 MB (61501206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8261673199dcf5692c4330cc97abe8ab51aa9869a9dc3c5528a79c8c478cd5a5`  
		Last Modified: Mon, 14 Aug 2023 23:32:44 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fc79944bab26ef967bcf8b1223c26921655dd067b5af7b33418bd0126e5fa`  
		Last Modified: Mon, 14 Aug 2023 23:32:44 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
