## `clojure:temurin-17-tools-deps-1.11.1.1323-bullseye`

```console
$ docker pull clojure@sha256:87410dd0d564e50554ec5a9b3d1dfef60e22b45a99c01957193847b595011439
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps-1.11.1.1323-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:1296beaf875d0e16c0cf7ecb3c91d0fc2fb3824af2505d0f9fc5b17164cc0da0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.5 MB (319508784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f4781558e0a7d7bfa6fa1fb1ec27e0eb121bb9ba5cbc40a7c6325d34ef5e0f7`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 20:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 14:58:53 GMT
COPY dir:05dd898ce921dff423e175db4bfabc77c7b70b060cfa18a18ee060c7533c567b in /opt/java/openjdk 
# Thu, 04 May 2023 14:58:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 May 2023 20:31:34 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Fri, 19 May 2023 20:31:35 GMT
WORKDIR /tmp
# Fri, 19 May 2023 20:31:50 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 19 May 2023 20:31:51 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 19 May 2023 20:31:51 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 19 May 2023 20:31:51 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 19 May 2023 20:31:51 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbada72a4382332aa6aa78d824d0bdddefea4c233d0617f4e8924c1c87446c9`  
		Last Modified: Thu, 04 May 2023 15:09:12 GMT  
		Size: 192.6 MB (192580390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58efbfc1f9794f45a544fbf9b34d39a41f9f84d4729bf77fc234ff64a197c750`  
		Last Modified: Fri, 19 May 2023 20:42:30 GMT  
		Size: 71.9 MB (71878306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69019f1a5619030aab374b380d980e437cbbb816e8b867c67b8a61e072e97dbd`  
		Last Modified: Fri, 19 May 2023 20:42:22 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f57c9f4bffbcb4ac1521d5495a1618c1b809454b5f1d121ff4c8ea15c75d2a`  
		Last Modified: Fri, 19 May 2023 20:42:22 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps-1.11.1.1323-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8f257c14cb89d4f1884436c8bb608b9b23b0ec32d1ba0dd9699929e5df2397a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.1 MB (317076178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ca296905ec313c4bbaf2509a896cee4410f0765d7b157dcb9cbdd3b756975df`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 23 May 2023 01:29:19 GMT
COPY dir:1b2a87d4690d92c678e5e7380bdebd2fd0670a13533a2a897045c86dc03eb9f6 in /opt/java/openjdk 
# Tue, 23 May 2023 01:29:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 01:31:06 GMT
ENV CLOJURE_VERSION=1.11.1.1323
# Tue, 23 May 2023 01:31:06 GMT
WORKDIR /tmp
# Tue, 23 May 2023 01:31:19 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c4666f0e2c2397b91554befd71ff6149b2e89acbf90400e1dcf557526cfb593d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 23 May 2023 01:31:20 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 23 May 2023 01:31:20 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 23 May 2023 01:31:20 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 23 May 2023 01:31:20 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6f4a297b4e40485159fdaaaca21c302eba0567a5165c796f74cdfaaaeeefed`  
		Last Modified: Tue, 23 May 2023 01:37:02 GMT  
		Size: 191.4 MB (191387676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2554a6db7d9263fb78eec27ac142cb5603d75ef8ab2cb7a01cf8fcc881c57857`  
		Last Modified: Tue, 23 May 2023 01:38:00 GMT  
		Size: 72.0 MB (71994874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f752b58a03cf81ca21125b811888b8cebc87972c7dfcec999710b67e6ef55402`  
		Last Modified: Tue, 23 May 2023 01:37:53 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d28fcb78920667bacdfa9a8f6ebff0c9f72a6fe0555c351580a0d5e996e5c`  
		Last Modified: Tue, 23 May 2023 01:37:53 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
