## `maven:3-amazoncorretto-17`

```console
$ docker pull maven@sha256:b437aca8b97eee12217b45dde8f1d77ad4210c73c4ebb596b8f8fa839bd704ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17` - linux; amd64

```console
$ docker pull maven@sha256:0dd0f31546b397b99ea4db13455c27c8a38f1fc37dcb265646e940ee4d4470a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.3 MB (226302057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8e8b5e9465e5e4dfefba81bf8b3611245e7331cf0ce78285a2cb23d8d0d582`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Jun 2022 23:19:41 GMT
ADD file:e6c6bb016423b24a28b273cc76e9fbbf81934b77a0ede797ccfd0eeac465c8a4 in / 
# Tue, 21 Jun 2022 23:19:42 GMT
CMD ["/bin/bash"]
# Tue, 19 Jul 2022 22:38:35 GMT
ARG version=17.0.4.8-1
# Tue, 19 Jul 2022 22:38:58 GMT
# ARGS: version=17.0.4.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 19 Jul 2022 22:38:58 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:38:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Wed, 20 Jul 2022 04:32:41 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 20 Jul 2022 04:32:41 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 20 Jul 2022 04:32:41 GMT
ARG USER_HOME_DIR=/root
# Wed, 20 Jul 2022 04:32:41 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 20 Jul 2022 04:32:41 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 20 Jul 2022 04:32:43 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 20 Jul 2022 04:32:43 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 20 Jul 2022 04:32:43 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 20 Jul 2022 04:32:43 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 20 Jul 2022 04:32:44 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 20 Jul 2022 04:32:44 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 20 Jul 2022 04:32:44 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:017c82d6391f0bf122516eac436a6e8d77ac13282fdd13dde7e7e47dc71d447e`  
		Last Modified: Wed, 15 Jun 2022 22:09:36 GMT  
		Size: 62.3 MB (62294977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c297b4544f77e61a5ef202b51c7b35066efeb505d0980b8fb71af85f3a0cfb4`  
		Last Modified: Tue, 19 Jul 2022 22:46:36 GMT  
		Size: 151.6 MB (151642501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b47e45a470a975e57178c12faf1f4d6a1fb0a45d581e7471c33b3e175002d88`  
		Last Modified: Wed, 20 Jul 2022 04:35:26 GMT  
		Size: 3.6 MB (3623869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f17e4cee6290282fd1b3c229c4e9ca6dcdfd2b2e1db433104d4ab5efb224e0a`  
		Last Modified: Wed, 20 Jul 2022 04:35:26 GMT  
		Size: 8.7 MB (8739498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114ad61d2624871341f753cd1f18b8649584e748d883dff72f1950bc2526fed4`  
		Last Modified: Wed, 20 Jul 2022 04:35:26 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3234856ce11b1c066ee246322681b07f8ce551e7f17962c001ad3f552339da57`  
		Last Modified: Wed, 20 Jul 2022 04:35:26 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:f671e0def97375ddf7c2cc3fbe0c9e102a1fbb23554f2aacc5801b4e334a1e4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.5 MB (226452774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1457a0298133d05a86952c1325879827f10da20307ab6434b03a31d3c5f3a9`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
# Wed, 20 Jul 2022 06:01:29 GMT
ARG version=17.0.4.8-1
# Wed, 20 Jul 2022 06:01:46 GMT
# ARGS: version=17.0.4.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 20 Jul 2022 06:01:46 GMT
ENV LANG=C.UTF-8
# Wed, 20 Jul 2022 06:01:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Wed, 20 Jul 2022 07:42:21 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 20 Jul 2022 07:42:22 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 20 Jul 2022 07:42:23 GMT
ARG USER_HOME_DIR=/root
# Wed, 20 Jul 2022 07:42:24 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 20 Jul 2022 07:42:25 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 20 Jul 2022 07:42:28 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 20 Jul 2022 07:42:29 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 20 Jul 2022 07:42:30 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 20 Jul 2022 07:42:32 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 20 Jul 2022 07:42:33 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 20 Jul 2022 07:42:33 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 20 Jul 2022 07:42:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2aa980da9360b7040c08b4f8e530b7c0b74f78793771a0d340b39474533996`  
		Last Modified: Wed, 20 Jul 2022 06:04:20 GMT  
		Size: 150.2 MB (150153923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672703a2d3b07c94e631a5493c4870634a3b9e50ac9e4b62d6f7ce516254ecbf`  
		Last Modified: Wed, 20 Jul 2022 07:46:35 GMT  
		Size: 3.6 MB (3639525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e893f1a263434126cd3e963a6b66d35b6e29107bc8cbea4258a15eedb0def8`  
		Last Modified: Wed, 20 Jul 2022 07:46:35 GMT  
		Size: 8.7 MB (8739470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13b22ffe1c43593e9ce8f4848e72940f95a5a3ae5badd529498d9df855543b`  
		Last Modified: Wed, 20 Jul 2022 07:46:34 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570c1e87bbff807fb084edcf281e580f6913d4f812afd5c5c6773dba9927bd5e`  
		Last Modified: Wed, 20 Jul 2022 07:46:34 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
