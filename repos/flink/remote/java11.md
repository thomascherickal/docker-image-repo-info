## `flink:java11`

```console
$ docker pull flink@sha256:d5725a71cfefaf9ccb119ba31a2f44f00565ca97a78d38c91d1b30436ef0371a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `flink:java11` - linux; amd64

```console
$ docker pull flink@sha256:715ecb004499f1ac2576ac234e1139253bf9399569e0fd464a115e847be09529
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.7 MB (569742898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7f7788fc322040bc0c08ff55f15e7c24a9d41f9f56f6c35733306f06b43d9e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 20:27:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:27:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:27:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 20:27:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:28:17 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 31 Jan 2023 20:28:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 31 Jan 2023 20:28:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 01 Feb 2023 01:44:23 GMT
RUN set -ex;   apt-get update;   apt-get -y install gpg libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 01:44:23 GMT
ENV GOSU_VERSION=1.11
# Wed, 01 Feb 2023 01:44:29 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Wed, 01 Feb 2023 23:10:41 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.16.1/flink-1.16.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.16.1/flink-1.16.1-bin-scala_2.12.tgz.asc GPG_KEY=A5F3BCE4CBE993573EC5966A65321B8382B219AF CHECK_GPG=true
# Wed, 01 Feb 2023 23:10:41 GMT
ENV FLINK_HOME=/opt/flink
# Wed, 01 Feb 2023 23:10:41 GMT
ENV PATH=/opt/flink/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Feb 2023 23:10:41 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Wed, 01 Feb 2023 23:10:42 GMT
WORKDIR /opt/flink
# Wed, 01 Feb 2023 23:11:30 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;     sed -i 's/rest.address: localhost/rest.address: 0.0.0.0/g' $FLINK_HOME/conf/flink-conf.yaml;   sed -i 's/rest.bind-address: localhost/rest.bind-address: 0.0.0.0/g' $FLINK_HOME/conf/flink-conf.yaml;   sed -i 's/jobmanager.bind-host: localhost/jobmanager.bind-host: 0.0.0.0/g' $FLINK_HOME/conf/flink-conf.yaml;   sed -i 's/taskmanager.bind-host: localhost/taskmanager.bind-host: 0.0.0.0/g' $FLINK_HOME/conf/flink-conf.yaml;   sed -i '/taskmanager.host: localhost/d' $FLINK_HOME/conf/flink-conf.yaml;
# Wed, 01 Feb 2023 23:11:31 GMT
COPY file:ab8cf5711c2ee73018994cee7133a7f61b2e5fca388abbb79b5eac61bf7f4fa3 in / 
# Wed, 01 Feb 2023 23:11:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 23:11:31 GMT
EXPOSE 6123 8081
# Wed, 01 Feb 2023 23:11:31 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b99dc26ba300e0f809f00511dcac6ceb6c9dde4a5c0a7288225868d3a7df21`  
		Last Modified: Tue, 31 Jan 2023 20:33:44 GMT  
		Size: 12.4 MB (12431335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475d0703f5bc1c862565817c8cca45229e0c4353ec8bbf2bf354818548bd740a`  
		Last Modified: Tue, 31 Jan 2023 20:35:45 GMT  
		Size: 46.6 MB (46635607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2576264bf764d7f43ca167c0598daa092b2266d16587f8363005f491d311759`  
		Last Modified: Tue, 31 Jan 2023 20:35:38 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c69bee068beb6999a6c69205883ecc89d327c329e7a5c5643b47584e8d8c515`  
		Last Modified: Wed, 01 Feb 2023 01:47:05 GMT  
		Size: 4.7 MB (4652943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271d90aec04b15a892aa4fd8f1e367c0af24977fabfe0c0193bad2403823777f`  
		Last Modified: Wed, 01 Feb 2023 01:47:03 GMT  
		Size: 900.5 KB (900507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311a357cfbfd93f8412aec814eda60557c16c164635cf83a5f48319ea1dda380`  
		Last Modified: Wed, 01 Feb 2023 23:12:51 GMT  
		Size: 4.6 KB (4611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03835db286a38a53c44013589485bb0a1367b9307a283a6e8d9d9c3cb8ca9cc0`  
		Last Modified: Wed, 01 Feb 2023 23:12:50 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc230ef9ef457c616a65313ae23aaad98cd56db55cb4a9a7448929d09bbcdb7`  
		Last Modified: Wed, 01 Feb 2023 23:13:11 GMT  
		Size: 474.7 MB (474686473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f75d90510726a020d5be0815aefad28a3c752ed34a1bc65a76eae5ac9a827e6`  
		Last Modified: Wed, 01 Feb 2023 23:12:50 GMT  
		Size: 2.1 KB (2110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `flink:java11` - linux; arm64 variant v8

```console
$ docker pull flink@sha256:af3dff2df7891b5ef6193e3b6493e676cebf4b0180b784bc3a9b54943f75c8d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.8 MB (565787924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595b8abc0c0680d23ef1ad14828242c22b9b0ebdb0a90c444d7095d52ed9f966`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["help"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:27:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:27:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:27:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:27:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:28:47 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Thu, 02 Mar 2023 04:29:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:29:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 08:09:08 GMT
RUN set -ex;   apt-get update;   apt-get -y install gpg libsnappy1v5 gettext-base libjemalloc-dev;   rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 08:09:08 GMT
ENV GOSU_VERSION=1.11
# Thu, 02 Mar 2023 08:09:30 GMT
RUN set -ex;   wget -nv -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)";   wget -nv -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc";   export GNUPGHOME="$(mktemp -d)";   for server in ha.pool.sks-keyservers.net $(shuf -e                           hkp://p80.pool.sks-keyservers.net:80                           keyserver.ubuntu.com                           hkp://keyserver.ubuntu.com:80                           pgp.mit.edu) ; do       gpg --batch --keyserver "$server" --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;   done &&   gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;   gpgconf --kill all;   rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;   chmod +x /usr/local/bin/gosu;   gosu nobody true
# Thu, 02 Mar 2023 08:09:30 GMT
ENV FLINK_TGZ_URL=https://www.apache.org/dyn/closer.cgi?action=download&filename=flink/flink-1.16.1/flink-1.16.1-bin-scala_2.12.tgz FLINK_ASC_URL=https://www.apache.org/dist/flink/flink-1.16.1/flink-1.16.1-bin-scala_2.12.tgz.asc GPG_KEY=A5F3BCE4CBE993573EC5966A65321B8382B219AF CHECK_GPG=true
# Thu, 02 Mar 2023 08:09:30 GMT
ENV FLINK_HOME=/opt/flink
# Thu, 02 Mar 2023 08:09:30 GMT
ENV PATH=/opt/flink/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 08:09:31 GMT
RUN groupadd --system --gid=9999 flink &&     useradd --system --home-dir $FLINK_HOME --uid=9999 --gid=flink flink
# Thu, 02 Mar 2023 08:09:31 GMT
WORKDIR /opt/flink
# Thu, 02 Mar 2023 08:10:04 GMT
RUN set -ex;   wget -nv -O flink.tgz "$FLINK_TGZ_URL";     if [ "$CHECK_GPG" = "true" ]; then     wget -nv -O flink.tgz.asc "$FLINK_ASC_URL";     export GNUPGHOME="$(mktemp -d)";     for server in ha.pool.sks-keyservers.net $(shuf -e                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys "$GPG_KEY" && break || : ;     done &&     gpg --batch --verify flink.tgz.asc flink.tgz;     gpgconf --kill all;     rm -rf "$GNUPGHOME" flink.tgz.asc;   fi;     tar -xf flink.tgz --strip-components=1;   rm flink.tgz;     chown -R flink:flink .;     sed -i 's/rest.address: localhost/rest.address: 0.0.0.0/g' $FLINK_HOME/conf/flink-conf.yaml;   sed -i 's/rest.bind-address: localhost/rest.bind-address: 0.0.0.0/g' $FLINK_HOME/conf/flink-conf.yaml;   sed -i 's/jobmanager.bind-host: localhost/jobmanager.bind-host: 0.0.0.0/g' $FLINK_HOME/conf/flink-conf.yaml;   sed -i 's/taskmanager.bind-host: localhost/taskmanager.bind-host: 0.0.0.0/g' $FLINK_HOME/conf/flink-conf.yaml;   sed -i '/taskmanager.host: localhost/d' $FLINK_HOME/conf/flink-conf.yaml;
# Thu, 02 Mar 2023 08:10:08 GMT
COPY file:ab8cf5711c2ee73018994cee7133a7f61b2e5fca388abbb79b5eac61bf7f4fa3 in / 
# Thu, 02 Mar 2023 08:10:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 02 Mar 2023 08:10:08 GMT
EXPOSE 6123 8081
# Thu, 02 Mar 2023 08:10:08 GMT
CMD ["help"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ba20309dcd99cff3a43c2f3c01df9170ee1fe02df71ead98cfcef30b9c450`  
		Last Modified: Thu, 02 Mar 2023 04:33:24 GMT  
		Size: 12.4 MB (12390219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d5722bd69e931b1cf3e955e992893a8ea2e124b586c19b553fbe8a2d94f988`  
		Last Modified: Thu, 02 Mar 2023 04:35:11 GMT  
		Size: 45.0 MB (44977970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2d1016d6ffd5bed4cc6724687b1659787f8e3d1c112f02173b5efcb5425180`  
		Last Modified: Thu, 02 Mar 2023 04:35:06 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b50c42c75cbde6960c93fe285ec78a395a569606409b42d5e7170d2e1d7bd0`  
		Last Modified: Thu, 02 Mar 2023 08:12:11 GMT  
		Size: 4.5 MB (4502911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28c7e219afda3fe21e97828fb1134cd7534177e26b54127d3dc08c896442cb3`  
		Last Modified: Thu, 02 Mar 2023 08:12:09 GMT  
		Size: 835.4 KB (835392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2825c7e7c278423ed923ff7c4b547306ae7590fbde16671d1dcd1a697d323031`  
		Last Modified: Thu, 02 Mar 2023 08:12:08 GMT  
		Size: 4.6 KB (4648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a898382f2073c36991498f26fe3db5dd977906a6890a9c45549f10f012649fb6`  
		Last Modified: Thu, 02 Mar 2023 08:12:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43805a79483239b8da5d207c68d7f1e2c9afc62e04d37d89bd14250d775a2b20`  
		Last Modified: Thu, 02 Mar 2023 08:12:25 GMT  
		Size: 474.7 MB (474686446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfdc59cd154c2c1291c5f17053662f7919213da68445bc460f3465d78937288`  
		Last Modified: Thu, 02 Mar 2023 08:12:08 GMT  
		Size: 2.1 KB (2110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
