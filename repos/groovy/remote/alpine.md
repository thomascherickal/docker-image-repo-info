## `groovy:alpine`

```console
$ docker pull groovy@sha256:1edc4478e09bd5d344d09bc18b8962f1634c1e8e2962bec31a9f7508bb49890d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `groovy:alpine` - linux; amd64

```console
$ docker pull groovy@sha256:a1f8851edf74e8782212f028eacbdce8be19766c37286f37a8d891671e83dea2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.5 MB (186516276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d47b74bc1d2e78df514f1ac06f00cdf18ca811e21a35dc2d3a7da66c75d687d`
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
# Thu, 31 Aug 2023 20:23:30 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Thu, 31 Aug 2023 20:23:40 GMT
RUN set -eux;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='85d298268db61c4a538df905ec510eba7dc09300e7f7132bb2e25e5e8aef1933';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_x64_alpine-linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;
# Thu, 31 Aug 2023 20:23:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 31 Aug 2023 20:23:43 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 31 Aug 2023 20:23:43 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 31 Aug 2023 20:23:43 GMT
CMD ["jshell"]
# Thu, 31 Aug 2023 22:50:36 GMT
CMD ["groovysh"]
# Thu, 31 Aug 2023 22:50:37 GMT
ENV GROOVY_HOME=/opt/groovy
# Thu, 31 Aug 2023 22:50:37 GMT
RUN set -o errexit -o nounset     && echo "Adding groovy user and group"     && addgroup --system --gid 1000 groovy     && adduser --system --ingroup groovy --uid 1000 --shell /bin/ash groovy     && mkdir --parents /home/groovy/.groovy/grapes     && chown -R groovy:groovy /home/groovy     && chmod -R 1777 /home/groovy         && echo "Symlinking root .groovy to groovy .groovy"     && ln -s /home/groovy/.groovy /root/.groovy
# Thu, 31 Aug 2023 22:50:37 GMT
VOLUME [/home/groovy/.groovy/grapes]
# Thu, 31 Aug 2023 22:50:37 GMT
WORKDIR /home/groovy
# Thu, 14 Sep 2023 22:33:46 GMT
ENV GROOVY_VERSION=4.0.15
# Thu, 14 Sep 2023 22:33:56 GMT
RUN set -o errexit -o nounset     && echo "Installing build dependencies"     && apk add --no-cache --virtual .build-deps         gnupg         && echo "Downloading Groovy"     && wget --no-verbose --output-document=groovy.zip "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip"         && echo "Importing keys listed in http://www.apache.org/dist/groovy/KEYS from key server"     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --no-tty --keyserver keyserver.ubuntu.com --recv-keys         7FAA0F2206DE228F0DB01AD741321490758AAD6F         331224E1D7BE883D16E8A685825C06C827AF6B66         34441E504A937F43EB0DAEF96A65176A0FB1CD0B         9A810E3B766E089FFB27C70F11B595CEDC4AEBB5         81CABC23EECA0790E8989B361FF96E10F0E13706         && echo "Checking download signature"     && wget --no-verbose --output-document=groovy.zip.asc "https://archive.apache.org/dist/groovy/${GROOVY_VERSION}/distribution/apache-groovy-binary-${GROOVY_VERSION}.zip.asc"     && gpg --batch --no-tty --verify groovy.zip.asc groovy.zip     && rm -rf "${GNUPGHOME}"     && rm groovy.zip.asc         && echo "Cleaning up build dependencies"     && apk del .build-deps         && echo "Installing Groovy"     && unzip groovy.zip     && rm groovy.zip     && mv "groovy-${GROOVY_VERSION}" "${GROOVY_HOME}/"     && ln -s "${GROOVY_HOME}/bin/grape" /usr/bin/grape     && ln -s "${GROOVY_HOME}/bin/groovy" /usr/bin/groovy     && ln -s "${GROOVY_HOME}/bin/groovyc" /usr/bin/groovyc     && ln -s "${GROOVY_HOME}/bin/groovyConsole" /usr/bin/groovyConsole     && ln -s "${GROOVY_HOME}/bin/groovydoc" /usr/bin/groovydoc     && ln -s "${GROOVY_HOME}/bin/groovysh" /usr/bin/groovysh     && ln -s "${GROOVY_HOME}/bin/java2groovy" /usr/bin/java2groovy         && echo "Editing startGroovy to include java.xml.bind module"     && sed --in-place 's|startGroovy ( ) {|startGroovy ( ) {\n    JAVA_OPTS="$JAVA_OPTS --add-modules=ALL-SYSTEM"|' "${GROOVY_HOME}/bin/startGroovy"
# Thu, 14 Sep 2023 22:33:56 GMT
USER 1000:1000
# Thu, 14 Sep 2023 22:33:57 GMT
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
	-	`sha256:aadc5b7e0214f710a0879304f390e9594ed19078f820eaad2017264866baa175`  
		Last Modified: Thu, 31 Aug 2023 20:30:08 GMT  
		Size: 144.1 MB (144102415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba060933c7942f0ec8c39e0d52961c4bd0f163bf394b6e2456242494bfbf679f`  
		Last Modified: Thu, 31 Aug 2023 20:29:57 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c636a3b00e19e4e7cf14f5ae0909805ecc4018ea34a691725560bc0594c9d52a`  
		Last Modified: Thu, 31 Aug 2023 20:29:56 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a66dac48868b0095c01d793f2d362dc942217dece7712025481781be6e9da3c`  
		Last Modified: Thu, 31 Aug 2023 22:52:33 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1506e66f1ef9a5036cc8ec76d320447b788822ee427cb024c71a5afb3f6cd497`  
		Last Modified: Thu, 14 Sep 2023 22:36:22 GMT  
		Size: 29.7 MB (29733311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa084e33d89ce4e7306692e49bcad2129d8b20c4c1a38157d29df0a162e25b8`  
		Last Modified: Thu, 14 Sep 2023 22:36:19 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
