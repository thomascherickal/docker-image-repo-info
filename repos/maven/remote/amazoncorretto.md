## `maven:amazoncorretto`

```console
$ docker pull maven@sha256:c992f57c1ecea64c16f9095f9516486fd9978f7eb5a8d73adf3f5e29f34121e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:5c04ac2a8f7da5d5b63a3a2fa8c491a12c2b4d89f3cd278673b80e3ac4335608
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.8 MB (221817860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34fff39b532f2359ab4123923fbf2e05c2bcc39382659ca7e3cfb92ed44986bf`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 12 Jan 2022 02:20:04 GMT
ADD file:618cac8c5b6f6ff56ce221df12002d34997bcc996a0af3200b58db07d68be275 in / 
# Wed, 12 Jan 2022 02:20:04 GMT
CMD ["/bin/bash"]
# Wed, 19 Jan 2022 22:03:05 GMT
ARG version=11.0.14.9-1
# Wed, 19 Jan 2022 22:03:27 GMT
# ARGS: version=11.0.14.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 19 Jan 2022 22:03:28 GMT
ENV LANG=C.UTF-8
# Wed, 19 Jan 2022 22:03:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 20 Jan 2022 00:30:55 GMT
ARG MAVEN_VERSION=3.8.4
# Thu, 20 Jan 2022 00:30:55 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Jan 2022 00:30:55 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Thu, 20 Jan 2022 00:30:55 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Thu, 20 Jan 2022 00:31:07 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 20 Jan 2022 00:31:10 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 20 Jan 2022 00:31:10 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Jan 2022 00:31:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Jan 2022 00:31:11 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 20 Jan 2022 00:31:11 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 20 Jan 2022 00:31:11 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Jan 2022 00:31:11 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3a461b3ae562f8b6cf015b4c480a21b630a874f7fec851457680159226c81632`  
		Last Modified: Mon, 10 Jan 2022 23:29:44 GMT  
		Size: 62.2 MB (62212074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18e9b697db63eef866b1b6b7a1d0c9f2c2807b310992643fcd3d974ce17258c`  
		Last Modified: Wed, 19 Jan 2022 22:10:48 GMT  
		Size: 146.9 MB (146874196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfe3e4dc85f6941420b79a134572a99e60712f715dd3987d6545514df79c522`  
		Last Modified: Thu, 20 Jan 2022 00:35:29 GMT  
		Size: 3.6 MB (3620587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a9eb42e38e02d48f5e37b3262da4c5531bdd71c1bc49bfaa9f55461e8bbbe0`  
		Last Modified: Thu, 20 Jan 2022 00:35:29 GMT  
		Size: 9.1 MB (9109790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f46ca3505296ab7a9600a3bd2a89c8fb2e22f52e69ea0e78bbdfbbb03fda24`  
		Last Modified: Thu, 20 Jan 2022 00:35:28 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4eb03e7426bc164654788b48d17e67a184a06a635c243bc7af0b73c55e50d4`  
		Last Modified: Thu, 20 Jan 2022 00:35:28 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:e868ac2cad342fefcb6f10b9446351113c14fcb0e1da6bf1e31f49ccb9d17089
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.6 MB (220640353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189c827b517bb83501d2ae769198400c0a54d4ecf30240b0035fd7731078a99e`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 12 Jan 2022 02:39:41 GMT
ADD file:afc90ca87d61fdaef5c9d192a5151ab745ac8b8ea4d7544c2dfdd66bdb3b7993 in / 
# Wed, 12 Jan 2022 02:39:43 GMT
CMD ["/bin/bash"]
# Wed, 19 Jan 2022 22:29:54 GMT
ARG version=11.0.14.9-1
# Wed, 19 Jan 2022 22:30:14 GMT
# ARGS: version=11.0.14.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 19 Jan 2022 22:30:15 GMT
ENV LANG=C.UTF-8
# Wed, 19 Jan 2022 22:30:16 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Wed, 19 Jan 2022 23:17:36 GMT
ARG MAVEN_VERSION=3.8.4
# Wed, 19 Jan 2022 23:17:37 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Jan 2022 23:17:38 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Wed, 19 Jan 2022 23:17:39 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Wed, 19 Jan 2022 23:17:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 19 Jan 2022 23:17:55 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Jan 2022 23:17:56 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Jan 2022 23:17:57 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Jan 2022 23:17:59 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Jan 2022 23:18:00 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 19 Jan 2022 23:18:00 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Jan 2022 23:18:01 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:b2e274b2b0f90c3d6329566163244a0f2e6d97e4c010c62133388ac89652105f`  
		Last Modified: Wed, 12 Jan 2022 02:41:56 GMT  
		Size: 63.8 MB (63836908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c27b0182ad3bdf283f8d2b977e58b3122d366f07c0350d3efd711f8ef3601be`  
		Last Modified: Wed, 19 Jan 2022 22:32:09 GMT  
		Size: 144.1 MB (144072309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308a2926677c7f19fa7b5c4753eac56b3821aae5294ce0d9044317e2d59147a3`  
		Last Modified: Wed, 19 Jan 2022 23:22:51 GMT  
		Size: 3.6 MB (3620140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbac0ac649a00185b4fc94292f0d0c2b84a3f86b2f75b17cdb407161930311ce`  
		Last Modified: Wed, 19 Jan 2022 23:22:52 GMT  
		Size: 9.1 MB (9109783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea394bd65fd7c2eac9e4182ff8c3adfcb11d45313692d0515f288b547f2325d`  
		Last Modified: Wed, 19 Jan 2022 23:22:50 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9e4ecdcda839909000f9dbd8355d9e350efc57f98c8ecb47eadd33ae21ae88`  
		Last Modified: Wed, 19 Jan 2022 23:22:50 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
