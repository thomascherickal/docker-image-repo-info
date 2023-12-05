## `clojure:temurin-17-tools-deps-1.11.1.1429-bullseye`

```console
$ docker pull clojure@sha256:268c239390a70f5479122e8af36eaf471e0e9c450858473340f4d7822e58be7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-17-tools-deps-1.11.1.1429-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:4110a2e8e4863fd1deb5c3d3986e20f2caddb65680f3a3700cbd48988a06ec2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.0 MB (272029265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ad1c172286b51223aef24aeca7225de04e2800351e0e7a01a9d69c2883e5a76`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 10:02:53 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Sat, 02 Dec 2023 10:02:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:29:45 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:29:45 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:30:02 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:30:02 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:30:02 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 05 Dec 2023 18:30:02 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Dec 2023 18:30:02 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a35d66848e01a74b7790ea370bb493db47c5518cd5c088ad8d2bf98e4e7b617`  
		Last Modified: Sat, 02 Dec 2023 10:18:57 GMT  
		Size: 144.9 MB (144873962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466322cfaff00d74dec349690bd93968913052f719509e9646722070433e3229`  
		Last Modified: Tue, 05 Dec 2023 18:41:19 GMT  
		Size: 72.1 MB (72096381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e13cf1fcb41e1b6411089aaea97ed187190a87bc9d2066a4e84e466888dc0e`  
		Last Modified: Tue, 05 Dec 2023 18:41:11 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c2da7137b979d67eea939c6e6a5734c89f7758c1a6499a14c449a872524286`  
		Last Modified: Tue, 05 Dec 2023 18:41:11 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
