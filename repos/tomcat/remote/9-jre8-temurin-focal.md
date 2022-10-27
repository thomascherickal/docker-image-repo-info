## `tomcat:9-jre8-temurin-focal`

```console
$ docker pull tomcat@sha256:a04c8470c3ac570fb40b80cfd2405d59d002f2c97bde5fce48392e86ba0c9170
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:9-jre8-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:af51fdff8f860be8637b7ca267391e46caec14f93c561db4f09e96a875ed689a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99444865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f625647da26884d613a7cf9424812d4bb6f901f54706898e259685013921614d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:27:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 17:27:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 17:27:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 17:27:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 17:27:46 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Tue, 25 Oct 2022 17:28:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 25 Oct 2022 17:28:32 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Oct 2022 23:49:44 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 23:49:44 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 23:49:45 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 23:49:45 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 23:49:45 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 23:49:45 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 23:54:52 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Oct 2022 23:54:52 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Oct 2022 23:54:52 GMT
ENV TOMCAT_VERSION=9.0.68
# Wed, 26 Oct 2022 23:54:52 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Wed, 26 Oct 2022 23:54:52 GMT
COPY dir:6a40b1abe3a008eb1072d867c7683b68644a51957d70b2ebef120d531ba5d741 in /usr/local/tomcat 
# Wed, 26 Oct 2022 23:54:57 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 23:54:58 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 23:54:58 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 23:54:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1869246ce33b7e9d4cfc0f2be772ef684e2425767400664f548b81c2a69eb`  
		Last Modified: Tue, 25 Oct 2022 17:33:48 GMT  
		Size: 16.4 MB (16353656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec745e019fcec97ad385550869975f32c84d380c2e1e0144f7adf645c8b4e1a`  
		Last Modified: Wed, 26 Oct 2022 16:43:39 GMT  
		Size: 41.8 MB (41808475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebeffd81f32972bf834384b283b12d171bd004c2dfdb5b66091154fff8c6f93c`  
		Last Modified: Wed, 26 Oct 2022 16:43:34 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02af61b53089943d5094ab161d49505f8ce872bbfd5db4c18bd05e8db01bcd63`  
		Last Modified: Thu, 27 Oct 2022 00:10:12 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1299527e4744357a50541c6a238c86ed8827b94d6a7066359b00b1eed1d82b10`  
		Last Modified: Thu, 27 Oct 2022 00:14:40 GMT  
		Size: 12.3 MB (12256036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461a559e383a9539c86abb7ab1595d6ba52d1997568ca8ab613d86cf0e894f67`  
		Last Modified: Thu, 27 Oct 2022 00:14:39 GMT  
		Size: 448.4 KB (448402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986662bdb947fe0cd3c27b18b4297bff3ffeab92a004d2eba82b16a6423238dd`  
		Last Modified: Thu, 27 Oct 2022 00:14:39 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:dce89c898d87ef356b0d65d22685a3766decdf4eee5dc88b60996541227dbd2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91941877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b268342536db3e2a195c68ec19afdcd8c0120c16aca9084eba30f36f3bb7e5ea`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:44 GMT
ADD file:75870468a948359044fa3df6c07c80badfea3dcde4823d41a19285436c40cf76 in / 
# Wed, 05 Oct 2022 00:13:44 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:29:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 06 Oct 2022 06:29:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 06:29:55 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 06 Oct 2022 06:30:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:30:13 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 06 Oct 2022 06:31:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 06 Oct 2022 06:31:25 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 07 Oct 2022 06:17:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 07 Oct 2022 06:17:29 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 06:17:29 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 07 Oct 2022 06:17:30 GMT
WORKDIR /usr/local/tomcat
# Fri, 07 Oct 2022 06:17:30 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 07 Oct 2022 06:17:30 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 07 Oct 2022 06:26:31 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 07 Oct 2022 06:26:31 GMT
ENV TOMCAT_MAJOR=9
# Sat, 08 Oct 2022 05:51:17 GMT
ENV TOMCAT_VERSION=9.0.68
# Sat, 08 Oct 2022 05:51:17 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Sat, 08 Oct 2022 05:51:18 GMT
COPY dir:b9517124fc6e5782ce7109071b8506ed756e6e01588e377025cf81b6291ad8bd in /usr/local/tomcat 
# Sat, 08 Oct 2022 05:51:26 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 08 Oct 2022 05:51:27 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 08 Oct 2022 05:51:27 GMT
EXPOSE 8080
# Sat, 08 Oct 2022 05:51:27 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e679d63f382033c15f8f921851bd71fb8a85a432c0a7a612bbef16e989075145`  
		Last Modified: Wed, 05 Oct 2022 00:15:44 GMT  
		Size: 24.6 MB (24590092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f29375a8d8574bfb25c0882725d6597aed6c594925cd62b3e2c024e61ac90e8`  
		Last Modified: Thu, 06 Oct 2022 06:39:16 GMT  
		Size: 15.2 MB (15180337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2f034f987dd8b177db74818633138d1932860a551239bfd01b33613bdf650d`  
		Last Modified: Thu, 06 Oct 2022 06:40:08 GMT  
		Size: 39.5 MB (39539727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766a569d5de14087d590be180c3af06fb0da8d601549076070c914043e4cf760`  
		Last Modified: Thu, 06 Oct 2022 06:40:03 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c7b8571191805d4884cc1a72ee95e1f0f792a149ef03ad96f423362c01186e`  
		Last Modified: Fri, 07 Oct 2022 06:54:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c1dec382faaf56f8d583b94841d5bc65071fd30f6736c9ec8a4de418db146b`  
		Last Modified: Sat, 08 Oct 2022 06:09:21 GMT  
		Size: 12.2 MB (12206350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34b79c34db62d930595a8e2ace08618b1cd00ef6712ddb8af07ac210aed76ff`  
		Last Modified: Sat, 08 Oct 2022 06:09:20 GMT  
		Size: 424.9 KB (424912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a195f4628b5bdfd12efcfa37bc318c508f555bed4ef29188bb9aecd7ed0536`  
		Last Modified: Sat, 08 Oct 2022 06:09:20 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:e35196c16606b2be4784cb905fd3a7bcfa90f1a1be4a85d444c9b82e04c79fdf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96936796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6870a64e63b640ec0902c3c6207f16ef931c6ee731a04630baea4aefe479d875`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:07:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:07:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:07:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:08:14 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:08:14 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Wed, 26 Oct 2022 01:09:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Oct 2022 01:09:55 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Oct 2022 17:16:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 17:16:29 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 17:16:29 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 17:16:29 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 17:16:30 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:16:30 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:22:03 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Oct 2022 17:22:03 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Oct 2022 17:22:03 GMT
ENV TOMCAT_VERSION=9.0.68
# Wed, 26 Oct 2022 17:22:03 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Wed, 26 Oct 2022 17:22:03 GMT
COPY dir:57bcd30f2d5bb685fa25c8ae07a942fe66802fd1f6cc85e584d2f1436f09a9f6 in /usr/local/tomcat 
# Wed, 26 Oct 2022 17:22:06 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 17:22:07 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 17:22:07 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 17:22:07 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b9bffe95bbbebdbdfba5c69142aeb65478735d04064fd29982a5b9c980559e`  
		Last Modified: Wed, 26 Oct 2022 01:16:15 GMT  
		Size: 16.2 MB (16216007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6957aefb66d28abfffaa8b0316225c93ae248e51de41c6472d528a29af6525`  
		Last Modified: Wed, 26 Oct 2022 01:17:16 GMT  
		Size: 40.8 MB (40803724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8abb56da477fa4a069dad39242e6d6999b85b514c78dc09595ac485605f1270`  
		Last Modified: Wed, 26 Oct 2022 01:17:12 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abed071b46cae4add2f87cc1f742710455da8d3452100d0f5ff92adce473f82`  
		Last Modified: Wed, 26 Oct 2022 17:39:58 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afa2b330b91f165250ca258e0a9aa6a545c6319d44de677623e1306aa38f922`  
		Last Modified: Wed, 26 Oct 2022 17:45:18 GMT  
		Size: 12.3 MB (12271316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eef5e48b4b4cc5b7d0fcf5821b53e35666420b68d5532929c8cd8d74bdbe1f6`  
		Last Modified: Wed, 26 Oct 2022 17:45:17 GMT  
		Size: 449.3 KB (449290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03e80168d84a3a97aecfc45503a641dec46b97187fd48d635fe8c7a3539ae5e`  
		Last Modified: Wed, 26 Oct 2022 17:45:17 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:09cc4f010caec08559093e89ba247b35ce68da5ff69d75c625828df50d34251d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104859306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f36e89d8cf58cf537bd1f5cc8fc1a4e967a50d107a4e7a499f29d6cd2ac415`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 13:45:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 13:45:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 13:45:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 13:46:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 13:46:33 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Tue, 25 Oct 2022 13:48:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 25 Oct 2022 13:48:30 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Oct 2022 02:10:31 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 02:10:32 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 02:10:33 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 02:10:33 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 02:10:34 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 02:10:34 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 02:20:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Oct 2022 02:20:12 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Oct 2022 02:20:13 GMT
ENV TOMCAT_VERSION=9.0.68
# Wed, 26 Oct 2022 02:20:13 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Wed, 26 Oct 2022 02:20:14 GMT
COPY dir:e164470f530d181b69a3c73aff03c2d6b926b59f1d4ebd7cca91ef9b53365be3 in /usr/local/tomcat 
# Wed, 26 Oct 2022 02:20:22 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:20:25 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 02:20:25 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 02:20:26 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5379e7ddac04281da9373ff24df0f186311a53e8595b3802f49472833a303c`  
		Last Modified: Tue, 25 Oct 2022 13:58:28 GMT  
		Size: 17.6 MB (17591474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dfa70173e738375ca5e76d051fb44a983159bc4d9d7c5f8e9b70c2f637e747`  
		Last Modified: Tue, 25 Oct 2022 13:59:36 GMT  
		Size: 41.2 MB (41195297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5cc3cd169e42df56848b903c511721c7f9492a6563b4b026f21ca9af764439`  
		Last Modified: Tue, 25 Oct 2022 13:59:28 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b4bb35bdcca497bc2f19fbd7ee1ab154232858e7c3dba47b0a7132a3c125ff`  
		Last Modified: Wed, 26 Oct 2022 02:46:44 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d34d14eefa8cea8aef04e420f19ca224c164451ab9f07126f114e0a30d47696`  
		Last Modified: Wed, 26 Oct 2022 02:52:37 GMT  
		Size: 12.3 MB (12297539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62553f1add797aed91c344d96451253082ccece127a5e795b659029790e7650`  
		Last Modified: Wed, 26 Oct 2022 02:52:35 GMT  
		Size: 474.0 KB (473992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d3939c0eb7340fd2150ce89e97e30f1b99f6f06e707d3a70a49fc38bfe1f`  
		Last Modified: Wed, 26 Oct 2022 02:52:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
