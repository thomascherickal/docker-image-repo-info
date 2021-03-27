## `maven:3-ibmjava`

```console
$ docker pull maven@sha256:2e8d593bc4b8174f4d4a1c747bccc5a0a3837365257368b6aa0eec53c2552982
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:6ca06c798f75337b2ac016689efd019330367f28a62bce58dabafc5c54318b26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.3 MB (236311214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad8f5e6bed8748d2cd78f41c2cac72a479bad1a8f884858b9b35e3f4de4948a6`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:30:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:31:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:31:04 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:34:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='c51b7afed4911a4eefdf02c44ee440de726a5a605c5507cc50d4795394b418c2';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dfe87d34c40cd0c23dc4b7ee47c85f84e26d21ff75476b234998bb9132379659';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='bbc55934ec867290cd9307422beae48e5032dfabb7cb496bed6e47b7ab3f90be';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ed2722f283a3f3eb0a71f23354b0b4d2761865e759a3bf7f89297e17c20e6f';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c2ddf185daafacd0b50f3e4e593d613b2e9b70d66b88a8da6ee313181376aef6';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:34:34 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 18:59:51 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 26 Mar 2021 18:59:51 GMT
ARG USER_HOME_DIR=/root
# Fri, 26 Mar 2021 18:59:51 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 26 Mar 2021 18:59:52 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 26 Mar 2021 19:00:22 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 26 Mar 2021 19:00:22 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 26 Mar 2021 19:00:22 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 26 Mar 2021 19:00:23 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 26 Mar 2021 19:00:23 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 26 Mar 2021 19:00:23 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 26 Mar 2021 19:00:23 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4764ed71d2900c9874838108e377eb8821088502d5504fadeb080e5dd1a3e65d`  
		Last Modified: Fri, 26 Mar 2021 09:35:47 GMT  
		Size: 3.0 MB (2958415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86949eeef16a3389800d71fc509c42bf38f63c03fc1a49fffbc6dbedd587391`  
		Last Modified: Fri, 26 Mar 2021 09:37:24 GMT  
		Size: 168.0 MB (168001680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9721e0329ab14ceaa26804c63d6f3514324d0452cabfbc5b7c2e0cb8e7470a1`  
		Last Modified: Fri, 26 Mar 2021 19:07:07 GMT  
		Size: 38.6 MB (38638089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85818b5e8a7e711d07943f0ac2c8189dd1805076d29a745413b92f2c8c8f819b`  
		Last Modified: Fri, 26 Mar 2021 19:07:03 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f353b568c8be7dc131661aed6f85830d73b20597a4408fa1fd7ec7db5090d1d`  
		Last Modified: Fri, 26 Mar 2021 19:07:03 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; 386

```console
$ docker pull maven@sha256:c7574f1c24db77e686caf22931770850bdb6d493739ccf4577c2b3a93fe3fae5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.2 MB (223187745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ce6b6966d088c6367a7f7042552878b72b54b5603809f21f07674bdd5e1d399`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 25 Mar 2021 22:56:34 GMT
ADD file:bf6540bf2a58280c4a1ca750923f197a94e87ea60d68ee682aa7b8443bf9d3ac in / 
# Thu, 25 Mar 2021 22:56:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:56:39 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:56:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:56:41 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:29:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 12:30:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:30:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 12:32:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='c51b7afed4911a4eefdf02c44ee440de726a5a605c5507cc50d4795394b418c2';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dfe87d34c40cd0c23dc4b7ee47c85f84e26d21ff75476b234998bb9132379659';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='bbc55934ec867290cd9307422beae48e5032dfabb7cb496bed6e47b7ab3f90be';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ed2722f283a3f3eb0a71f23354b0b4d2761865e759a3bf7f89297e17c20e6f';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c2ddf185daafacd0b50f3e4e593d613b2e9b70d66b88a8da6ee313181376aef6';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 12:32:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 14:53:07 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 26 Mar 2021 14:53:07 GMT
ARG USER_HOME_DIR=/root
# Fri, 26 Mar 2021 14:53:08 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 26 Mar 2021 14:53:08 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 26 Mar 2021 14:53:49 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 26 Mar 2021 14:53:49 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 26 Mar 2021 14:53:50 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 26 Mar 2021 14:53:50 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 26 Mar 2021 14:53:50 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 26 Mar 2021 14:53:50 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 26 Mar 2021 14:53:51 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:2f0eb5f15f485a536d788bddd145b48525637bfc6c2a34803b34babd20b5ce0b`  
		Last Modified: Thu, 25 Mar 2021 22:58:12 GMT  
		Size: 27.1 MB (27138250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74666259d3def5d951f6a67a56022c1b10a46a265872c781b51e31eb14bf6006`  
		Last Modified: Thu, 25 Mar 2021 22:58:06 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf32f44a20f56ba75e3142f14f780ea37d9cc6f3e84321468895f72c6cc38c0`  
		Last Modified: Thu, 25 Mar 2021 22:58:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f41518e71c9104d8d50be2b4d3ce4968be99db988a1310d973af5b750c1d9e`  
		Last Modified: Fri, 26 Mar 2021 12:32:38 GMT  
		Size: 3.0 MB (2988377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbdebe6571a9bc07d586dade363092984b8fa5cb5e8308938dfbf0bd262cb11`  
		Last Modified: Fri, 26 Mar 2021 12:33:46 GMT  
		Size: 156.2 MB (156172173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58f39a84992e3152a3ae3d2f6c53a342c5872f104825e8ae8961bd3b063f166`  
		Last Modified: Fri, 26 Mar 2021 14:54:23 GMT  
		Size: 36.9 MB (36886695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b417127fb584559b21a997ea2cb671de0ff8018a86b35a7a166360183e307`  
		Last Modified: Fri, 26 Mar 2021 14:54:18 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8423f3e12f11d84510f86b164042ffd82330b369d325c3e22400dfc84984290b`  
		Last Modified: Fri, 26 Mar 2021 14:54:18 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:1c37b6a7abebd1064eb339e2b8cbd33a898e083e6c2a9145a19638a1598f96bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.5 MB (235536182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a18963fe6f19c293b2f37dbee30834288c02a66cbc0dc43dd13511b2ca0dfb48`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 06:05:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 04 Mar 2021 06:06:37 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Mar 2021 21:37:28 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Thu, 11 Mar 2021 21:41:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='c51b7afed4911a4eefdf02c44ee440de726a5a605c5507cc50d4795394b418c2';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dfe87d34c40cd0c23dc4b7ee47c85f84e26d21ff75476b234998bb9132379659';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='bbc55934ec867290cd9307422beae48e5032dfabb7cb496bed6e47b7ab3f90be';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ed2722f283a3f3eb0a71f23354b0b4d2761865e759a3bf7f89297e17c20e6f';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c2ddf185daafacd0b50f3e4e593d613b2e9b70d66b88a8da6ee313181376aef6';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 11 Mar 2021 21:41:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 11 Mar 2021 23:25:32 GMT
ARG MAVEN_VERSION=3.6.3
# Thu, 11 Mar 2021 23:25:41 GMT
ARG USER_HOME_DIR=/root
# Thu, 11 Mar 2021 23:25:53 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Thu, 11 Mar 2021 23:26:00 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Thu, 11 Mar 2021 23:28:25 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 11 Mar 2021 23:28:32 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 11 Mar 2021 23:28:37 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 11 Mar 2021 23:28:39 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 11 Mar 2021 23:28:42 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 11 Mar 2021 23:28:46 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 11 Mar 2021 23:28:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59980a4d9c242412ef5a5dfbafd355a75407f666e0da0f08f867f5bba04d0a5f`  
		Last Modified: Thu, 04 Mar 2021 06:12:04 GMT  
		Size: 3.1 MB (3082310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58521849eebddc10c568855d811d4386a5b2bc6d70b49b06e011758dae285e20`  
		Last Modified: Thu, 11 Mar 2021 21:43:21 GMT  
		Size: 167.7 MB (167715153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dabf1a12cdaccd053ebbe55ad646fd4146e44eee0c2a2d914a116df1f049b24`  
		Last Modified: Thu, 11 Mar 2021 23:29:57 GMT  
		Size: 34.3 MB (34315352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcef91c5daf616fd557b685dbbcc73c56629230f272bb007c530d81d77c1f909`  
		Last Modified: Thu, 11 Mar 2021 23:29:51 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91c0d9dfa333ef28182acb3dd146ac1996428b64f777599500b876a11ecbd5`  
		Last Modified: Thu, 11 Mar 2021 23:29:51 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:b980f20ededec02887e36a05065e22adbb4ff8336821a92a7f4b4d8057303db6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.8 MB (218783670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b6f199b4df98211c8299950676d7d01c0342844cd65a529a89c02ffbd07358`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:31 GMT
ADD file:1c7dbc64158234b813a2eeff0c325efa0cff7c3983e93fc9f7de0004e901c2c1 in / 
# Thu, 25 Mar 2021 22:53:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:35 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:14:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 26 Mar 2021 09:14:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:14:24 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Fri, 26 Mar 2021 09:17:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='c51b7afed4911a4eefdf02c44ee440de726a5a605c5507cc50d4795394b418c2';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='dfe87d34c40cd0c23dc4b7ee47c85f84e26d21ff75476b234998bb9132379659';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='bbc55934ec867290cd9307422beae48e5032dfabb7cb496bed6e47b7ab3f90be';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ed2722f283a3f3eb0a71f23354b0b4d2761865e759a3bf7f89297e17c20e6f';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='c2ddf185daafacd0b50f3e4e593d613b2e9b70d66b88a8da6ee313181376aef6';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Mar 2021 09:17:18 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 26 Mar 2021 14:28:10 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 26 Mar 2021 14:28:11 GMT
ARG USER_HOME_DIR=/root
# Fri, 26 Mar 2021 14:28:11 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 26 Mar 2021 14:28:11 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 26 Mar 2021 14:28:34 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 26 Mar 2021 14:28:37 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 26 Mar 2021 14:28:37 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 26 Mar 2021 14:28:37 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 26 Mar 2021 14:28:38 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 26 Mar 2021 14:28:39 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 26 Mar 2021 14:28:39 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:bf8da0ed3f9ec60019cec9fac782f04b7281f232a86e7613579e54c348b8402b`  
		Last Modified: Thu, 25 Mar 2021 22:54:27 GMT  
		Size: 25.4 MB (25381419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de72c87d1d7a4355d21e04b9ce611f427f0c84ee6705dd53a1fd990012cefdd6`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffe2f5d8eac8afe4b79981c9c93b44c985dbb7b3bb5f9af5e918c6aac415fcf`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f5a2b948c3809ff99d8a7efdcd231a3399837ea439f2360e25328330eea026`  
		Last Modified: Fri, 26 Mar 2021 09:17:43 GMT  
		Size: 2.7 MB (2676671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d762f85c24bab568e74bfce8af30c760a7d5c3694505f56a9bdac64ddc1fc236`  
		Last Modified: Fri, 26 Mar 2021 09:18:24 GMT  
		Size: 158.3 MB (158331939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c68804a3b933136b6508ee60acf19b661b0a9cd44e367d2c2a1474de467ce12`  
		Last Modified: Fri, 26 Mar 2021 14:31:21 GMT  
		Size: 32.4 MB (32391393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f28503fa73d709286ddc50bb3d466d039e367d8fe82476d179d6824de4c162c`  
		Last Modified: Fri, 26 Mar 2021 14:31:18 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c258eaf26c1b446644c0094062c1dd6c8f70099839a20249d2da84dedbd72a`  
		Last Modified: Fri, 26 Mar 2021 14:31:20 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
