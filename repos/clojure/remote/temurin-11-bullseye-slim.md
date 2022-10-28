## `clojure:temurin-11-bullseye-slim`

```console
$ docker pull clojure@sha256:91504f0b1c86960ff94ce5d085c7fae682b80724be149445d29f7ccd30f3316c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-11-bullseye-slim` - linux; amd64

```console
$ docker pull clojure@sha256:3268486aa75b29bf6ce81594cf9e649170a9a675fb12da291f6a378248f2df14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291018369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538007bc3a91a7075819396a8741d84d1725db6e3b6aeedd0dcd84c1137ea222`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 21:50:03 GMT
COPY dir:80db6f3290e8de5c875b6f069ca1d81f6b5c9f4e34668a64373c380a024a607d in /opt/java/openjdk 
# Wed, 26 Oct 2022 21:50:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:36:32 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:36:32 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:36:51 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:36:52 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:36:52 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c841fe95a1d54b7ca4c2b99fafd39b67e5751811eec91ebb5a03381e515360e`  
		Last Modified: Wed, 26 Oct 2022 22:07:24 GMT  
		Size: 198.1 MB (198124716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4790735c0abbbb68654085dfcfdf8d8123225d9bb5dea3606b5543fc199a9f3a`  
		Last Modified: Fri, 28 Oct 2022 20:47:29 GMT  
		Size: 61.5 MB (61472999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2790e0d974323bff0ca74e14c2a78c1361f849e69227e4df61d9286b53de2b`  
		Last Modified: Fri, 28 Oct 2022 20:47:20 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-11-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:bbe6d95c1e1393ff71a9296f6d7ff98e499671f71eef298fe56a1e0b4233e3ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.5 MB (286524030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba0ca46f97883540241231705224866bd8a113ebf0526c3b34079fddde5ea92`
-	Default Command: `["clj"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 15:38:30 GMT
COPY dir:0c9c8c2b9cd43799d246d5824c591352650ad79f5d15544287f00c2deb1e4608 in /opt/java/openjdk 
# Wed, 26 Oct 2022 15:38:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Oct 2022 20:28:28 GMT
ENV CLOJURE_VERSION=1.11.1.1182
# Fri, 28 Oct 2022 20:28:28 GMT
WORKDIR /tmp
# Fri, 28 Oct 2022 20:28:42 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0e80041419bb91e142e2e8683e4dad6faf79958b603bb63b2a93bdd62c2a4f14 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 28 Oct 2022 20:28:43 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 28 Oct 2022 20:28:43 GMT
CMD ["clj"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a3d7b35da3e357173d5404cc59df1a4394d6031ee4598b02de7918d2110bae`  
		Last Modified: Wed, 26 Oct 2022 15:58:03 GMT  
		Size: 194.9 MB (194866982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e508601b07019c800087567952a52c5e277db586bb08cd3defbf4b6191654e8f`  
		Last Modified: Fri, 28 Oct 2022 20:36:38 GMT  
		Size: 61.6 MB (61592520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7070fa7bddb7c920533c8cea5b8a65ea4eec23105cac34aa1c06a522a672338e`  
		Last Modified: Fri, 28 Oct 2022 20:36:31 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
