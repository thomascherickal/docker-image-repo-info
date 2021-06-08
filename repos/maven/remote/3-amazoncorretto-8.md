## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:a1872a37a71e6de177202203cbb1123a4c2a7ed69bc13f259867c16629d2ac37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:ca54be2aebc1de64b7fc4370af77d0f52a9b67a445b6e424d4bbb6415280f5f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150454525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f9c121e06532d11d2c74a235db8059f71d0b91924e486ef47e5ec18cfad600`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 29 Apr 2021 22:25:37 GMT
ADD file:47fcf0318dccec16b61a0d21a0f16c45b77dea5abf50ba6604f1ffadcb299d10 in / 
# Thu, 29 Apr 2021 22:25:38 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:44:18 GMT
ARG version=1.8.0_292.b10-1
# Tue, 08 Jun 2021 00:19:42 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 08 Jun 2021 00:19:42 GMT
ENV LANG=C.UTF-8
# Tue, 08 Jun 2021 00:19:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Tue, 08 Jun 2021 00:49:36 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 08 Jun 2021 00:49:36 GMT
ARG USER_HOME_DIR=/root
# Tue, 08 Jun 2021 00:49:37 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 08 Jun 2021 00:49:37 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 08 Jun 2021 00:49:46 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Tue, 08 Jun 2021 00:49:48 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 08 Jun 2021 00:49:48 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 08 Jun 2021 00:49:49 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 08 Jun 2021 00:49:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Tue, 08 Jun 2021 00:49:49 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 08 Jun 2021 00:49:49 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 08 Jun 2021 00:49:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 08 Jun 2021 00:49:49 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3c2c91c7c4311eca863331479504040ee4f45fda9a610947b82886e7bbd5b737`  
		Last Modified: Thu, 29 Apr 2021 22:27:18 GMT  
		Size: 61.9 MB (61947132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208abeba43225ffca24ba33c2ad70ea4c1b237116c3dd0b14bb0cc1b69e9ec4`  
		Last Modified: Tue, 08 Jun 2021 00:20:44 GMT  
		Size: 75.3 MB (75309778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e320fd7999066689b7d44f9d0e146eb8a756d47b86a99584ccd94523b082517`  
		Last Modified: Tue, 08 Jun 2021 00:52:07 GMT  
		Size: 3.6 MB (3585450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d30b8ee56115ded489d92f02ca23e47c7be1c0148a8e005916221bac43af78`  
		Last Modified: Tue, 08 Jun 2021 00:52:08 GMT  
		Size: 9.6 MB (9610956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e0e0891d1b1486ceccd9a4c0cae67e962d8b2750dcf14bf032bb1b67e0d24e`  
		Last Modified: Tue, 08 Jun 2021 00:52:07 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e793d82bd9ed847350215139c62ff1654990bceed40289d7770a7086253c19ab`  
		Last Modified: Tue, 08 Jun 2021 00:52:07 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:eb9bcd61af4b045517eb971e283d3b5b58a9dc4f95471ba6c2a9547c1f0b8007
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136250724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7d554f563541cb1eb2b8f847fab54708e6bb5d98b998af76e213175d5d22cf`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 03 Jun 2021 21:39:22 GMT
ADD file:03605b69274d89b78234df03d53dacc9cac408d68b82b1fb5d63b84c01b69300 in / 
# Thu, 03 Jun 2021 21:39:22 GMT
CMD ["/bin/bash"]
# Fri, 04 Jun 2021 02:58:08 GMT
ARG version=1.8.0_292.b10-1
# Mon, 07 Jun 2021 23:39:40 GMT
# ARGS: version=1.8.0_292.b10-1
RUN set -eux     && if [[ `arch` == 'aarch64' ]]; then version=1.8.0_292.b10-2; fi     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 07 Jun 2021 23:39:41 GMT
ENV LANG=C.UTF-8
# Mon, 07 Jun 2021 23:39:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Tue, 08 Jun 2021 00:17:52 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 08 Jun 2021 00:17:52 GMT
ARG USER_HOME_DIR=/root
# Tue, 08 Jun 2021 00:17:52 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 08 Jun 2021 00:17:53 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 08 Jun 2021 00:18:00 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Tue, 08 Jun 2021 00:18:07 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 08 Jun 2021 00:18:07 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 08 Jun 2021 00:18:07 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 08 Jun 2021 00:18:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Tue, 08 Jun 2021 00:18:08 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 08 Jun 2021 00:18:08 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 08 Jun 2021 00:18:08 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 08 Jun 2021 00:18:08 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:316be4ce82c0add9f71a6ce1face38b99f456abd45232cf7ad96ccac098ef5fe`  
		Last Modified: Thu, 29 Apr 2021 22:41:52 GMT  
		Size: 63.7 MB (63660068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f463bc9e7ce3860652ffe3d3b9dd0046c6736599da78d4a216e741d24b6192f5`  
		Last Modified: Mon, 07 Jun 2021 23:40:44 GMT  
		Size: 59.4 MB (59385977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d8706ec3c8596d708b1aade04977d08ab064bc768e5b2ee333101ca0076228`  
		Last Modified: Tue, 08 Jun 2021 00:22:06 GMT  
		Size: 3.6 MB (3592500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f50a80d5ef1d42aa373bca99904d4fa2d6918c1e37fcf27989623397bcb45cb`  
		Last Modified: Tue, 08 Jun 2021 00:22:06 GMT  
		Size: 9.6 MB (9610966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8dec394bffdd3fad70b6257594fde99403c92513ffa39c639d7a8a0b8d6105c`  
		Last Modified: Tue, 08 Jun 2021 00:22:05 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a859faad8468b4a7f2468b23fbbee21e0f613b06bb4c285ccd9d069e69fec9`  
		Last Modified: Tue, 08 Jun 2021 00:22:05 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
