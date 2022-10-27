## `tomcat:8-jre8-temurin`

```console
$ docker pull tomcat@sha256:0ec67c4a896d298dc86f6966ecf8b3009e96b3e49b7c8cba79d8583a4f45f859
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:8-jre8-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:c141a6ba8cfd1d96372a9e63691c10ffd7f6ef01ab45ce56ba13c22049b15b76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.3 MB (96344363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:830650ee158eecb55e0974c3d8449f7ee7fc4159d20bfc9bbbee900f5a903dd1`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:41 GMT
ADD file:ba96f963bbfd429a0839c40603fdd7829eaca58f20adfa0d15e6beae8244bc08 in / 
# Tue, 25 Oct 2022 01:53:41 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:27:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 17:27:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 17:27:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 17:28:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 17:28:11 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Tue, 25 Oct 2022 17:28:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 25 Oct 2022 17:28:38 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Oct 2022 23:48:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 23:48:52 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 23:48:53 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 23:48:53 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 23:48:53 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 23:48:53 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 23:59:12 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 26 Oct 2022 23:59:12 GMT
ENV TOMCAT_MAJOR=8
# Wed, 26 Oct 2022 23:59:12 GMT
ENV TOMCAT_VERSION=8.5.83
# Wed, 26 Oct 2022 23:59:12 GMT
ENV TOMCAT_SHA512=57cbe9608a9c4e88135e5f5480812e8d57690d5f3f6c43a7c05fe647bddb7c3b684bf0fc0efebad399d05e80c6d20c43d5ecdf38ec58f123e6653e443f9054e3
# Wed, 26 Oct 2022 23:59:12 GMT
COPY dir:2e0b50df25e60798dfd28c553cda21eb89f7eb6f8d2e826a24ff72f18344d5c5 in /usr/local/tomcat 
# Wed, 26 Oct 2022 23:59:18 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 23:59:19 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 23:59:19 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 23:59:19 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:301a8b74f71f85f3a31e9c7e7fedd5b001ead5bcf895bc2911c1d260e06bd987`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 30.4 MB (30426374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4688df200b56af3e7b12bd48807e851b1a3717379161a295d43dd3184abec55e`  
		Last Modified: Wed, 26 Oct 2022 16:43:13 GMT  
		Size: 12.4 MB (12442357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317eff501ed473c93069a282f9127b5ff4a4e221fe04b6660657f1a0c2207046`  
		Last Modified: Wed, 26 Oct 2022 16:43:54 GMT  
		Size: 41.8 MB (41807983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7a126acf9d6891d01e855a78476143052dcbc8c6963ec50941506634fb38de`  
		Last Modified: Wed, 26 Oct 2022 16:43:48 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b5a22f69ed01e1a509192f067bbe5c0e91e6a4c387acaac6e5702b08201f41`  
		Last Modified: Thu, 27 Oct 2022 00:09:37 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300daff9a0eb951fac2db11c6d771787c991f8bcb65d3b5d15b0c56eeb654bf9`  
		Last Modified: Thu, 27 Oct 2022 00:18:42 GMT  
		Size: 11.2 MB (11214564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b470d40b74b297744e04fec69e05b684832f6bd4318d18d6eba8d0351564cc8`  
		Last Modified: Thu, 27 Oct 2022 00:18:41 GMT  
		Size: 452.6 KB (452620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcaac9741121a3dd778cdcd04ceee7b60cbf395d71acf6e57f9e0c20c33d04`  
		Last Modified: Thu, 27 Oct 2022 00:18:40 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:db01c78c66eea555b3033816954e3d0991270de8a7a034bcf1d4eeb483b96ba1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90146630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682dc934b8d583bedd27aedbe993eeb09ad0f01bdc11e394af5ebb071e17773d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:30:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 06 Oct 2022 06:30:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 06:30:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 06 Oct 2022 06:30:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:30:53 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 06 Oct 2022 06:31:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 06 Oct 2022 06:31:41 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 07 Oct 2022 06:16:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 07 Oct 2022 06:16:05 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 06:16:06 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 07 Oct 2022 06:16:06 GMT
WORKDIR /usr/local/tomcat
# Fri, 07 Oct 2022 06:16:06 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 07 Oct 2022 06:16:06 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 07 Oct 2022 06:34:28 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 07 Oct 2022 06:34:28 GMT
ENV TOMCAT_MAJOR=8
# Wed, 12 Oct 2022 00:48:41 GMT
ENV TOMCAT_VERSION=8.5.83
# Wed, 12 Oct 2022 00:48:41 GMT
ENV TOMCAT_SHA512=57cbe9608a9c4e88135e5f5480812e8d57690d5f3f6c43a7c05fe647bddb7c3b684bf0fc0efebad399d05e80c6d20c43d5ecdf38ec58f123e6653e443f9054e3
# Wed, 12 Oct 2022 00:48:42 GMT
COPY dir:6939dfc512ae5c458803d9bd0c62e2960ece6a0a8b00da054d60c62450b3d39d in /usr/local/tomcat 
# Wed, 12 Oct 2022 00:48:50 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Oct 2022 00:48:50 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 12 Oct 2022 00:48:51 GMT
EXPOSE 8080
# Wed, 12 Oct 2022 00:48:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719b6638b27c56e64e5456f9e5ccd262ec6c6ed045d97ce1df9a938b8e0e1822`  
		Last Modified: Thu, 06 Oct 2022 06:39:41 GMT  
		Size: 12.0 MB (12015320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bcda6c674cf03ff9f8915f8884924bab5b0c377076d840172756691f21fca7`  
		Last Modified: Thu, 06 Oct 2022 06:40:25 GMT  
		Size: 39.5 MB (39537226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfba53c42866b1ad1ead1b76a3b9d6961ab0b030e5cd4f6bd1600e5a4775a5c9`  
		Last Modified: Thu, 06 Oct 2022 06:40:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06e65cd00c33655d2a36085b5eacee0922f1b222e3b06292bf9decbfe22bbba`  
		Last Modified: Fri, 07 Oct 2022 06:53:57 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a832b51a078dfdccd0fc7d94342f1b761c90d9bb36cad48f581d00b5020c840`  
		Last Modified: Wed, 12 Oct 2022 01:09:31 GMT  
		Size: 11.1 MB (11148723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ff8b35227219d77cc65999bdb44babcf584e6eb90bba8633c8f9a35a5fee72`  
		Last Modified: Wed, 12 Oct 2022 01:09:30 GMT  
		Size: 426.3 KB (426266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa7199ff4b9b53c1f1326f5e8f695692466ee7db20554048c09f0afd7c19e3f`  
		Last Modified: Wed, 12 Oct 2022 01:09:29 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:6827d06d478c67039fa1bbbf68f361a0697af20bfed7e6254175c95365e0c236
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93260891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4707dee8958c418d9038a2bbdab77187618630de6aba6e223f7bf4ae20a1726d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:08:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:08:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:08:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:09:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:09:02 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Wed, 26 Oct 2022 01:10:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Oct 2022 01:10:01 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Oct 2022 17:15:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 17:15:52 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 17:15:52 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 17:15:52 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 17:15:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:15:53 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:27:24 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 26 Oct 2022 17:27:24 GMT
ENV TOMCAT_MAJOR=8
# Wed, 26 Oct 2022 17:27:24 GMT
ENV TOMCAT_VERSION=8.5.83
# Wed, 26 Oct 2022 17:27:24 GMT
ENV TOMCAT_SHA512=57cbe9608a9c4e88135e5f5480812e8d57690d5f3f6c43a7c05fe647bddb7c3b684bf0fc0efebad399d05e80c6d20c43d5ecdf38ec58f123e6653e443f9054e3
# Wed, 26 Oct 2022 17:27:24 GMT
COPY dir:83a980a9d9dc012cf889e835417f92fdc382a77964d084a60afae6fccbf4daf2 in /usr/local/tomcat 
# Wed, 26 Oct 2022 17:27:27 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 17:27:28 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 17:27:28 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 17:27:28 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d33b973dbba18a894c3b9064cedfece84e92985bce6e3be86a5efef3afdea8`  
		Last Modified: Wed, 26 Oct 2022 01:16:34 GMT  
		Size: 12.4 MB (12400371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f697897ed2257dda5be8508f0a03cad8141fa496a3e37b2a994fd61309cf99c`  
		Last Modified: Wed, 26 Oct 2022 01:17:30 GMT  
		Size: 40.8 MB (40803056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d8712637d762132e09b6a1a7126c20f5b102f422e01c1071728a35488e2b8`  
		Last Modified: Wed, 26 Oct 2022 01:17:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bc24cf4838a92ddf07c37dc5adc53eadeefa127d372dd41f9313fecce01930`  
		Last Modified: Wed, 26 Oct 2022 17:39:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c774047e3ccf38117111513f39e81c149d56f6f3389b81922b0dcdca0c5d7f3c`  
		Last Modified: Wed, 26 Oct 2022 17:49:59 GMT  
		Size: 11.2 MB (11222527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709962c5d01aae6d25d58e0bce4a929c341c4fd8b8c195bc671b7647442200d5`  
		Last Modified: Wed, 26 Oct 2022 17:49:58 GMT  
		Size: 452.0 KB (451983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2005acb6441b0e9a679ac2b7380673257747f81172e6f1ab44ec203ad044499c`  
		Last Modified: Wed, 26 Oct 2022 17:49:58 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:71e08492da036a65b9facc02eb5a13500aeaf96fb1cfafd73355e435d964fe42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101898146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efdb22c3fd8b9f58ba6975c3beae12abcf5ad5043e959838b0073a1d472b303a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 13:47:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 13:47:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 13:47:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 13:47:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 13:47:49 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Tue, 25 Oct 2022 13:48:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='65b8bd74382d6514d2458ff4375468651791a55a186a5bffe0803204801e9c94';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='a9dd1ea4280a85158191101688bbf1920c4676a3849e22dc7783fb61f60d6199';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='0e58c3fb39303969d7d6ff660c0b63997ab0ee68af3452f3d17f2892c61a58f6';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='2422a8831fe414b9dba4c443ee3562431dfcde27577124f0db58ec903afc262a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 25 Oct 2022 13:48:45 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Oct 2022 02:08:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 02:08:55 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 02:08:56 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 02:08:57 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 02:08:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 02:08:57 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 02:28:37 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 26 Oct 2022 02:28:38 GMT
ENV TOMCAT_MAJOR=8
# Wed, 26 Oct 2022 02:28:38 GMT
ENV TOMCAT_VERSION=8.5.83
# Wed, 26 Oct 2022 02:28:38 GMT
ENV TOMCAT_SHA512=57cbe9608a9c4e88135e5f5480812e8d57690d5f3f6c43a7c05fe647bddb7c3b684bf0fc0efebad399d05e80c6d20c43d5ecdf38ec58f123e6653e443f9054e3
# Wed, 26 Oct 2022 02:28:39 GMT
COPY dir:e50c318b4e7429c679ab95018cba8bf6498e2b0378cfbddf1450397b3fee216e in /usr/local/tomcat 
# Wed, 26 Oct 2022 02:28:47 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 02:28:50 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 02:28:50 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 02:28:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222b03548b709077a95a1d389c380123c26cac903f8c75f9ad589c4adad13fe9`  
		Last Modified: Tue, 25 Oct 2022 13:58:58 GMT  
		Size: 13.3 MB (13266255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003723378379d113d8c11cee67cac1bd59fa29fa443ec3c7d5ccf54b97f92f4a`  
		Last Modified: Tue, 25 Oct 2022 13:59:56 GMT  
		Size: 41.2 MB (41194760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae24631925a085d4f9a23428fac40b4b8c891271506de3a6bd9e20aaa84e77b`  
		Last Modified: Tue, 25 Oct 2022 13:59:47 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a1c51f5d24a88ba0514d43cd722418b351566b733499467ff6969ed0c4376b`  
		Last Modified: Wed, 26 Oct 2022 02:46:01 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1995efba3eddd54af9fb391d18a907deba9c2b9aa502bfa5dbf0bf2e8227cfbd`  
		Last Modified: Wed, 26 Oct 2022 02:57:32 GMT  
		Size: 11.2 MB (11243313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a202f51e2099ef340d544254629ad83f604ccd1797a4d34d782b11ab164c8616`  
		Last Modified: Wed, 26 Oct 2022 02:57:31 GMT  
		Size: 484.0 KB (483953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb45ce2dd0b2e708b2cffad416e712393ba678932d97fafa2e7113d7d1ec627`  
		Last Modified: Wed, 26 Oct 2022 02:57:31 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
