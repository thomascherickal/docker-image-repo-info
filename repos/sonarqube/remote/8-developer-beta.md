## `sonarqube:8-developer-beta`

```console
$ docker pull sonarqube@sha256:3fb9544074a3aeb45f365dcf82764c76243d904e86cd3d339783f3844088b683
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8-developer-beta` - linux; amd64

```console
$ docker pull sonarqube@sha256:1f637516f48bafe13b764100d42f267716de1757190c29c44c1dc2329f6b64db
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **470.4 MB (470385239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d53dc5ea74aa5ba4e6795e4bb5ff879dbab2627364115e4df972c6e5cbd9a066`
-	Entrypoint: `[".\/bin\/run.sh"]`
-	`SHELL`: `["\/bin\/bash","-c"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 19:14:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 19:14:45 GMT
ENV LANG=C.UTF-8
# Fri, 22 Nov 2019 19:16:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 22 Nov 2019 19:16:21 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 19:16:22 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 22 Nov 2019 19:16:22 GMT
ENV JAVA_VERSION=11.0.5
# Fri, 22 Nov 2019 19:16:58 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jre_
# Fri, 22 Nov 2019 19:16:58 GMT
ENV JAVA_URL_VERSION=11.0.5_10
# Fri, 22 Nov 2019 19:17:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Thu, 19 Dec 2019 04:16:48 GMT
RUN apt-get update     && apt-get install -y curl unzip libfreetype6 libfontconfig1     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:16:48 GMT
EXPOSE 9000
# Thu, 19 Dec 2019 04:16:49 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Thu, 19 Dec 2019 04:16:49 GMT
ARG SONARQUBE_VERSION=8.1.0.31237
# Thu, 19 Dec 2019 04:17:12 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.1.0.31237.zip
# Thu, 19 Dec 2019 04:17:12 GMT
ENV SONAR_VERSION=8.1.0.31237 SONARQUBE_HOME=/opt/sq SONARQUBE_PUBLIC_HOME=/opt/sonarqube
# Thu, 19 Dec 2019 04:17:13 GMT
SHELL [/bin/bash -c]
# Thu, 19 Dec 2019 04:17:13 GMT
# ARGS: SONARQUBE_VERSION=8.1.0.31237 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.1.0.31237.zip
RUN sed -i -e "s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g"   "$JAVA_HOME/conf/security/java.security"
# Thu, 19 Dec 2019 04:17:30 GMT
# ARGS: SONARQUBE_VERSION=8.1.0.31237 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.1.0.31237.zip
RUN set -x     && cd /opt     && curl -o sonarqube.zip -fsSL "$SONARQUBE_ZIP_URL"     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sq     && rm sonarqube.zip*     && rm --recursive --force "$SONARQUBE_HOME/bin"/*     && mv "$SONARQUBE_HOME/conf" "$SONARQUBE_HOME/conf_save"     && mv "$SONARQUBE_HOME/extensions" "$SONARQUBE_HOME/extensions_save"     && rm --recursive --force "$SONARQUBE_HOME/logs"     && rm --recursive --force "$SONARQUBE_HOME/data"     && mkdir --parents "$SONARQUBE_PUBLIC_HOME/conf"     && mkdir --parents "$SONARQUBE_PUBLIC_HOME/extensions"     && mkdir --parents "$SONARQUBE_PUBLIC_HOME/logs"     && mkdir --parents "$SONARQUBE_PUBLIC_HOME/data"     && cp --recursive "$SONARQUBE_HOME/conf_save"/* "$SONARQUBE_PUBLIC_HOME/conf/"     && cp --recursive "$SONARQUBE_HOME/extensions_save"/* "$SONARQUBE_PUBLIC_HOME/extensions/"     && ln -s "$SONARQUBE_PUBLIC_HOME/conf" "$SONARQUBE_HOME/conf"     && ln -s "$SONARQUBE_PUBLIC_HOME/extensions" "$SONARQUBE_HOME/extensions"     && ln -s "$SONARQUBE_PUBLIC_HOME/logs" "$SONARQUBE_HOME/logs"     && ln -s "$SONARQUBE_PUBLIC_HOME/data" "$SONARQUBE_HOME/data"     && chown --recursive sonarqube:sonarqube "$SONARQUBE_HOME" "$SONARQUBE_PUBLIC_HOME"
# Thu, 19 Dec 2019 04:17:30 GMT
COPY --chown=sonarqube:sonarqubefile:7e8bed266915cfbc07c846686c59039a89cda10c59553d4ba545b4c34d032e46 in /opt/sq/bin/ 
# Thu, 19 Dec 2019 04:17:31 GMT
USER sonarqube
# Thu, 19 Dec 2019 04:17:31 GMT
WORKDIR /opt/sq
# Thu, 19 Dec 2019 04:17:31 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dc2bdcfe193ce54affa45170354ca76667c40f8cf536b6282dd379e17e24a`  
		Last Modified: Fri, 22 Nov 2019 19:19:08 GMT  
		Size: 3.2 MB (3249119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec880363624c27ef6cc7e146eb42bb15e84efbfe8f365f8ed8718804b44c61b`  
		Last Modified: Fri, 22 Nov 2019 19:20:24 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8992c959a11ddefb3735efc010a2d670c008659dccb4712b85b3428c25437a0d`  
		Last Modified: Fri, 22 Nov 2019 19:21:16 GMT  
		Size: 42.1 MB (42105011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a0cd249fd61fb683eb60f2aeba08fb7d001e1b479ea34dd716c0ac6851418c`  
		Last Modified: Thu, 19 Dec 2019 04:18:36 GMT  
		Size: 5.0 MB (5030519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467c3f9c05c1a74fe93adfaf5f2dae75cb9ec60939d58ebbe90649235afc8fc7`  
		Last Modified: Thu, 19 Dec 2019 04:18:35 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0caf629446c2fe2988f8265e46c8e1ebbf6f8a59a4acf7ae745b3c7b50088a`  
		Last Modified: Thu, 19 Dec 2019 04:19:04 GMT  
		Size: 14.5 KB (14463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3411161327cd7e9fcb2ec19f078bf54729de82f575c363556199d633869132d`  
		Last Modified: Thu, 19 Dec 2019 04:19:31 GMT  
		Size: 392.9 MB (392890423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14b505930810b3fa7f182b04ed09f5aeb65df29f5277f249a232a690c6e2ff4`  
		Last Modified: Thu, 19 Dec 2019 04:19:04 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
