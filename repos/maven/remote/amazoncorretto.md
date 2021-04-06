## `maven:amazoncorretto`

```console
$ docker pull maven@sha256:99a2d41491b3fdc0397555d6ecccfafbfb568b62aa4fbcf452ced82d44cf3504
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:926f220957e212031a0e8b607090062a66a4a8f37d7c0fbc7aeee2457460c0de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221637611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1f7729b72a6497beecedb16bd12c4af51bf97b441fdd096c4d384816e283af`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:20 GMT
ADD file:3b750ce7e7425c1cb02261d65b1e301d5818cda51a80dc8ab3b915ee5ca37d4e in / 
# Tue, 30 Mar 2021 21:59:21 GMT
CMD ["/bin/bash"]
# Wed, 31 Mar 2021 16:17:44 GMT
ARG version=11.0.10.9-1
# Wed, 31 Mar 2021 16:18:06 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 31 Mar 2021 16:18:07 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 16:18:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Mon, 05 Apr 2021 17:53:58 GMT
ARG MAVEN_VERSION=3.8.1
# Mon, 05 Apr 2021 17:53:59 GMT
ARG USER_HOME_DIR=/root
# Mon, 05 Apr 2021 17:53:59 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Mon, 05 Apr 2021 17:53:59 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Mon, 05 Apr 2021 17:54:13 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Mon, 05 Apr 2021 17:54:20 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 05 Apr 2021 17:54:20 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 05 Apr 2021 17:54:20 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 05 Apr 2021 17:54:20 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 05 Apr 2021 17:54:21 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 05 Apr 2021 17:54:21 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 05 Apr 2021 17:54:21 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:99a21848b482c10fd4b103b7ab95e1446142e76e3dfa673efd0a23fb264ec5e5`  
		Last Modified: Tue, 30 Mar 2021 13:54:37 GMT  
		Size: 61.9 MB (61946585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ff02117c57c37731db7de0f6f622c192c9a014a6e20799e8275c82fde8bdb5`  
		Last Modified: Wed, 31 Mar 2021 16:20:56 GMT  
		Size: 146.5 MB (146526785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43950373d874b7f08e1c85ce59f57d3ad6ac80da2285da3ef8e8ab595858fd4b`  
		Last Modified: Mon, 05 Apr 2021 18:05:07 GMT  
		Size: 3.6 MB (3552047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d206ed979abe98ee0b1370d44982730a72f423279908d0f2f490dcc82df934c3`  
		Last Modified: Mon, 05 Apr 2021 18:05:07 GMT  
		Size: 9.6 MB (9610979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ba0285f4de2df41af13949bb0f588c3d2dbc86a918b4a526fb7ed16e86a312`  
		Last Modified: Mon, 05 Apr 2021 18:05:05 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22081064179d1bb7062f587da721734b07d789b9d6f212d0cdf4ed7cb94a677`  
		Last Modified: Mon, 05 Apr 2021 18:05:06 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:7495234459eaf2130f892e366be5e0eee7c4dd1d283c90848480c8864662ecab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221454969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114dabab3dfcf81eea37abde050cad0f385e76d87d6cada38136d66c3f0c733d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 30 Mar 2021 21:59:58 GMT
ADD file:540e42c4903b87925bc490b00820f555e531041d1b1fcea6ee56f4cc3bbc895d in / 
# Tue, 30 Mar 2021 22:00:02 GMT
CMD ["/bin/bash"]
# Wed, 31 Mar 2021 14:31:51 GMT
ARG version=11.0.10.9-1
# Wed, 31 Mar 2021 14:32:23 GMT
# ARGS: version=11.0.10.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 31 Mar 2021 14:32:25 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 14:32:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Mon, 05 Apr 2021 17:50:33 GMT
ARG MAVEN_VERSION=3.8.1
# Mon, 05 Apr 2021 17:50:34 GMT
ARG USER_HOME_DIR=/root
# Mon, 05 Apr 2021 17:50:35 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Mon, 05 Apr 2021 17:50:36 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Mon, 05 Apr 2021 17:50:56 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Mon, 05 Apr 2021 17:51:00 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 05 Apr 2021 17:51:02 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 05 Apr 2021 17:51:03 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 05 Apr 2021 17:51:05 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 05 Apr 2021 17:51:06 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 05 Apr 2021 17:51:08 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 05 Apr 2021 17:51:09 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:7d8296f22a3c3f786ce15fb5be7dce44af09932e617f9a981183619985014031`  
		Last Modified: Tue, 30 Mar 2021 22:01:09 GMT  
		Size: 63.7 MB (63660038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95699b3b4c6148372044d77f04b93534536f2c698321e9f4811b142a9052825`  
		Last Modified: Wed, 31 Mar 2021 14:35:08 GMT  
		Size: 144.6 MB (144597607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6853b1f509aad397f2b0194a925397b7070ce599ef659720fbb536e429f27502`  
		Last Modified: Mon, 05 Apr 2021 17:57:48 GMT  
		Size: 3.6 MB (3585157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c88cef9804c3269b6cb549f272c3d2cdf9f97267745c58ffb5f131b37940195`  
		Last Modified: Mon, 05 Apr 2021 17:57:48 GMT  
		Size: 9.6 MB (9610955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67392b5a3670321588d8c9c36ee4f0a5ba7eea50c1d878dafdf72633ac76725`  
		Last Modified: Mon, 05 Apr 2021 17:57:47 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0d9ab13872c4dc513f907afef8b5e0d6b78abdfba90dc2f38d12dcebcadfc`  
		Last Modified: Mon, 05 Apr 2021 17:57:47 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
