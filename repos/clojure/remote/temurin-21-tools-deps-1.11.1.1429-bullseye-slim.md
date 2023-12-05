## `clojure:temurin-21-tools-deps-1.11.1.1429-bullseye-slim`

```console
$ docker pull clojure@sha256:ca004f850bb92bd1e215ea2c824a5a393bfd81fc2d9c99c642f8ad5cfd2f4494
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:temurin-21-tools-deps-1.11.1.1429-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:0b97c3617e6ff19168d18167dedef24fda180eaf9c87593bf1e52dcbff28f796
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251755949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:224237ca3a0c7af474e2c7f8f27e4d21e0380709bd1f8042c54afb6ef88f1c83`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:24:45 GMT
COPY dir:e6025cb107ac582823e7222bca84438ae7fa7384431777ac5a68b80c2a5b3d9d in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:24:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:32:43 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:32:43 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:33:00 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:33:00 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:33:00 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 05 Dec 2023 18:33:01 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Dec 2023 18:33:01 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee9fe142867358965136f1cc0a08d653e824e3428b6f7730c4fba26ee8a35ea`  
		Last Modified: Tue, 21 Nov 2023 10:39:48 GMT  
		Size: 158.6 MB (158630588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e78b4abd170896ade1f5156a5631b7f8670dd1774ac1d315dd10d6fe10b553`  
		Last Modified: Tue, 05 Dec 2023 18:44:12 GMT  
		Size: 61.7 MB (61706518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622a4ffbff47249b22d3135a8137111dda7ef57a910a91294d21a9de448bff09`  
		Last Modified: Tue, 05 Dec 2023 18:44:06 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccc34e51aa57df399485a3882fb6fd5b0f3bc4b1756bcd9dc3ff54e0b36a68e`  
		Last Modified: Tue, 05 Dec 2023 18:44:05 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
