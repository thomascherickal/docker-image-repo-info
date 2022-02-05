## `clojure:latest`

```console
$ docker pull clojure@sha256:a52bafe8fbbf006e6dd9d4455a32b3ed75a23fed1e610d412977194163b40fd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:latest` - linux; amd64

```console
$ docker pull clojure@sha256:4946a842194edf97e626632922b734eedadd8bfd314ea3e16af3c5bbfb705302
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.9 MB (351928902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b0072d768187a35141322c7d4331b8b58a257561e7aa860b06f5f12f26f968`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 09:18:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 09:22:30 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 26 Jan 2022 09:22:30 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 09:22:30 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 09:22:31 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 26 Jan 2022 09:22:58 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Jan 2022 09:22:59 GMT
CMD ["jshell"]
# Thu, 27 Jan 2022 16:56:58 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 27 Jan 2022 16:56:58 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 27 Jan 2022 16:56:58 GMT
WORKDIR /tmp
# Thu, 27 Jan 2022 16:57:03 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 27 Jan 2022 16:57:03 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 27 Jan 2022 16:57:04 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 27 Jan 2022 16:57:32 GMT
RUN boot
# Thu, 27 Jan 2022 16:57:32 GMT
ENV LEIN_VERSION=2.9.8
# Thu, 27 Jan 2022 16:57:32 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 27 Jan 2022 16:57:33 GMT
WORKDIR /tmp
# Thu, 27 Jan 2022 16:57:45 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "9952cba539cc6454c3b7385ebce57577087bf2b9001c3ab5c55d668d0aeff6e9 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 27 Jan 2022 16:57:45 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Thu, 27 Jan 2022 16:57:45 GMT
ENV LEIN_ROOT=1
# Thu, 27 Jan 2022 16:57:48 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Fri, 04 Feb 2022 23:44:49 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 23:44:49 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 23:45:08 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 04 Feb 2022 23:45:08 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 23:45:09 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 04 Feb 2022 23:45:09 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 04 Feb 2022 23:45:09 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc79ff7de66b9ef44dc6cd4f500aa92bd1f0b09ccd13eb0ee6441084fbb719cf`  
		Last Modified: Wed, 26 Jan 2022 09:41:32 GMT  
		Size: 1.6 MB (1582049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601a7753163a82e58164b68f17f35605d4e91cb610380e5cdc1e47d045bba5da`  
		Last Modified: Wed, 26 Jan 2022 09:48:21 GMT  
		Size: 187.9 MB (187900233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a6063e2665793109483499c1f3fe562ce1311d61395614336fb342aee43a9f`  
		Last Modified: Thu, 27 Jan 2022 17:21:20 GMT  
		Size: 283.1 KB (283104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e64dec0151106e9e772a41c3be51417c0f5cf31592d394dd55f2e23af3842b1`  
		Last Modified: Thu, 27 Jan 2022 17:21:22 GMT  
		Size: 58.8 MB (58820598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589aa4a2b0a093ec548b086e29e97d31d31067c862ad4cc22b043eddb966cd90`  
		Last Modified: Thu, 27 Jan 2022 17:21:17 GMT  
		Size: 11.9 MB (11861585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3146f7210e9f4b13b7ce2b4732752065afde128941e31656e55c7772c62edcad`  
		Last Modified: Thu, 27 Jan 2022 17:21:16 GMT  
		Size: 4.2 MB (4207373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaaf3d33420a6eb3b5bdb4b6c8736ea6e71bd613a0af312b4671343e54700b0`  
		Last Modified: Fri, 04 Feb 2022 23:56:48 GMT  
		Size: 55.9 MB (55906668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5718157e8a923b8c06dd0843ced9f630ba52616b57ac41f62a6e689cb20016`  
		Last Modified: Fri, 04 Feb 2022 23:56:37 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8588865f497e60b7c8ec05ba39408142aada712c400303dc1ab7b490b5852ef`  
		Last Modified: Fri, 04 Feb 2022 23:56:37 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:latest` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:1146470fa02c2ffd22b44edf929ef39c67af608ab4957379c38245da9e1a0b92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.7 MB (348716411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11c51200448c48b9775061a60d6ffd80dcb0524edcfb6f59b575c50a3ed14f3c`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 05:54:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 26 Jan 2022 05:54:29 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 05:54:30 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 05:54:31 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 26 Jan 2022 05:54:45 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 26 Jan 2022 05:54:45 GMT
CMD ["jshell"]
# Wed, 26 Jan 2022 21:14:35 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Jan 2022 21:14:35 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Jan 2022 21:14:36 GMT
WORKDIR /tmp
# Wed, 26 Jan 2022 21:14:41 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Jan 2022 21:14:42 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Jan 2022 21:14:43 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Jan 2022 21:15:01 GMT
RUN boot
# Wed, 26 Jan 2022 21:15:01 GMT
ENV LEIN_VERSION=2.9.8
# Wed, 26 Jan 2022 21:15:02 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 26 Jan 2022 21:15:03 GMT
WORKDIR /tmp
# Wed, 26 Jan 2022 21:15:13 GMT
RUN set -eux; apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "9952cba539cc6454c3b7385ebce57577087bf2b9001c3ab5c55d668d0aeff6e9 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 26 Jan 2022 21:15:14 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Wed, 26 Jan 2022 21:15:15 GMT
ENV LEIN_ROOT=1
# Wed, 26 Jan 2022 21:15:18 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Fri, 04 Feb 2022 21:40:31 GMT
ENV CLOJURE_VERSION=1.10.3.1075
# Fri, 04 Feb 2022 21:40:32 GMT
WORKDIR /tmp
# Fri, 04 Feb 2022 21:40:49 GMT
RUN apt-get update && apt-get install -y curl make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a6b72c9b23d348a0636813c5f59db5dda622e3b8dbb86124cbb51e3aced714d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove curl wget
# Fri, 04 Feb 2022 21:40:50 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 04 Feb 2022 21:40:51 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 04 Feb 2022 21:40:51 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 04 Feb 2022 21:40:52 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abf67e3e34eccefabf68f15c7d753f1a4c8e241beb1818f97e276186d54124e`  
		Last Modified: Wed, 26 Jan 2022 06:13:02 GMT  
		Size: 1.6 MB (1565889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf423efb00f6c398e72a29f80e84cf999f7b9a81877dedb0e179db07c4daaa2`  
		Last Modified: Wed, 26 Jan 2022 06:20:25 GMT  
		Size: 186.5 MB (186527434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ec1fe9a5adf38c7107d372dfff182d90b1983ce2dc3045097612b7071a1791`  
		Last Modified: Wed, 26 Jan 2022 21:41:14 GMT  
		Size: 67.2 KB (67218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ee2eec4fd174648f119e8be09742139e3de31b5356919f065853e33083a9d1`  
		Last Modified: Wed, 26 Jan 2022 21:41:21 GMT  
		Size: 58.8 MB (58816250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc1f7aaae0c4992bdffc34dbabd9c6fb6803d8b27b352fb8bd4e11d7c6db9c2`  
		Last Modified: Wed, 26 Jan 2022 21:41:14 GMT  
		Size: 11.6 MB (11645523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d7ce92c186c8454780ecb93edb1133626231c4dfc918396fa46f88c2f1677b`  
		Last Modified: Wed, 26 Jan 2022 21:41:13 GMT  
		Size: 4.2 MB (4207135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab4e5a6dec990d7f3fb7f455cbb167ff2272aa1761e49afe97ab99bdce86fce`  
		Last Modified: Fri, 04 Feb 2022 21:55:05 GMT  
		Size: 55.8 MB (55829156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac47432fd0ff01173bff3fd94298fb4d9241c5e6b28d238486d38ac18a87203`  
		Last Modified: Fri, 04 Feb 2022 21:54:57 GMT  
		Size: 626.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d86676301c1d7e42f0174ed8dcccd39111ce4e7234e3e43bb9ae4196f4672`  
		Last Modified: Fri, 04 Feb 2022 21:54:57 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
