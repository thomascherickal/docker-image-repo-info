## `clojure:openjdk-17-lein`

```console
$ docker pull clojure@sha256:17080d1b1aa9b0f9eb8a39dfdc1805cd7685634d9744ae813aea31f6221063c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-lein` - linux; amd64

```console
$ docker pull clojure@sha256:16808a8ecc7ec459f36c7ca66177754e075af402b99071bb932c28b1d506f6de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233034111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687e4853f69e438d749f9661145a0ff2dee54620aceeed631e233d03eee8a0f`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:48:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:48:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Wed, 12 May 2021 06:48:04 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:48:04 GMT
ENV LANG=C.UTF-8
# Thu, 27 May 2021 23:30:48 GMT
ENV JAVA_VERSION=17-ea+24
# Thu, 27 May 2021 23:31:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='30b8cc8945c42ab310bca47ecfe2acdf2a0285d26dfeb6bfba46ebc5947aef6e'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='61d192356099180ee3beec3a22cb9e97cb810c7f55f2c870a73841c3ac61abcb'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 27 May 2021 23:31:02 GMT
CMD ["jshell"]
# Thu, 27 May 2021 23:55:28 GMT
ENV LEIN_VERSION=2.9.6
# Thu, 27 May 2021 23:55:28 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 27 May 2021 23:55:29 GMT
WORKDIR /tmp
# Thu, 27 May 2021 23:55:40 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 27 May 2021 23:55:40 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 27 May 2021 23:55:40 GMT
ENV LEIN_ROOT=1
# Thu, 27 May 2021 23:55:44 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Thu, 27 May 2021 23:55:44 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2b89b6081832b112f9483322d4710c661f12135e79279dc3fb1672883ada8d`  
		Last Modified: Wed, 12 May 2021 06:58:18 GMT  
		Size: 3.3 MB (3268772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a2652fa53fe093e3b2e02b7f2d9a2837ea0791b549d005381635049293586a`  
		Last Modified: Thu, 27 May 2021 23:37:22 GMT  
		Size: 186.6 MB (186612738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b9db3701f07391f00731ab78614ccb0e898b412f47419b2cdcc94b043ce5a4`  
		Last Modified: Fri, 28 May 2021 00:00:13 GMT  
		Size: 11.8 MB (11802961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8456fbbd958e31c03d958922053fca1576539d0c3e53bb5f5bf2b9345749cf5`  
		Last Modified: Fri, 28 May 2021 00:00:12 GMT  
		Size: 4.2 MB (4203725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-lein` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:dc95ac8e289339ec7236c550b6ed7307847da243e3927c59ba9dd5965ba5f92d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.6 MB (227632374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74b38aa0ffef772f087e0603a3eff06c3c09e83712cf859278250066173b137`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Thu, 27 May 2021 08:38:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 08:38:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Thu, 27 May 2021 08:38:57 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 May 2021 08:38:57 GMT
ENV LANG=C.UTF-8
# Thu, 27 May 2021 08:38:57 GMT
ENV JAVA_VERSION=17-ea+23
# Thu, 27 May 2021 08:39:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/23/GPL/openjdk-17-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='b43ffb86cad128acb9955d2dec2b254ffd0e0c7b7d2a15d8b7ad93772e8f722b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/23/GPL/openjdk-17-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='b5979d864a5c527c98adc81b5430d669672a609a4c19cd8c8b03edb84de74949'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 27 May 2021 08:39:09 GMT
CMD ["jshell"]
# Thu, 27 May 2021 14:09:06 GMT
ENV LEIN_VERSION=2.9.6
# Thu, 27 May 2021 14:09:07 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 27 May 2021 14:09:07 GMT
WORKDIR /tmp
# Thu, 27 May 2021 14:09:22 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "094b58e2b13b42156aaf7d443ed5f6665aee27529d9512f8d7282baa3cc01429 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 27 May 2021 14:09:22 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 27 May 2021 14:09:22 GMT
ENV LEIN_ROOT=1
# Thu, 27 May 2021 14:09:26 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Thu, 27 May 2021 14:09:26 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb067f13654098b66e57229fcd818a7d0f0c73bd34d158e3bedc28ee2a7b821`  
		Last Modified: Thu, 27 May 2021 08:54:42 GMT  
		Size: 3.1 MB (3118848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257d9d3e721d479d92ee9a91355ffcf19f7e099bbec28bbf4e48117341a6869f`  
		Last Modified: Thu, 27 May 2021 08:54:58 GMT  
		Size: 182.6 MB (182595734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb234de673eecc763d286b2afd453e73dfe23f85e9929af510ef9526fbee3874`  
		Last Modified: Thu, 27 May 2021 14:19:36 GMT  
		Size: 11.8 MB (11802827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0637f0f4988eaf409d022d79af6238b3ccfd2996e022e4257e446d66409d204c`  
		Last Modified: Thu, 27 May 2021 14:19:35 GMT  
		Size: 4.2 MB (4203715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
