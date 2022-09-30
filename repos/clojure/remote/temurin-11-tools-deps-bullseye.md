## `clojure:temurin-11-tools-deps-bullseye`

```console
$ docker pull clojure@sha256:9e01c5eea354a8836bdd7f8bf747b678e471ecbf7d98f979ec5f75865507309a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-tools-deps-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:639ce2566fcad6b45e761466be02a80f2fa7ba3ae734d5e191562b7dc2193c03
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.5 MB (300451416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bd0a129fc3a54d41b7649c74c075e9ef481c3ebebca8222e0cc698d37d103de`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:18 GMT
ADD file:ff01c6dedb67cf22e9b0735e099b9b6367770c4880941862cc7ec0e979b4118b in / 
# Tue, 13 Sep 2022 00:56:19 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:20:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:23:55 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:23:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:26:16 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:26:16 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:26:31 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:26:32 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:26:32 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:23858da423a6737f0467fab0014e5b53009ea7405d575636af0c3f100bbb2f10`  
		Last Modified: Tue, 13 Sep 2022 01:00:00 GMT  
		Size: 55.0 MB (55029732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9489cf708b9c57f6b8585996c4aef3fd0dffac96db31dce0b646256dfd6607`  
		Last Modified: Fri, 30 Sep 2022 22:37:39 GMT  
		Size: 198.1 MB (198124868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4094d83566801970d801ff51083794d70d3b19e98363ac30c8eece2ed0c4305d`  
		Last Modified: Fri, 30 Sep 2022 22:38:33 GMT  
		Size: 47.3 MB (47296201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdc53340c43e75ac8668f8d77a0a655771ad3bc761ade9354cd0a63045ea031`  
		Last Modified: Fri, 30 Sep 2022 22:38:27 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-tools-deps-bullseye` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ba8100d643fb13d6ea05a8289abcbf848e3fabd85170d266b39b27ea98164e8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295850285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b21429ce8efbba3f3644c7dc1e5ef7e01f8aa6decab5b5bed9843e975143d8e9`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:41 GMT
ADD file:879fb0cd23107ac6f53581456074c7ff13c051aa262de3ca16ffa8475cf04dec in / 
# Tue, 13 Sep 2022 02:10:42 GMT
CMD ["bash"]
# Fri, 30 Sep 2022 22:40:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 30 Sep 2022 22:44:15 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:44:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:46:53 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:46:53 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:47:09 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:47:10 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:47:10 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:10cff8997b4d4f243419e6bede830f1ac33f3d18c5200e5fb80e19333883ec2b`  
		Last Modified: Tue, 13 Sep 2022 02:15:49 GMT  
		Size: 53.7 MB (53691380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496229bd9bf2839e6a37383e68eb8152323866be978a27514af1c0315606d266`  
		Last Modified: Fri, 30 Sep 2022 23:02:36 GMT  
		Size: 194.9 MB (194867813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6690021e3b5251bfe24c8921df43754a1b419abcfa56369a857529d779549e92`  
		Last Modified: Fri, 30 Sep 2022 23:03:38 GMT  
		Size: 47.3 MB (47290475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9087ef1395185f52858e1ec84e2f81caff31ca67d8ca7e0e1572ae0a092d38f0`  
		Last Modified: Fri, 30 Sep 2022 23:03:32 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
