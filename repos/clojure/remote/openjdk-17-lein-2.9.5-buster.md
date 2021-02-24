## `clojure:openjdk-17-lein-2.9.5-buster`

```console
$ docker pull clojure@sha256:a64478f523aad866c8f20a0553dbd20b537df35b0d737f0a788c146c35b26a9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:openjdk-17-lein-2.9.5-buster` - linux; amd64

```console
$ docker pull clojure@sha256:1a65b2bcd0e1cc40d8b1ad8a61b35cb2ad17d071f0f430ab914a0dde7cfca6af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.9 MB (335855413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486b2ac99880889b2a86aac6af380a2934663fc8e783ed01f409d853816de690`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:35:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:09:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:09:08 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 09 Feb 2021 17:09:08 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 17:09:09 GMT
ENV LANG=C.UTF-8
# Thu, 18 Feb 2021 23:22:21 GMT
ENV JAVA_VERSION=17-ea+10
# Thu, 18 Feb 2021 23:22:35 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/10/GPL/openjdk-17-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='89ed24a42ee151bc720dcc6fd76272404a99b080acf107b8ec42b1270d2f3953'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/10/GPL/openjdk-17-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='f5dd69285e57325b130f80b5dc62beffa9ccdab08f881bbdb68ecbe7e3b249ab'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 18 Feb 2021 23:22:35 GMT
CMD ["jshell"]
# Mon, 22 Feb 2021 22:25:12 GMT
ENV LEIN_VERSION=2.9.5
# Mon, 22 Feb 2021 22:25:12 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Mon, 22 Feb 2021 22:25:12 GMT
WORKDIR /tmp
# Mon, 22 Feb 2021 22:25:18 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Mon, 22 Feb 2021 22:25:18 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 22 Feb 2021 22:25:19 GMT
ENV LEIN_ROOT=1
# Wed, 24 Feb 2021 18:27:26 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.2"]])' > project.clj   && lein deps && rm project.clj
# Wed, 24 Feb 2021 18:27:27 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7467d1831b6947c294d92ee957902c3cd448b17c5ac2103ca5e79d15afb317c3`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 7.8 MB (7830684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feab2c490a3cea21cc051ff29c33cc9857418edfa1be9966124b18abe1d5ae16`  
		Last Modified: Tue, 09 Feb 2021 04:46:00 GMT  
		Size: 10.0 MB (9996459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15a0f46f8c38f4ca7daecf160ba9cdb3ddeafda769e2741e179851cfaa14eec`  
		Last Modified: Tue, 09 Feb 2021 04:46:23 GMT  
		Size: 51.8 MB (51830963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0106ec58b548c1a449201a49526fa42f4b7f6ed71674a7e26d2eef3d3579c4f2`  
		Last Modified: Tue, 09 Feb 2021 17:19:49 GMT  
		Size: 13.9 MB (13920669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e87cd89d3f97623c81d037c7e05e64e9a0f49dcd71db2995b9a50d25018293e`  
		Last Modified: Thu, 18 Feb 2021 23:29:06 GMT  
		Size: 185.8 MB (185796149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8538a5e07e35a795020d26616b17c1f153ac8e297c8782aab8ac4f056ee9172`  
		Last Modified: Mon, 22 Feb 2021 22:31:43 GMT  
		Size: 11.9 MB (11875271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de6b1b90da23d65a8188d0f680c6e7d68e3dae9e208a9e2cd5abd706277d6ab`  
		Last Modified: Wed, 24 Feb 2021 18:34:19 GMT  
		Size: 4.2 MB (4205020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:openjdk-17-lein-2.9.5-buster` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:d5d3905a1ad8bbbbcf85f6557c9b215ca4a748a22a00295be051e0622f0972d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.9 MB (329939554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da1ca2e579622dfc0147995025b96114f8e86c40f0513c009f52bd0017d4dd5f`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:45 GMT
ADD file:78412ee35e3dc6fb5fdfce41eb05dd273ba1d49328ab327465639bfa4821aa51 in / 
# Tue, 09 Feb 2021 02:40:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:43:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:43:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:44:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:10:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:10:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-17
# Tue, 09 Feb 2021 07:10:53 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 07:10:54 GMT
ENV LANG=C.UTF-8
# Thu, 18 Feb 2021 23:43:21 GMT
ENV JAVA_VERSION=17-ea+10
# Thu, 18 Feb 2021 23:43:38 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/10/GPL/openjdk-17-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='89ed24a42ee151bc720dcc6fd76272404a99b080acf107b8ec42b1270d2f3953'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/10/GPL/openjdk-17-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='f5dd69285e57325b130f80b5dc62beffa9ccdab08f881bbdb68ecbe7e3b249ab'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 18 Feb 2021 23:43:39 GMT
CMD ["jshell"]
# Mon, 22 Feb 2021 22:47:07 GMT
ENV LEIN_VERSION=2.9.5
# Mon, 22 Feb 2021 22:47:08 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Mon, 22 Feb 2021 22:47:09 GMT
WORKDIR /tmp
# Mon, 22 Feb 2021 22:47:19 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Mon, 22 Feb 2021 22:47:19 GMT
ENV PATH=/usr/local/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 22 Feb 2021 22:47:20 GMT
ENV LEIN_ROOT=1
# Wed, 24 Feb 2021 18:59:31 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.2"]])' > project.clj   && lein deps && rm project.clj
# Wed, 24 Feb 2021 18:59:32 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:c78c297fb0d010ee085f95ae439636ecb167b050c1acb4273bd576998cf94a83`  
		Last Modified: Tue, 09 Feb 2021 02:47:03 GMT  
		Size: 49.2 MB (49183229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06af62193c25241eb123af8cf115c7a6298e834976fe148ac79ec11a7ca06ee5`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 7.7 MB (7694122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b846e1b73901174c506ae5e6219ac2f356ef71eaa5896dfbc238dc67ca4bf73`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb44d26a138a8d064a4ab8f9b472c64e7136c2482ec5af19bab8811b6d2c15b7`  
		Last Modified: Tue, 09 Feb 2021 04:57:46 GMT  
		Size: 52.2 MB (52165287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e26e0ab11a8be6b1e0ab54b0d53c323acda50b89d3549bd9c10527f3f79e07`  
		Last Modified: Tue, 09 Feb 2021 07:21:52 GMT  
		Size: 14.7 MB (14673596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bd567bd5c6437cccdc680b411006c83e30d08de84404ca32c4eb5acc2d064a`  
		Last Modified: Thu, 18 Feb 2021 23:49:07 GMT  
		Size: 180.2 MB (180158715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898d22a7d34f7ae7057301f49bca3b982c613e33e851427ff350f2763c5257db`  
		Last Modified: Mon, 22 Feb 2021 22:54:31 GMT  
		Size: 11.9 MB (11875160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f143521ad0fb34266c7aaf26b43737ea212e8cf47e96655ed14859cbb8aa0a`  
		Last Modified: Wed, 24 Feb 2021 19:06:51 GMT  
		Size: 4.2 MB (4205164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
