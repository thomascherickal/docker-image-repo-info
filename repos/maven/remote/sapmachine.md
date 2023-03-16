## `maven:sapmachine`

```console
$ docker pull maven@sha256:67808a00a73477246e06004ec4426684426261bf601b5169f6d877ffa80f1840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `maven:sapmachine` - linux; amd64

```console
$ docker pull maven@sha256:a8a65de2672cc163899cdaf5c8d1a16bb3311d25e42695db4208bd7ef21a2038
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.5 MB (273476680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34514902d5c2f57377e0add6a5a4a77a5f39302078905c2ebd51ac8ba7e1385a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:26:17 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:27:27 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.6     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:27:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Thu, 16 Mar 2023 01:27:28 GMT
CMD ["jshell"]
# Thu, 16 Mar 2023 06:07:14 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Mar 2023 06:07:14 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Mar 2023 06:07:14 GMT
ARG SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd
# Thu, 16 Mar 2023 06:07:14 GMT
ARG BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries
# Thu, 16 Mar 2023 06:07:14 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Mar 2023 06:07:14 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Mar 2023 06:07:28 GMT
# ARGS: BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries MAVEN_VERSION=3.9.0 SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd USER_HOME_DIR=/root
RUN set -x   && apt-get update   && apt-get install -y ca-certificates curl git gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  apache-maven-${MAVEN_VERSION}-bin.tar.gz" | sha512sum -c -   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys   6A814B1F869C2BBEAB7CB7271A2A1C94BDE89688   29BEA2A645F2D6CED7FB12E02B172E3E156466E8   && gpg --batch --verify apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz   && mkdir -p ${MAVEN_HOME} ${MAVEN_HOME}/ref   && tar -xzf apache-maven-${MAVEN_VERSION}-bin.tar.gz -C ${MAVEN_HOME} --strip-components=1   && (rm -rf "$GNUPGHOME" apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz || true)   && ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn   && apt-get remove --purge --autoremove -y gnupg dirmngr   && mvn --version
# Thu, 16 Mar 2023 06:07:29 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 16 Mar 2023 06:07:29 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 16 Mar 2023 06:07:29 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Mar 2023 06:07:29 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64f3b1d0b88367c9674c2ad7667c1472644ab30869cfa9bf4a742956941bdb7`  
		Last Modified: Thu, 16 Mar 2023 01:28:18 GMT  
		Size: 7.9 MB (7917721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ae572d9e7f03f1dc112631e8dd1680621a83e7ae00e1ed8a4dc2c1becda3ae`  
		Last Modified: Thu, 16 Mar 2023 01:28:54 GMT  
		Size: 198.1 MB (198080464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc4595a2ca5cd6fff624091e3c9b8c5ca6e9d8dbbb57e97619e5377f978ad4b`  
		Last Modified: Thu, 16 Mar 2023 06:12:22 GMT  
		Size: 38.9 MB (38899219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f6e50bac086656cd5b2d26461a7bb4e651bc82e00da0a11d3358afbef0c5a2`  
		Last Modified: Thu, 16 Mar 2023 06:12:17 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf0049d4e46be2e521b3be8bd868e3309c65ba4d2071014297b3c53b16131d9`  
		Last Modified: Thu, 16 Mar 2023 06:12:17 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:sapmachine` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:bd80ae01b7fe6fc769141f60893d7c4d95ce4f0ae46322d2b49e5faea2440d73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.0 MB (270002380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dae678a5173c69a4a5373a34d784977d44a3d8e4ee133bd64dfa479cd26255b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:54:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:55:28 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.6     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:55:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Thu, 16 Mar 2023 03:55:30 GMT
CMD ["jshell"]
# Thu, 16 Mar 2023 06:01:12 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Mar 2023 06:01:12 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Mar 2023 06:01:12 GMT
ARG SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd
# Thu, 16 Mar 2023 06:01:12 GMT
ARG BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries
# Thu, 16 Mar 2023 06:01:12 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Mar 2023 06:01:12 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Mar 2023 06:01:24 GMT
# ARGS: BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries MAVEN_VERSION=3.9.0 SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd USER_HOME_DIR=/root
RUN set -x   && apt-get update   && apt-get install -y ca-certificates curl git gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  apache-maven-${MAVEN_VERSION}-bin.tar.gz" | sha512sum -c -   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys   6A814B1F869C2BBEAB7CB7271A2A1C94BDE89688   29BEA2A645F2D6CED7FB12E02B172E3E156466E8   && gpg --batch --verify apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz   && mkdir -p ${MAVEN_HOME} ${MAVEN_HOME}/ref   && tar -xzf apache-maven-${MAVEN_VERSION}-bin.tar.gz -C ${MAVEN_HOME} --strip-components=1   && (rm -rf "$GNUPGHOME" apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz || true)   && ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn   && apt-get remove --purge --autoremove -y gnupg dirmngr   && mvn --version
# Thu, 16 Mar 2023 06:01:24 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 16 Mar 2023 06:01:24 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 16 Mar 2023 06:01:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Mar 2023 06:01:24 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c31633819b087c3d39e7948f611348779db8dd22bc8a3db707f870d7cd24b3`  
		Last Modified: Thu, 16 Mar 2023 03:56:12 GMT  
		Size: 7.8 MB (7757240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a37334232fc2008f6bbcb04969537ab530206c40ad106fd76326bac241c1ca`  
		Last Modified: Thu, 16 Mar 2023 03:56:43 GMT  
		Size: 196.1 MB (196108832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c810bb603746445e635471e4d64d6bb88d152bd296328d992bd202f68988d90c`  
		Last Modified: Thu, 16 Mar 2023 06:05:35 GMT  
		Size: 38.9 MB (38938937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d980c8b795b4dc995aef080300d7383b050992628548c592c8d41d66be1e09f6`  
		Last Modified: Thu, 16 Mar 2023 06:05:31 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2d42eac29fb82b7a4fe33d3da1b75fdea8bc5edf0effa5f2bc116425d56def`  
		Last Modified: Thu, 16 Mar 2023 06:05:31 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:sapmachine` - linux; ppc64le

```console
$ docker pull maven@sha256:8b3229f7e94e0eae3d84b4f331487c0ec985fa28c705741f662b4213d3b2d815
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.5 MB (286525933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1e236b879e6ab80f4326f7eab0ccfc81c7ccc01995167356948f25ebdb4f2f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:14 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:39:17 GMT
ADD file:e8eae0af07e662df38a5b691d04648b4fc72382b6918877da22520ed4d01c3a6 in / 
# Wed, 08 Mar 2023 04:39:17 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:49:28 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:53:10 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.6     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:53:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Thu, 16 Mar 2023 02:53:15 GMT
CMD ["jshell"]
# Thu, 16 Mar 2023 04:30:12 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Mar 2023 04:30:12 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Mar 2023 04:30:13 GMT
ARG SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd
# Thu, 16 Mar 2023 04:30:13 GMT
ARG BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries
# Thu, 16 Mar 2023 04:30:13 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Mar 2023 04:30:14 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Mar 2023 04:30:44 GMT
# ARGS: BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries MAVEN_VERSION=3.9.0 SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd USER_HOME_DIR=/root
RUN set -x   && apt-get update   && apt-get install -y ca-certificates curl git gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  apache-maven-${MAVEN_VERSION}-bin.tar.gz" | sha512sum -c -   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys   6A814B1F869C2BBEAB7CB7271A2A1C94BDE89688   29BEA2A645F2D6CED7FB12E02B172E3E156466E8   && gpg --batch --verify apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz   && mkdir -p ${MAVEN_HOME} ${MAVEN_HOME}/ref   && tar -xzf apache-maven-${MAVEN_VERSION}-bin.tar.gz -C ${MAVEN_HOME} --strip-components=1   && (rm -rf "$GNUPGHOME" apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz || true)   && ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn   && apt-get remove --purge --autoremove -y gnupg dirmngr   && mvn --version
# Thu, 16 Mar 2023 04:30:46 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 16 Mar 2023 04:30:46 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 16 Mar 2023 04:30:47 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Mar 2023 04:30:47 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:35c7876eb976fb68d0f3bf24f227b6220a73f879e77ad564d913af35104da2eb`  
		Last Modified: Thu, 16 Mar 2023 01:58:06 GMT  
		Size: 33.3 MB (33300378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287fe41bdc8fb09ac5317ba55919a01ec0458a942720c3be52727923a6c60280`  
		Last Modified: Thu, 16 Mar 2023 02:55:51 GMT  
		Size: 9.3 MB (9316584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9033a2be5149a2cafea5c523c6f064c2d3a3e0055cc2264827b6861ba150527`  
		Last Modified: Thu, 16 Mar 2023 02:56:46 GMT  
		Size: 198.2 MB (198224075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4856e526d534ede82cf23c5e90d87e801d2ee6e5d9c56aeb15b29f64424758`  
		Last Modified: Thu, 16 Mar 2023 04:38:03 GMT  
		Size: 45.7 MB (45683682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24460eb215192420a1030035b75256c8381c00efa7dbe305f475f267588321f9`  
		Last Modified: Thu, 16 Mar 2023 04:37:52 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a369304a2e0aeaccf7bfc2adad917c578d9e02fc6dfa19a2bf1e85d3a1e217`  
		Last Modified: Thu, 16 Mar 2023 04:37:52 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
