## `groovy:jdk11-alpine`

```console
$ docker pull groovy@sha256:dc45532f4205f130c45dade35baedec1ded9737e810fd963f58733d6456bdb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `groovy:jdk11-alpine` - linux; amd64

```console
$ docker pull groovy@sha256:3afe589f2c259e9ad9ddfac09e2298c26821615cc34233f1b092a81dd96aaed4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.6 MB (182557774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25dfd46958f740727da917e3d9d1473a3e2c86beb20009e49bde7016becdd71e`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["groovysh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 19:19:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 08 Aug 2023 19:19:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 19:19:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 14 Aug 2023 18:09:08 GMT
RUN apk add --no-cache fontconfig java-cacerts bash libretls musl-locales musl-locales-lang ttf-dejavu tzdata zlib     && rm -rf /var/cache/apk/*
# Thu, 31 Aug 2023 20:21:36 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Thu, 31 Aug 2023 20:21:46 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1a94e642bf6cc4124d4f01f43184f9127ef994cbd324e2ee42cc50f715cbaedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_alpine-linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Thu, 31 Aug 2023 20:21:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 31 Aug 2023 20:21:48 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 31 Aug 2023 20:21:48 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 31 Aug 2023 20:21:48 GMT
CMD ["jshell"]
# Thu, 31 Aug 2023 22:49:59 GMT
CMD ["groovysh"]
# Thu, 31 Aug 2023 22:49:59 GMT
ENV GROOVY_HOME=/opt/groovy
# Thu, 31 Aug 2023 22:50:00 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && addgroup --system --gid 1000 groovy     && adduser --system --ingroup groovy --uid 1000 --shell /bin/ash groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown -R groovy:groovy /home/groovy     && chmod -R 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln -s /home/groovy/.groovy /root/.groovy
# Thu, 31 Aug 2023 22:50:00 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Thu, 31 Aug 2023 22:50:00 GMT
WORKDIR /home/groovy
# Thu, 31 Aug 2023 22:50:00 GMT
ENV GROOVY_VERSION=4.0.14
# Thu, 31 Aug 2023 22:50:10 GMT
RUN set -o errexit -o nounset     && echo "Installing build dependencies"     && apk add --no-cache --virtual .build-deps         gnupg         && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver keyserver.ubuntu.com --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm -rf "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Cleaning up build dependencies"     && apk del .build-deps         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln -s "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln -s "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln -s "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln -s "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln -s "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln -s "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln -s "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Thu, 31 Aug 2023 22:50:10 GMT
USER 1000:1000
# Thu, 31 Aug 2023 22:50:11 GMT
RUN set -o errexit -o nounset     && echo "Testing Groovy installation"     && groovy --version
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994e83f716a0db024fb37caf707eae5af27172a0fffb691c6e7b53bb7fc5b3ab`  
		Last Modified: Mon, 14 Aug 2023 18:13:07 GMT  
		Size: 9.3 MB (9276497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87612432044feedbbd160768378d6ac4be8b858919286406656abe0e39f3b02`  
		Last Modified: Thu, 31 Aug 2023 20:26:56 GMT  
		Size: 140.2 MB (140159211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd8607be42c68560b61b558999dbf89b35809682e184ce167f68b3b3d13d535`  
		Last Modified: Thu, 31 Aug 2023 20:26:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84006294e89afa4503c260d37d954994c01e322584f766b9c6bd539ca3458da`  
		Last Modified: Thu, 31 Aug 2023 20:26:45 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c0fde0a251d14662fd64925f35660dd08e8a27b1cc18a222fdd56c0787fb38`  
		Last Modified: Thu, 31 Aug 2023 22:51:35 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc24c38025b3bbed7556cd91f71dec2e01ddd173f92bc83388e01833558a369`  
		Last Modified: Thu, 31 Aug 2023 22:51:36 GMT  
		Size: 29.7 MB (29718016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efff0d40000e5c2153fe47eaa08b4fe13e95d781ffd77535e4c03bae0075d66`  
		Last Modified: Thu, 31 Aug 2023 22:51:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
