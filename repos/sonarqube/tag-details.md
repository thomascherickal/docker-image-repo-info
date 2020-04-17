<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sonarqube`

-	[`sonarqube:7.9.3-community`](#sonarqube793-community)
-	[`sonarqube:7.9-community`](#sonarqube79-community)
-	[`sonarqube:8.2-community`](#sonarqube82-community)
-	[`sonarqube:8.2-developer`](#sonarqube82-developer)
-	[`sonarqube:8.2-enterprise`](#sonarqube82-enterprise)
-	[`sonarqube:8-community`](#sonarqube8-community)
-	[`sonarqube:8-developer`](#sonarqube8-developer)
-	[`sonarqube:8-enterprise`](#sonarqube8-enterprise)
-	[`sonarqube:community`](#sonarqubecommunity)
-	[`sonarqube:developer`](#sonarqubedeveloper)
-	[`sonarqube:enterprise`](#sonarqubeenterprise)
-	[`sonarqube:latest`](#sonarqubelatest)
-	[`sonarqube:lts`](#sonarqubelts)

## `sonarqube:7.9.3-community`

```console
$ docker pull sonarqube@sha256:daf51eb642f84c9e280dcb0cb5dfc9a7853beb8e2796cbad0db0d18f80393f45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:7.9.3-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:cb045a7b46f913fb07e0c7c46ab62879fb78eb252200008428d5667f3c396c59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.7 MB (286696139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c26581d4b9b54446d7b09d59808bdaa05da41df4a6a0bf2aeafba6066600794`
-	Entrypoint: `[".\/bin\/run.sh"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:05:50 GMT
RUN apt-get update     && apt-get install -y curl gnupg2 unzip     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:05:51 GMT
ENV SONAR_VERSION=7.9.3 SONARQUBE_HOME=/opt/sonarqube SONARQUBE_JDBC_USERNAME=sonar SONARQUBE_JDBC_PASSWORD=sonar SONARQUBE_JDBC_URL=
# Fri, 17 Apr 2020 10:05:51 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:05:52 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:05:54 GMT
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done
# Fri, 17 Apr 2020 10:06:13 GMT
RUN set -x     && cd /opt     && curl -o sonarqube.zip -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip     && curl -o sonarqube.zip.asc -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip.asc     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv sonarqube-$SONAR_VERSION sonarqube     && chown -R sonarqube:sonarqube sonarqube     && rm sonarqube.zip*     && rm -rf $SONARQUBE_HOME/bin/*
# Fri, 17 Apr 2020 10:06:14 GMT
VOLUME [/opt/sonarqube/data]
# Fri, 17 Apr 2020 10:06:14 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:06:14 GMT
COPY file:aa007fcc6be4125cbbb27fe345978294add03a4f05e942a5208a37be832addca in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:06:15 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:06:15 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583424677bf8a2a7d1ebe176293a64c39bbb8d6ba8d12048f013af4e941a3861`  
		Last Modified: Fri, 17 Apr 2020 10:08:41 GMT  
		Size: 6.0 MB (5984876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560b7570bd8332051d2fb4092d83568328013ac71dd9eeedab37a70b56c14e74`  
		Last Modified: Fri, 17 Apr 2020 10:08:39 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96baee3083f83f3f3289a64c8e9e7aa820e138048f6f888a65158dbf1133ca2`  
		Last Modified: Fri, 17 Apr 2020 10:08:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aebcb2200f2e6423966a59142d662a1dd140537df2a20099db1d7cabb8c6e9`  
		Last Modified: Fri, 17 Apr 2020 10:09:29 GMT  
		Size: 208.1 MB (208144762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abadafa5ab9541945485f7a713fd09f2c3319ed68335c8419416d9e2c060c10`  
		Last Modified: Fri, 17 Apr 2020 10:08:40 GMT  
		Size: 789.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:7.9-community`

```console
$ docker pull sonarqube@sha256:daf51eb642f84c9e280dcb0cb5dfc9a7853beb8e2796cbad0db0d18f80393f45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:7.9-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:cb045a7b46f913fb07e0c7c46ab62879fb78eb252200008428d5667f3c396c59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.7 MB (286696139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c26581d4b9b54446d7b09d59808bdaa05da41df4a6a0bf2aeafba6066600794`
-	Entrypoint: `[".\/bin\/run.sh"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:05:50 GMT
RUN apt-get update     && apt-get install -y curl gnupg2 unzip     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:05:51 GMT
ENV SONAR_VERSION=7.9.3 SONARQUBE_HOME=/opt/sonarqube SONARQUBE_JDBC_USERNAME=sonar SONARQUBE_JDBC_PASSWORD=sonar SONARQUBE_JDBC_URL=
# Fri, 17 Apr 2020 10:05:51 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:05:52 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:05:54 GMT
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done
# Fri, 17 Apr 2020 10:06:13 GMT
RUN set -x     && cd /opt     && curl -o sonarqube.zip -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip     && curl -o sonarqube.zip.asc -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip.asc     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv sonarqube-$SONAR_VERSION sonarqube     && chown -R sonarqube:sonarqube sonarqube     && rm sonarqube.zip*     && rm -rf $SONARQUBE_HOME/bin/*
# Fri, 17 Apr 2020 10:06:14 GMT
VOLUME [/opt/sonarqube/data]
# Fri, 17 Apr 2020 10:06:14 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:06:14 GMT
COPY file:aa007fcc6be4125cbbb27fe345978294add03a4f05e942a5208a37be832addca in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:06:15 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:06:15 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583424677bf8a2a7d1ebe176293a64c39bbb8d6ba8d12048f013af4e941a3861`  
		Last Modified: Fri, 17 Apr 2020 10:08:41 GMT  
		Size: 6.0 MB (5984876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560b7570bd8332051d2fb4092d83568328013ac71dd9eeedab37a70b56c14e74`  
		Last Modified: Fri, 17 Apr 2020 10:08:39 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96baee3083f83f3f3289a64c8e9e7aa820e138048f6f888a65158dbf1133ca2`  
		Last Modified: Fri, 17 Apr 2020 10:08:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aebcb2200f2e6423966a59142d662a1dd140537df2a20099db1d7cabb8c6e9`  
		Last Modified: Fri, 17 Apr 2020 10:09:29 GMT  
		Size: 208.1 MB (208144762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abadafa5ab9541945485f7a713fd09f2c3319ed68335c8419416d9e2c060c10`  
		Last Modified: Fri, 17 Apr 2020 10:08:40 GMT  
		Size: 789.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8.2-community`

```console
$ docker pull sonarqube@sha256:ee95412e0b61d5127b377c0b6d141d814e1d7cbcffff64933194da48634fb95d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8.2-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:52e1a3fcae6fb805cecb2894aee6b09ab0dd5d5b84fd0ba25269e2911bc95314
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302191326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5203e55f281cc9a6ee9ce53848b238890667b9f7ddd56cbf7246ab12cc682eb`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:06:43 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:06:43 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:06:43 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:06:45 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:07:04 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "$SONARQUBE_ZIP_URL"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:07:05 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:07:05 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:07:05 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:07:05 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea3e87bd78a1afaab4f8e797b652c72104c27067895218b886412693f4e4f26`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 15.0 KB (14984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3695f3dc51df741c3dc99b525335973a82f2001dd8e215b19df752b98e94608c`  
		Last Modified: Fri, 17 Apr 2020 10:10:02 GMT  
		Size: 220.9 MB (220902607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d71901465c1fed918cf4c3d0a39722014f700ca3b8d6c2af21aad0828374c9`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8.2-developer`

```console
$ docker pull sonarqube@sha256:93b01ed06a127053226699c16f1e3d8ea4cb6aecb8b679441f58ce044d267267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8.2-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:596df5438f1ceb7adf5a81ee2564410840879bc0a4ace9731c857901211a4836
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.9 MB (363901398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfe92ff462faf7543d91bafa56d9e705dd3e47656cec6eed960caee4e911063`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:07:13 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:07:13 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:07:13 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:07:15 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:07:39 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "$SONARQUBE_ZIP_URL"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:07:39 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:07:40 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:07:40 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:07:40 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1dbf1b27574ac1a1544a294210a80f0d970e27ebe6bdb8d1cff9b16963288c`  
		Last Modified: Fri, 17 Apr 2020 10:10:10 GMT  
		Size: 15.0 KB (14985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53862f08bedebd5850edaaad4593475c92f663901f96ff9242bfc0732c4648`  
		Last Modified: Fri, 17 Apr 2020 10:10:53 GMT  
		Size: 282.6 MB (282612678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675085a12b56f4404a8c8419d863f3366b889adcd4f0e0037c0fb057b3610a9e`  
		Last Modified: Fri, 17 Apr 2020 10:10:09 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8.2-enterprise`

```console
$ docker pull sonarqube@sha256:ae7a23c9e0e264f6c33f1ffd1c8a5d9a6828356fec1e7d999cf06eb7be837d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8.2-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:c9a0ea9f2babd56c02d3e12d4544d7bc5c1d2022c3e220a0be424b892496826e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.7 MB (385723404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc0cef885e631e0e2b70f1ec40ae58940f574c7d0ad9b363c0388bb489926cc`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:07:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:07:48 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:07:48 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:07:50 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:08:15 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "${SONARQUBE_ZIP_URL}"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:08:15 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:08:16 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:08:16 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:08:17 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be03a705f7c2a3c69e5e5c9a1b0b7990352c89836a97f77118a30d45d5ac538c`  
		Last Modified: Fri, 17 Apr 2020 10:11:10 GMT  
		Size: 15.0 KB (14984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1e7c2c39f6ea061e18396433a787caa1ccb95f0bec10e025869f9be490f10e`  
		Last Modified: Fri, 17 Apr 2020 10:11:55 GMT  
		Size: 304.4 MB (304434679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f854954293c64504fa762935fc02e69af241505c2970106bf576d70f72e23a`  
		Last Modified: Fri, 17 Apr 2020 10:11:10 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8-community`

```console
$ docker pull sonarqube@sha256:ee95412e0b61d5127b377c0b6d141d814e1d7cbcffff64933194da48634fb95d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:52e1a3fcae6fb805cecb2894aee6b09ab0dd5d5b84fd0ba25269e2911bc95314
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302191326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5203e55f281cc9a6ee9ce53848b238890667b9f7ddd56cbf7246ab12cc682eb`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:06:43 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:06:43 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:06:43 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:06:45 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:07:04 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "$SONARQUBE_ZIP_URL"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:07:05 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:07:05 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:07:05 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:07:05 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea3e87bd78a1afaab4f8e797b652c72104c27067895218b886412693f4e4f26`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 15.0 KB (14984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3695f3dc51df741c3dc99b525335973a82f2001dd8e215b19df752b98e94608c`  
		Last Modified: Fri, 17 Apr 2020 10:10:02 GMT  
		Size: 220.9 MB (220902607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d71901465c1fed918cf4c3d0a39722014f700ca3b8d6c2af21aad0828374c9`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8-developer`

```console
$ docker pull sonarqube@sha256:93b01ed06a127053226699c16f1e3d8ea4cb6aecb8b679441f58ce044d267267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:596df5438f1ceb7adf5a81ee2564410840879bc0a4ace9731c857901211a4836
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.9 MB (363901398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfe92ff462faf7543d91bafa56d9e705dd3e47656cec6eed960caee4e911063`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:07:13 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:07:13 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:07:13 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:07:15 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:07:39 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "$SONARQUBE_ZIP_URL"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:07:39 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:07:40 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:07:40 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:07:40 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1dbf1b27574ac1a1544a294210a80f0d970e27ebe6bdb8d1cff9b16963288c`  
		Last Modified: Fri, 17 Apr 2020 10:10:10 GMT  
		Size: 15.0 KB (14985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53862f08bedebd5850edaaad4593475c92f663901f96ff9242bfc0732c4648`  
		Last Modified: Fri, 17 Apr 2020 10:10:53 GMT  
		Size: 282.6 MB (282612678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675085a12b56f4404a8c8419d863f3366b889adcd4f0e0037c0fb057b3610a9e`  
		Last Modified: Fri, 17 Apr 2020 10:10:09 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8-enterprise`

```console
$ docker pull sonarqube@sha256:ae7a23c9e0e264f6c33f1ffd1c8a5d9a6828356fec1e7d999cf06eb7be837d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:c9a0ea9f2babd56c02d3e12d4544d7bc5c1d2022c3e220a0be424b892496826e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.7 MB (385723404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc0cef885e631e0e2b70f1ec40ae58940f574c7d0ad9b363c0388bb489926cc`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:07:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:07:48 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:07:48 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:07:50 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:08:15 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "${SONARQUBE_ZIP_URL}"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:08:15 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:08:16 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:08:16 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:08:17 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be03a705f7c2a3c69e5e5c9a1b0b7990352c89836a97f77118a30d45d5ac538c`  
		Last Modified: Fri, 17 Apr 2020 10:11:10 GMT  
		Size: 15.0 KB (14984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1e7c2c39f6ea061e18396433a787caa1ccb95f0bec10e025869f9be490f10e`  
		Last Modified: Fri, 17 Apr 2020 10:11:55 GMT  
		Size: 304.4 MB (304434679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f854954293c64504fa762935fc02e69af241505c2970106bf576d70f72e23a`  
		Last Modified: Fri, 17 Apr 2020 10:11:10 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:community`

```console
$ docker pull sonarqube@sha256:ee95412e0b61d5127b377c0b6d141d814e1d7cbcffff64933194da48634fb95d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:community` - linux; amd64

```console
$ docker pull sonarqube@sha256:52e1a3fcae6fb805cecb2894aee6b09ab0dd5d5b84fd0ba25269e2911bc95314
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302191326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5203e55f281cc9a6ee9ce53848b238890667b9f7ddd56cbf7246ab12cc682eb`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:06:43 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:06:43 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:06:43 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:06:45 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:07:04 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "$SONARQUBE_ZIP_URL"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:07:05 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:07:05 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:07:05 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:07:05 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea3e87bd78a1afaab4f8e797b652c72104c27067895218b886412693f4e4f26`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 15.0 KB (14984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3695f3dc51df741c3dc99b525335973a82f2001dd8e215b19df752b98e94608c`  
		Last Modified: Fri, 17 Apr 2020 10:10:02 GMT  
		Size: 220.9 MB (220902607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d71901465c1fed918cf4c3d0a39722014f700ca3b8d6c2af21aad0828374c9`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:developer`

```console
$ docker pull sonarqube@sha256:93b01ed06a127053226699c16f1e3d8ea4cb6aecb8b679441f58ce044d267267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:596df5438f1ceb7adf5a81ee2564410840879bc0a4ace9731c857901211a4836
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.9 MB (363901398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfe92ff462faf7543d91bafa56d9e705dd3e47656cec6eed960caee4e911063`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:07:13 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:07:13 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:07:13 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:07:15 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:07:39 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "$SONARQUBE_ZIP_URL"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:07:39 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:07:40 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:07:40 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:07:40 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1dbf1b27574ac1a1544a294210a80f0d970e27ebe6bdb8d1cff9b16963288c`  
		Last Modified: Fri, 17 Apr 2020 10:10:10 GMT  
		Size: 15.0 KB (14985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53862f08bedebd5850edaaad4593475c92f663901f96ff9242bfc0732c4648`  
		Last Modified: Fri, 17 Apr 2020 10:10:53 GMT  
		Size: 282.6 MB (282612678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675085a12b56f4404a8c8419d863f3366b889adcd4f0e0037c0fb057b3610a9e`  
		Last Modified: Fri, 17 Apr 2020 10:10:09 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:enterprise`

```console
$ docker pull sonarqube@sha256:ae7a23c9e0e264f6c33f1ffd1c8a5d9a6828356fec1e7d999cf06eb7be837d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:c9a0ea9f2babd56c02d3e12d4544d7bc5c1d2022c3e220a0be424b892496826e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.7 MB (385723404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc0cef885e631e0e2b70f1ec40ae58940f574c7d0ad9b363c0388bb489926cc`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:07:48 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:07:48 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:07:48 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:07:50 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:08:15 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "${SONARQUBE_ZIP_URL}"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:08:15 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:08:16 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:08:16 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:08:17 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be03a705f7c2a3c69e5e5c9a1b0b7990352c89836a97f77118a30d45d5ac538c`  
		Last Modified: Fri, 17 Apr 2020 10:11:10 GMT  
		Size: 15.0 KB (14984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1e7c2c39f6ea061e18396433a787caa1ccb95f0bec10e025869f9be490f10e`  
		Last Modified: Fri, 17 Apr 2020 10:11:55 GMT  
		Size: 304.4 MB (304434679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f854954293c64504fa762935fc02e69af241505c2970106bf576d70f72e23a`  
		Last Modified: Fri, 17 Apr 2020 10:11:10 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:latest`

```console
$ docker pull sonarqube@sha256:ee95412e0b61d5127b377c0b6d141d814e1d7cbcffff64933194da48634fb95d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:latest` - linux; amd64

```console
$ docker pull sonarqube@sha256:52e1a3fcae6fb805cecb2894aee6b09ab0dd5d5b84fd0ba25269e2911bc95314
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302191326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5203e55f281cc9a6ee9ce53848b238890667b9f7ddd56cbf7246ab12cc682eb`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:06:39 GMT
RUN apt-get update     && apt-get install -y curl unzip gnupg2 libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:06:39 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:06:41 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:06:42 GMT
ARG SONARQUBE_VERSION=8.2.0.32929
# Fri, 17 Apr 2020 10:06:43 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
# Fri, 17 Apr 2020 10:06:43 GMT
ENV SONAR_VERSION=8.2.0.32929 SONARQUBE_HOME=/opt/sonarqube
# Fri, 17 Apr 2020 10:06:43 GMT
SHELL [/bin/bash -c]
# Fri, 17 Apr 2020 10:06:45 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Fri, 17 Apr 2020 10:07:04 GMT
# ARGS: SONARQUBE_VERSION=8.2.0.32929 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.2.0.32929.zip
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;   done     && set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "$SONARQUBE_ZIP_URL"     && curl -o sonarqube.zip.asc -fSL "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME"
# Fri, 17 Apr 2020 10:07:05 GMT
COPY --chown=sonarqube:sonarqubefile:b67f51917544737172cd7539a3a3c97397219c52ca27cd8feedde9b53f20a97c in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:07:05 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:07:05 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:07:05 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2e2bfb9c2757188574959a8c4072e10aee60863d73b7da3616a887e8dc0da1`  
		Last Modified: Fri, 17 Apr 2020 10:09:42 GMT  
		Size: 8.7 MB (8709085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef439a9c382059aecd35eda48240d22848a78c68e60b325e9760a32ab40087da`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea3e87bd78a1afaab4f8e797b652c72104c27067895218b886412693f4e4f26`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 15.0 KB (14984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3695f3dc51df741c3dc99b525335973a82f2001dd8e215b19df752b98e94608c`  
		Last Modified: Fri, 17 Apr 2020 10:10:02 GMT  
		Size: 220.9 MB (220902607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d71901465c1fed918cf4c3d0a39722014f700ca3b8d6c2af21aad0828374c9`  
		Last Modified: Fri, 17 Apr 2020 10:09:38 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:lts`

```console
$ docker pull sonarqube@sha256:daf51eb642f84c9e280dcb0cb5dfc9a7853beb8e2796cbad0db0d18f80393f45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:lts` - linux; amd64

```console
$ docker pull sonarqube@sha256:cb045a7b46f913fb07e0c7c46ab62879fb78eb252200008428d5667f3c396c59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.7 MB (286696139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c26581d4b9b54446d7b09d59808bdaa05da41df4a6a0bf2aeafba6066600794`
-	Entrypoint: `[".\/bin\/run.sh"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 10:16:26 GMT
ENV LANG=C.UTF-8
# Thu, 16 Apr 2020 10:19:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 16 Apr 2020 10:19:13 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 10:19:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 16 Apr 2020 10:19:14 GMT
ENV JAVA_VERSION=11.0.7
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Thu, 16 Apr 2020 10:20:16 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Thu, 16 Apr 2020 10:20:33 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 17 Apr 2020 10:05:50 GMT
RUN apt-get update     && apt-get install -y curl gnupg2 unzip     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:05:51 GMT
ENV SONAR_VERSION=7.9.3 SONARQUBE_HOME=/opt/sonarqube SONARQUBE_JDBC_USERNAME=sonar SONARQUBE_JDBC_PASSWORD=sonar SONARQUBE_JDBC_URL=
# Fri, 17 Apr 2020 10:05:51 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 10:05:52 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Fri, 17 Apr 2020 10:05:54 GMT
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done
# Fri, 17 Apr 2020 10:06:13 GMT
RUN set -x     && cd /opt     && curl -o sonarqube.zip -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip     && curl -o sonarqube.zip.asc -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip.asc     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv sonarqube-$SONAR_VERSION sonarqube     && chown -R sonarqube:sonarqube sonarqube     && rm sonarqube.zip*     && rm -rf $SONARQUBE_HOME/bin/*
# Fri, 17 Apr 2020 10:06:14 GMT
VOLUME [/opt/sonarqube/data]
# Fri, 17 Apr 2020 10:06:14 GMT
WORKDIR /opt/sonarqube
# Fri, 17 Apr 2020 10:06:14 GMT
COPY file:aa007fcc6be4125cbbb27fe345978294add03a4f05e942a5208a37be832addca in /opt/sonarqube/bin/ 
# Fri, 17 Apr 2020 10:06:15 GMT
USER sonarqube
# Fri, 17 Apr 2020 10:06:15 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2750eaebe665cac8881d45b8ac3ca818589f2e864b46191ed16b27b4839a087e`  
		Last Modified: Thu, 16 Apr 2020 10:23:39 GMT  
		Size: 3.2 MB (3249138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ad45fdc1358fe836a11f8750e2d244ac475142f1e4e3570954e98a2facd7bc`  
		Last Modified: Thu, 16 Apr 2020 10:26:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51062359ac505e3fe04d4099b00c6ffbf57552f66e928de3296199592a980f9`  
		Last Modified: Thu, 16 Apr 2020 10:27:41 GMT  
		Size: 42.2 MB (42214702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583424677bf8a2a7d1ebe176293a64c39bbb8d6ba8d12048f013af4e941a3861`  
		Last Modified: Fri, 17 Apr 2020 10:08:41 GMT  
		Size: 6.0 MB (5984876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560b7570bd8332051d2fb4092d83568328013ac71dd9eeedab37a70b56c14e74`  
		Last Modified: Fri, 17 Apr 2020 10:08:39 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96baee3083f83f3f3289a64c8e9e7aa820e138048f6f888a65158dbf1133ca2`  
		Last Modified: Fri, 17 Apr 2020 10:08:40 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aebcb2200f2e6423966a59142d662a1dd140537df2a20099db1d7cabb8c6e9`  
		Last Modified: Fri, 17 Apr 2020 10:09:29 GMT  
		Size: 208.1 MB (208144762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abadafa5ab9541945485f7a713fd09f2c3319ed68335c8419416d9e2c060c10`  
		Last Modified: Fri, 17 Apr 2020 10:08:40 GMT  
		Size: 789.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
