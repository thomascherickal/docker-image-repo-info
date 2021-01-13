## `clojure:openjdk-16-tools-deps-1.10.1.763`

```console
$ docker pull clojure@sha256:23a317f3571b404e47fd47a61ee393e9e855e1eb0b1e3da7cea6a58f56afc216
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-16-tools-deps-1.10.1.763` - linux; amd64

```console
$ docker pull clojure@sha256:e8fd208e2a132485b95ebac7e57b23a7320ae02da4e5baba6b3682f18cfa19ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258112576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a01d2d2bd6d7d88008dc169a7e55cd8d14851a2671830b4db45a0d9a6799ff6e`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 10:53:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 10:53:01 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 10:54:29 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 12 Jan 2021 10:54:29 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 10:54:31 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 12 Jan 2021 10:54:31 GMT
ENV JAVA_VERSION=16-ea+31
# Tue, 12 Jan 2021 10:54:59 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/31/GPL/openjdk-16-ea+31_linux-aarch64_bin.tar.gz; 			downloadSha256=619122347e25dccbc419168329b659cdb1967570431bc09f597a791107484554; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/31/GPL/openjdk-16-ea+31_linux-x64_bin.tar.gz; 			downloadSha256=f43aa41b3c71b9e278a37fd33a94579a8039e07abd21841ad9e1e0a4582abf24; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 12 Jan 2021 10:54:59 GMT
CMD ["jshell"]
# Wed, 13 Jan 2021 07:19:40 GMT
ENV CLOJURE_VERSION=1.10.1.763
# Wed, 13 Jan 2021 07:19:41 GMT
WORKDIR /tmp
# Wed, 13 Jan 2021 07:20:01 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "91421551872d421915c4a598741aefcc6749d3f4aafca9c08f271958e5456e2c *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Wed, 13 Jan 2021 07:20:01 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943d8acaac04a2b66af03bcc85abe1cd3f50e06d7e193634e04d4e55c4fc7cc8`  
		Last Modified: Tue, 12 Jan 2021 11:07:22 GMT  
		Size: 3.2 MB (3248558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceda8782cf4e61566acc646de4afb40c2a1b15bdd608305cdf6aa5937473a433`  
		Last Modified: Tue, 12 Jan 2021 11:08:56 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74bb24e649ac00dc172e70d77d1cd53630cf8e3c35c4a00e6a1f933b0b54668`  
		Last Modified: Tue, 12 Jan 2021 11:09:16 GMT  
		Size: 185.2 MB (185214357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebefe1c0d859ddab8e32ed8c73f463461c8e0c68725e5b9eb68cd134d9c567b`  
		Last Modified: Wed, 13 Jan 2021 07:28:42 GMT  
		Size: 42.5 MB (42541381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-16-tools-deps-1.10.1.763` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:8dc3dac549dc4c3ba12ef2bc382dd285f6b36fb6a3c22fe3813f3a47ba96903b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.6 MB (250575659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82e002b6f7888df2c50652ea9be3214af7da2ba96d45b4e9d83b991b6972b8e1`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:00:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:00:31 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 01:02:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 12 Jan 2021 01:02:13 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 01:02:15 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 12 Jan 2021 01:02:16 GMT
ENV JAVA_VERSION=16-ea+31
# Tue, 12 Jan 2021 01:03:12 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/31/GPL/openjdk-16-ea+31_linux-aarch64_bin.tar.gz; 			downloadSha256=619122347e25dccbc419168329b659cdb1967570431bc09f597a791107484554; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/31/GPL/openjdk-16-ea+31_linux-x64_bin.tar.gz; 			downloadSha256=f43aa41b3c71b9e278a37fd33a94579a8039e07abd21841ad9e1e0a4582abf24; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 12 Jan 2021 01:03:13 GMT
CMD ["jshell"]
# Tue, 12 Jan 2021 19:24:25 GMT
ENV CLOJURE_VERSION=1.10.1.763
# Tue, 12 Jan 2021 19:24:25 GMT
WORKDIR /tmp
# Tue, 12 Jan 2021 19:25:00 GMT
RUN apt-get update && apt-get install -y curl make rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "91421551872d421915c4a598741aefcc6749d3f4aafca9c08f271958e5456e2c *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Tue, 12 Jan 2021 19:25:02 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6132c56bf059fe6b3844038ac4ca6b320af5f511b4c60addc956fb470ebfcb8`  
		Last Modified: Tue, 12 Jan 2021 01:11:08 GMT  
		Size: 3.1 MB (3101516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a74a7e0616e4c6b1416ebb635323d67d5fbc93ea9f39d503031d2e52228e6b`  
		Last Modified: Tue, 12 Jan 2021 01:12:23 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c1ef58bd24c02c6ca91a46be9b616b609b61fc8083bfcf2b7cc1ad5f19d2ca`  
		Last Modified: Tue, 12 Jan 2021 01:12:48 GMT  
		Size: 179.6 MB (179573911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704032b1cf41b1f7a09e6f21f0926438a7c812df964b5c236c2bcf3fda866749`  
		Last Modified: Tue, 12 Jan 2021 19:33:48 GMT  
		Size: 42.0 MB (42035529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
