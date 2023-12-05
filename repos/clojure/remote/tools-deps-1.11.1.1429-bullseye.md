## `clojure:tools-deps-1.11.1.1429-bullseye`

```console
$ docker pull clojure@sha256:09a6cd37e6b593ecbd9339ac7a0d43de36170d093d976b111a065f8b2a913484
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:tools-deps-1.11.1.1429-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:8454a0e15aff665313935634419fbf961169535fc4033da6a1462fd6eacd6bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.8 MB (285786027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3500510e56f42f4814193e35effe589f40e2d62facdaeab0d02a09cc3551df8c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 21 Nov 2023 10:24:21 GMT
COPY dir:e6025cb107ac582823e7222bca84438ae7fa7384431777ac5a68b80c2a5b3d9d in /opt/java/openjdk 
# Tue, 21 Nov 2023 10:24:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Dec 2023 18:32:19 GMT
ENV CLOJURE_VERSION=1.11.1.1429
# Tue, 05 Dec 2023 18:32:19 GMT
WORKDIR /tmp
# Tue, 05 Dec 2023 18:32:36 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "bf08cfeb007118b7277aa7423734f5d507604b868f7fc44c0f9929ca9cd94ed4 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 05 Dec 2023 18:32:36 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 05 Dec 2023 18:32:36 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 05 Dec 2023 18:32:37 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 05 Dec 2023 18:32:37 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd0bd145f3c1354fc931bad359bc41ac957c8a5d82aeae2e26bd8d6c004a313`  
		Last Modified: Tue, 21 Nov 2023 10:39:23 GMT  
		Size: 158.6 MB (158630599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0e8c60eaad361f573eb4ac4579249d6a841842e05f68421b9216cbd7c2c1cb`  
		Last Modified: Tue, 05 Dec 2023 18:43:51 GMT  
		Size: 72.1 MB (72096503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bcda2e63997f06df45b9b479db3152da5c5e5e4bba0586a71981c33d6363e2`  
		Last Modified: Tue, 05 Dec 2023 18:43:43 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8274ca443d6ce5be19d1ae8e0b5e267417c1d42200141730b1b5d9b6c6d1c3ea`  
		Last Modified: Tue, 05 Dec 2023 18:43:43 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
