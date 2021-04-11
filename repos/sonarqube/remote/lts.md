## `sonarqube:lts`

```console
$ docker pull sonarqube@sha256:ad851a8d661b5cfc855d2ab69353faab8623f3f1af4a3102124fff7041f11216
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:lts` - linux; amd64

```console
$ docker pull sonarqube@sha256:dfe97750571a821834b429feef4c27d6444ba67ae700d22c35cdc030dbac68b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.7 MB (290660161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f9672f8b755177eab6f192da28cc47297075095fce55aee27719af6083e762`
-	Entrypoint: `[".\/bin\/run.sh"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 12:44:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:47:32 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sat, 10 Apr 2021 12:47:33 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Sat, 10 Apr 2021 12:47:34 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 12:47:34 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 12:47:34 GMT
ENV JAVA_VERSION=11.0.10
# Sat, 10 Apr 2021 12:48:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jre_x64_linux_11.0.10_9.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jre_aarch64_linux_11.0.10_9.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Sun, 11 Apr 2021 03:20:12 GMT
RUN apt-get update     && apt-get install -y curl gnupg2 unzip     && rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 03:20:12 GMT
ENV SONAR_VERSION=7.9.6 SONARQUBE_HOME=/opt/sonarqube SONARQUBE_JDBC_USERNAME=sonar SONARQUBE_JDBC_PASSWORD=sonar SONARQUBE_JDBC_URL=
# Sun, 11 Apr 2021 03:20:12 GMT
EXPOSE 9000
# Sun, 11 Apr 2021 03:20:13 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Sun, 11 Apr 2021 03:20:14 GMT
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done
# Sun, 11 Apr 2021 03:20:44 GMT
RUN set -x     && cd /opt     && curl -o sonarqube.zip -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip     && curl -o sonarqube.zip.asc -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip.asc     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv sonarqube-$SONAR_VERSION sonarqube     && chown -R sonarqube:sonarqube sonarqube     && rm sonarqube.zip*     && rm -rf $SONARQUBE_HOME/bin/*
# Sun, 11 Apr 2021 03:20:44 GMT
VOLUME [/opt/sonarqube/data]
# Sun, 11 Apr 2021 03:20:45 GMT
WORKDIR /opt/sonarqube
# Sun, 11 Apr 2021 03:20:45 GMT
COPY file:d7c6edf99ad4508dcb273783aad5da8017e549d505d617619117cc576bbc8850 in /opt/sonarqube/bin/ 
# Sun, 11 Apr 2021 03:20:45 GMT
USER sonarqube
# Sun, 11 Apr 2021 03:20:45 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf4c47c8c6124c3089f3ed26410da9870ba18dd4bc68331e2b7e853116a6cad`  
		Last Modified: Sat, 10 Apr 2021 12:54:28 GMT  
		Size: 3.3 MB (3268764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810072571fafc7e3aa679b8d9c55a366c519def4429f84fe76b604d1714bb868`  
		Last Modified: Sat, 10 Apr 2021 12:59:25 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395682a2fa051e6f6d26afc54672593dc8aca2bb30e24d85c81597671c03e7eb`  
		Last Modified: Sat, 10 Apr 2021 13:01:05 GMT  
		Size: 47.0 MB (47045954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d48e13c2db207e80cc0471d5e7b01431a13f249fde5310ea73cc9dad312af3`  
		Last Modified: Sun, 11 Apr 2021 03:21:28 GMT  
		Size: 6.0 MB (5986995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb5390280680d1396fa1729c0651348bd0da3da471cff1c032dec195e2e275`  
		Last Modified: Sun, 11 Apr 2021 03:21:27 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096cf67a0d2fd766bc9be5cb0d253d1dc3ab71b6c97824ec3c1079c6f2534c31`  
		Last Modified: Sun, 11 Apr 2021 03:21:27 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c361605bd9bde830306ee75d3fdd69f951ece7049fd13c3c9c21cd0593341aaa`  
		Last Modified: Sun, 11 Apr 2021 03:21:39 GMT  
		Size: 207.2 MB (207214523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9874e2e5445e4db15944b152e7044aebbab2bd4341cb5d4102d103748101acaa`  
		Last Modified: Sun, 11 Apr 2021 03:21:27 GMT  
		Size: 815.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
