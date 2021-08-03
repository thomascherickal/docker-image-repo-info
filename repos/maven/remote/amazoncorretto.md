## `maven:amazoncorretto`

```console
$ docker pull maven@sha256:b3fe7ba453ddb8c9b3e50611bfb799814513209584a681ff0df4e2ae09cda4a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:4132f41dd9494a7f17e3410f0336b102e972b42b1e0401994ded788e3ef0e615
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221929542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a1f041e38017164db4701941c7a844e3a16857c81ee37b884bae782cf84869`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
# Tue, 03 Aug 2021 00:04:41 GMT
ARG version=11.0.12.7-1
# Tue, 03 Aug 2021 00:05:03 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 03 Aug 2021 00:05:03 GMT
ENV LANG=C.UTF-8
# Tue, 03 Aug 2021 00:05:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 03 Aug 2021 00:41:12 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 03 Aug 2021 00:41:12 GMT
ARG USER_HOME_DIR=/root
# Tue, 03 Aug 2021 00:41:13 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 03 Aug 2021 00:41:13 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 03 Aug 2021 00:41:22 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Tue, 03 Aug 2021 00:41:24 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 03 Aug 2021 00:41:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 03 Aug 2021 00:41:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 03 Aug 2021 00:41:25 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 03 Aug 2021 00:41:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 03 Aug 2021 00:41:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 03 Aug 2021 00:41:26 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f170fe744cfdd69b498f626d42da3fa5b31e4e88b3c49ee2ea881f4025eee5ad`  
		Last Modified: Tue, 03 Aug 2021 00:06:55 GMT  
		Size: 146.8 MB (146777358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dc87548866e7220c42566e014a0283e31debc26883c0a63d07393b618ace53`  
		Last Modified: Tue, 03 Aug 2021 00:45:43 GMT  
		Size: 3.6 MB (3574338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fefb9363f5ab8fdfe3ecac311026965191ba2e0466d9c81e164e6ef0338f88c`  
		Last Modified: Tue, 03 Aug 2021 00:45:43 GMT  
		Size: 9.6 MB (9610957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8a7b2b4d533683310a20fe7ad9dc5f50089edc66db3518e2decf4bc8a1b85d`  
		Last Modified: Tue, 03 Aug 2021 00:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c96809ba28028b4f63b7b31204619a745d3c2b86d4908b8e6e028f42138753`  
		Last Modified: Tue, 03 Aug 2021 00:45:42 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:1a85fa09713f71032cece33160b9096e057a5c935ebb3d3e35d45c96832149a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220685555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b3dd8770b263ad49ec52f86b78cb86404ab89dd102681693abd6224ecaf1ca`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Aug 2021 00:07:57 GMT
ARG version=11.0.12.7-1
# Tue, 03 Aug 2021 00:08:15 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 03 Aug 2021 00:08:16 GMT
ENV LANG=C.UTF-8
# Tue, 03 Aug 2021 00:08:16 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 03 Aug 2021 00:28:33 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 03 Aug 2021 00:28:33 GMT
ARG USER_HOME_DIR=/root
# Tue, 03 Aug 2021 00:28:33 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 03 Aug 2021 00:28:33 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 03 Aug 2021 00:28:41 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Tue, 03 Aug 2021 00:28:47 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 03 Aug 2021 00:28:47 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 03 Aug 2021 00:28:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 03 Aug 2021 00:28:47 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 03 Aug 2021 00:28:48 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 03 Aug 2021 00:28:48 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 03 Aug 2021 00:28:48 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8b16728471d5d9ac7f454dcd3043e891b79ff4ad587d6f92b86edd9b49b1e8`  
		Last Modified: Tue, 03 Aug 2021 00:10:12 GMT  
		Size: 143.9 MB (143933602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cfea09f3c7709adca72a2fff9fbc4ff50443a1567bf5a0e28f9676fc855d8e7`  
		Last Modified: Tue, 03 Aug 2021 00:33:21 GMT  
		Size: 3.6 MB (3592914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294a7d6cdfeaa2b81075bf325466f55c0a06e6baa65e45bbd3e6cbd68b913ae`  
		Last Modified: Tue, 03 Aug 2021 00:33:21 GMT  
		Size: 9.6 MB (9610972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b708fda45865e2fe264f017976efcd35c90197a1dbad54cadf0ea66426b08ad6`  
		Last Modified: Tue, 03 Aug 2021 00:33:20 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9d95099af1a72cdf6d130299d9105d8f392f76ffce09fdd7cbd0010486086b`  
		Last Modified: Tue, 03 Aug 2021 00:33:20 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
