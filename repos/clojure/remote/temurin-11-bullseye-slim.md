## `clojure:temurin-11-bullseye-slim`

```console
$ docker pull clojure@sha256:198919483984d274c9b2a87caced65fea52e20c35be871f692e1df59cfca1ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:b8872be3af0df31f3e6673315cf195a2d0c8a5bda5bb5811c49247abe32acdcd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (290999618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a858842cd9ad632f4e2c7559459c4c34d2bc80ca78c5f51eb97a70a9c1210c1`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:18:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Sep 2022 06:18:45 GMT
COPY dir:36d56a3b4865ff200a9bbbcc21ae60c89418e4eae9d60cbccb611641838bf98e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:24:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:26:36 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:26:36 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:26:53 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:26:53 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:26:54 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a2774ad4f184f0a10c74dd66c9b4fdf76a60a8dbb311b9499b3173aabfcc61`  
		Last Modified: Tue, 13 Sep 2022 06:24:44 GMT  
		Size: 198.1 MB (198124887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494a5619bec54dea03c4b56276aaaec7182ee35f2e8072919b618569eeb090d2`  
		Last Modified: Fri, 30 Sep 2022 22:38:52 GMT  
		Size: 61.5 MB (61469991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b79f099fc841ea31b914104f5d06808523a4510f65825a703826cc849e1961`  
		Last Modified: Fri, 30 Sep 2022 22:38:44 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:e686cb75d8202048ee9dc3ae6047b09a59ca57da789a71bb39e603365149b5ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.5 MB (286520071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2a04f04bea8e56813696774d452ee644e67a89a1a2b3849650bf906b4c45a`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:58:12 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Sep 2022 06:58:16 GMT
COPY dir:d8305eb424636b15e2ee68b77e921283e709f5d3d0768819ef40e6c325c7578e in /opt/java/openjdk 
# Fri, 30 Sep 2022 22:44:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Sep 2022 22:47:17 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Fri, 30 Sep 2022 22:47:18 GMT
WORKDIR /tmp
# Fri, 30 Sep 2022 22:47:36 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 30 Sep 2022 22:47:37 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 30 Sep 2022 22:47:37 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4184f46e59fa544d67090bc1b94d36f2af8c4757717aecdc90e0819aadac9`  
		Last Modified: Tue, 13 Sep 2022 07:01:59 GMT  
		Size: 194.9 MB (194867856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6cacd17794fb6d1989253f257625a7c6a8023c5a178f167ade47a6dbaad7f9`  
		Last Modified: Fri, 30 Sep 2022 23:04:00 GMT  
		Size: 61.6 MB (61597357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9e86ef09873ed19baa0a68c5ddd82ba04f33e374a4bdb4ada064c66ae761a`  
		Last Modified: Fri, 30 Sep 2022 23:03:51 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
