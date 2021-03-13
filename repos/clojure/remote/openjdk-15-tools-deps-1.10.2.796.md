## `clojure:openjdk-15-tools-deps-1.10.2.796`

```console
$ docker pull clojure@sha256:974e2e4cc3ccc60e7cb4a553386f50f8bd4df043df27c5e82566dfc69b702856
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-15-tools-deps-1.10.2.796` - linux; amd64

```console
$ docker pull clojure@sha256:226caeb6087bb805e8172487b5565eb8dc3d9482363c5556db750c4ecd90ecab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269130160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8cdc82fb8db03d87bc67a7d534f9877c261017274567b5d9bcd0fb2f7639484`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Mar 2021 20:57:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Mar 2021 21:01:35 GMT
ENV JAVA_HOME=/usr/local/openjdk-15
# Tue, 09 Mar 2021 21:01:36 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 09 Mar 2021 21:01:36 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 21:01:37 GMT
ENV LANG=C.UTF-8
# Tue, 09 Mar 2021 21:01:37 GMT
ENV JAVA_VERSION=15.0.2
# Tue, 09 Mar 2021 21:01:50 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='91ac6fc353b6bf39d995572b700e37a20e119a87034eeb939a6f24356fbcd207'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='3958f01858f9290c48c23e7804a0af3624e8eca6749b085c425df4c4f2f7dcbc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 21:01:51 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:50:01 GMT
ENV CLOJURE_VERSION=1.10.2.796
# Tue, 09 Mar 2021 21:50:01 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:50:18 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0ea8633c7f53eb76098132d4a4536169395be24bbdc253cff4d10251e2ea6e45 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 09 Mar 2021 21:50:18 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f1fbf102b7eaa0998133d35bbcc37641d4d23626a4a2673cb9a2393cb7c34c`  
		Last Modified: Tue, 09 Mar 2021 21:10:48 GMT  
		Size: 3.3 MB (3268548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd8a9c0aa2d3c2824cda489386aab6f22b531483077bfc2eb5b3a9f496b518b`  
		Last Modified: Tue, 09 Mar 2021 21:17:53 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5ad54c94206a793de773d834eabbb929cc23a20345c9e79637969b39fc1ee5`  
		Last Modified: Tue, 09 Mar 2021 21:18:09 GMT  
		Size: 196.2 MB (196173943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6a62062390b2ea697299be58ab3144f766692af98b7c659c40f654743a208b`  
		Last Modified: Tue, 09 Mar 2021 22:04:25 GMT  
		Size: 42.6 MB (42592315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-15-tools-deps-1.10.2.796` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b7a997148bee08b9db53d49706190232db59a281f5a4393b1a259526641d1bb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.3 MB (246339166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91546c1752906ee0998f031dd59bead1545d7b947fdd32b4ea4fb39a513a24fd`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:34:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:38:43 GMT
ENV JAVA_HOME=/usr/local/openjdk-15
# Fri, 12 Mar 2021 06:38:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 12 Mar 2021 06:38:46 GMT
ENV PATH=/usr/local/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 Mar 2021 06:38:46 GMT
ENV LANG=C.UTF-8
# Fri, 12 Mar 2021 06:38:47 GMT
ENV JAVA_VERSION=15.0.2
# Fri, 12 Mar 2021 06:39:10 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='91ac6fc353b6bf39d995572b700e37a20e119a87034eeb939a6f24356fbcd207'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk15.0.2/0d1cfde4252546c6931946de8db48ee2/7/GPL/openjdk-15.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='3958f01858f9290c48c23e7804a0af3624e8eca6749b085c425df4c4f2f7dcbc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 12 Mar 2021 06:39:12 GMT
CMD ["jshell"]
# Sat, 13 Mar 2021 01:01:48 GMT
ENV CLOJURE_VERSION=1.10.2.796
# Sat, 13 Mar 2021 01:01:49 GMT
WORKDIR /tmp
# Sat, 13 Mar 2021 01:02:37 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0ea8633c7f53eb76098132d4a4536169395be24bbdc253cff4d10251e2ea6e45 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Sat, 13 Mar 2021 01:02:40 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303a8d33f3a602102b6a15a1f7974fc79449cdcff2c2fa6709b56cd1ac792384`  
		Last Modified: Fri, 12 Mar 2021 06:45:08 GMT  
		Size: 3.1 MB (3118728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5713e17d4b97378d2eb98468427a9d36966d2bd612e5545b9ec3d4d656f36abc`  
		Last Modified: Fri, 12 Mar 2021 06:48:07 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d792d8f51ba63ce2be1ad8310f70ad7363dc633983072d4ad4dfd89a5006d45`  
		Last Modified: Fri, 12 Mar 2021 06:48:36 GMT  
		Size: 175.3 MB (175267057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92af116913235a02da16076c6afed0bdd33102f8be762ed087a27ff92a28b6b`  
		Last Modified: Sat, 13 Mar 2021 01:18:34 GMT  
		Size: 42.1 MB (42096658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
