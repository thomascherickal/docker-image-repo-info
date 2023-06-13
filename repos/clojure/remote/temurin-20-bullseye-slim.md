## `clojure:temurin-20-bullseye-slim`

```console
$ docker pull clojure@sha256:24e2d5a183480e364b588c4b9b96eff126cf5abdf1d192be5170befad533559a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:398db2d5a3ce87f6c0f7615afc43e831dc7bd65a72f05380c0f29648328a228c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.7 MB (295728627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e52b62c0113fc9d33422c0c759a45cbb76e96eeda9d60128d59159eff02754a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:53:06 GMT
COPY dir:02736280d197ac4d1b6ebf68d948efb46e7eeffd579505356f8c94946dbcce6f in /opt/java/openjdk 
# Tue, 13 Jun 2023 03:53:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 03:53:52 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 03:53:52 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 03:54:08 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 03:54:09 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 03:54:09 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 03:54:09 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 03:54:09 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d098ed12ffb6e1c454a1384074f474bd403cef6b65d6e8b73d5640a4874312de`  
		Last Modified: Tue, 13 Jun 2023 04:01:02 GMT  
		Size: 202.8 MB (202813962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d197fed8cf16e5cbc2bb1c60018cc7ff2e0ccca93bbb2bb32f0cc2e6917920`  
		Last Modified: Tue, 13 Jun 2023 04:01:38 GMT  
		Size: 61.5 MB (61496245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e48e26f96512a3cc6e69231a45292111872a0ebfa2eb75545f59e742434cecc`  
		Last Modified: Tue, 13 Jun 2023 04:01:31 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ac610165703f96994addd05c865b0175980fbc450a88c43bb91a3bb0106947`  
		Last Modified: Tue, 13 Jun 2023 04:01:31 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:7f6d915894eb6bda1a1291c7c39b5ff2310464c1b2f0671c87efe8d89faecbd8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.8 MB (292833233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647d1238bc9656f784e37f550b1f66a1c9b42396ab3757d69a4730d110e5d94f`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:58:18 GMT
COPY dir:f555428af67a610819205eec573e23f479077e0999818ee9dc0f3375599d21db in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:58:23 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:59:01 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Tue, 13 Jun 2023 04:59:02 GMT
WORKDIR /tmp
# Tue, 13 Jun 2023 04:59:15 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 13 Jun 2023 04:59:16 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 13 Jun 2023 04:59:16 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 13 Jun 2023 04:59:16 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 13 Jun 2023 04:59:16 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec330e2c6a276c3efe415a805c40d111b657a3b03708c5cd4d818fdca4560f53`  
		Last Modified: Tue, 13 Jun 2023 05:05:04 GMT  
		Size: 201.2 MB (201157962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476d1a6c94cdb7c7e167d3f69921c9c6b408bb865ee4206f839fe632f63d020d`  
		Last Modified: Tue, 13 Jun 2023 05:05:36 GMT  
		Size: 61.6 MB (61611425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34fca1ee9ce823716befcbabfd8b28cd513bd19170dc841cbebd69ce5da6b57`  
		Last Modified: Tue, 13 Jun 2023 05:05:30 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd3dc14e0eeaf801822401c05ad5a17deaa71d081b7f78043e73b4f4518ff70`  
		Last Modified: Tue, 13 Jun 2023 05:05:30 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
