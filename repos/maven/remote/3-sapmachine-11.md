## `maven:3-sapmachine-11`

```console
$ docker pull maven@sha256:ebefdb8542e3947c23bd38b26ec54f31451c64c4bb9fcf16170f87410fd789fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `maven:3-sapmachine-11` - linux; amd64

```console
$ docker pull maven@sha256:176b33ee61c09be41f88f2daa0b5154a9bab07f9e6f097c2d1e9bb81b2b28dd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.3 MB (274326749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4916d7835d528a1428cadb64fc5270e43d9e020d06418a57ade5bb5d9e11a303`
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
# Thu, 16 Mar 2023 01:26:50 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.18     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:26:51 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 16 Mar 2023 01:26:51 GMT
CMD ["jshell"]
# Thu, 16 Mar 2023 06:06:54 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Mar 2023 06:06:54 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Mar 2023 06:06:54 GMT
ARG SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd
# Thu, 16 Mar 2023 06:06:54 GMT
ARG BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries
# Thu, 16 Mar 2023 06:06:54 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Mar 2023 06:06:54 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Mar 2023 06:07:10 GMT
# ARGS: BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries MAVEN_VERSION=3.9.0 SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd USER_HOME_DIR=/root
RUN set -x   && apt-get update   && apt-get install -y ca-certificates curl git gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  apache-maven-${MAVEN_VERSION}-bin.tar.gz" | sha512sum -c -   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys   6A814B1F869C2BBEAB7CB7271A2A1C94BDE89688   29BEA2A645F2D6CED7FB12E02B172E3E156466E8   && gpg --batch --verify apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz   && mkdir -p ${MAVEN_HOME} ${MAVEN_HOME}/ref   && tar -xzf apache-maven-${MAVEN_VERSION}-bin.tar.gz -C ${MAVEN_HOME} --strip-components=1   && (rm -rf "$GNUPGHOME" apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz || true)   && ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn   && apt-get remove --purge --autoremove -y gnupg dirmngr   && mvn --version
# Thu, 16 Mar 2023 06:07:11 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 16 Mar 2023 06:07:11 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 16 Mar 2023 06:07:11 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Mar 2023 06:07:11 GMT
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
	-	`sha256:e90bdbb3b98b6c912f9103f8f77afbe33ec06ebce2b7b9160f7458614ebd7412`  
		Last Modified: Thu, 16 Mar 2023 01:28:31 GMT  
		Size: 198.9 MB (198930458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ff626c903444ab8172c9fd391cb7add5d8b3a6ea67bcba00b543d768313bb5`  
		Last Modified: Thu, 16 Mar 2023 06:12:06 GMT  
		Size: 38.9 MB (38899292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aca14e58ff27c06d042850989ef4582311bb7f724c264484da93eae3ea99508`  
		Last Modified: Thu, 16 Mar 2023 06:12:01 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577e3454550ea5c6573b4f0d74d671ee7b6b77c161a0850a5685b9542aff0923`  
		Last Modified: Thu, 16 Mar 2023 06:12:01 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-sapmachine-11` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:bcd55a6d56c8ca3f034379774ca35f610cdb13abab4b958af0eec2551376032f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.8 MB (270762107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4862b1d68c7ab4e6e8b110fc0e77012051dd32b9668a541916bafc36ec715c6`
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
# Thu, 16 Mar 2023 03:55:00 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.18     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:55:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 16 Mar 2023 03:55:02 GMT
CMD ["jshell"]
# Thu, 16 Mar 2023 06:00:48 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Mar 2023 06:00:48 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Mar 2023 06:00:48 GMT
ARG SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd
# Thu, 16 Mar 2023 06:00:48 GMT
ARG BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries
# Thu, 16 Mar 2023 06:00:49 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Mar 2023 06:00:49 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Mar 2023 06:01:08 GMT
# ARGS: BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries MAVEN_VERSION=3.9.0 SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd USER_HOME_DIR=/root
RUN set -x   && apt-get update   && apt-get install -y ca-certificates curl git gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  apache-maven-${MAVEN_VERSION}-bin.tar.gz" | sha512sum -c -   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys   6A814B1F869C2BBEAB7CB7271A2A1C94BDE89688   29BEA2A645F2D6CED7FB12E02B172E3E156466E8   && gpg --batch --verify apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz   && mkdir -p ${MAVEN_HOME} ${MAVEN_HOME}/ref   && tar -xzf apache-maven-${MAVEN_VERSION}-bin.tar.gz -C ${MAVEN_HOME} --strip-components=1   && (rm -rf "$GNUPGHOME" apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz || true)   && ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn   && apt-get remove --purge --autoremove -y gnupg dirmngr   && mvn --version
# Thu, 16 Mar 2023 06:01:09 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 16 Mar 2023 06:01:09 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 16 Mar 2023 06:01:09 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Mar 2023 06:01:09 GMT
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
	-	`sha256:5d11ce92bc63bc694aa4a48385a4db111547fe48e3897858dc8ba02a261a0961`  
		Last Modified: Thu, 16 Mar 2023 03:56:23 GMT  
		Size: 196.9 MB (196868346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3088b657ddcf90a65a1c86b2800b59ebfd01c597b2418f9bc9f5cc96c1fe221a`  
		Last Modified: Thu, 16 Mar 2023 06:05:20 GMT  
		Size: 38.9 MB (38939149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80ac59b1cca9031d52c33c5444a399fce7f7721758714b2a35d0c88251788ba`  
		Last Modified: Thu, 16 Mar 2023 06:05:16 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba9a66e9802225237e9132e1fb4d2cec53903316417c74a59bee9e4073dc771`  
		Last Modified: Thu, 16 Mar 2023 06:05:16 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-sapmachine-11` - linux; ppc64le

```console
$ docker pull maven@sha256:fcdbc3867e939d9fa7056f12e835b75714168b85e888587f728b2c73196b5c8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.2 MB (273150638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c8315a3a91bee79b49678b09babcc526564bc5712fd782be57ff3f4cc83550`
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
# Thu, 16 Mar 2023 02:51:16 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/$(dpkg --print-architecture)/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.18     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:51:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 16 Mar 2023 02:51:22 GMT
CMD ["jshell"]
# Thu, 16 Mar 2023 04:29:21 GMT
ARG MAVEN_VERSION=3.9.0
# Thu, 16 Mar 2023 04:29:22 GMT
ARG USER_HOME_DIR=/root
# Thu, 16 Mar 2023 04:29:22 GMT
ARG SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd
# Thu, 16 Mar 2023 04:29:24 GMT
ARG BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries
# Thu, 16 Mar 2023 04:29:25 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 16 Mar 2023 04:29:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 16 Mar 2023 04:30:03 GMT
# ARGS: BASE_URL=https://downloads.apache.org/maven/maven-3/3.9.0/binaries MAVEN_VERSION=3.9.0 SHA=1ea149f4e48bc7b34d554aef86f948eca7df4e7874e30caf449f3708e4f8487c71a5e5c072a05f17c60406176ebeeaf56b5f895090c7346f8238e2da06cf6ecd USER_HOME_DIR=/root
RUN set -x   && apt-get update   && apt-get install -y ca-certificates curl git gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  apache-maven-${MAVEN_VERSION}-bin.tar.gz" | sha512sum -c -   && curl -fsSLO --compressed ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys   6A814B1F869C2BBEAB7CB7271A2A1C94BDE89688   29BEA2A645F2D6CED7FB12E02B172E3E156466E8   && gpg --batch --verify apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz   && mkdir -p ${MAVEN_HOME} ${MAVEN_HOME}/ref   && tar -xzf apache-maven-${MAVEN_VERSION}-bin.tar.gz -C ${MAVEN_HOME} --strip-components=1   && (rm -rf "$GNUPGHOME" apache-maven-${MAVEN_VERSION}-bin.tar.gz.asc apache-maven-${MAVEN_VERSION}-bin.tar.gz || true)   && ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn   && apt-get remove --purge --autoremove -y gnupg dirmngr   && mvn --version
# Thu, 16 Mar 2023 04:30:05 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 16 Mar 2023 04:30:05 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 16 Mar 2023 04:30:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 16 Mar 2023 04:30:06 GMT
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
	-	`sha256:dfb4001c216aa44d4c74aea488fe3c81de8e5cb4f704800979440e955925035e`  
		Last Modified: Thu, 16 Mar 2023 02:56:11 GMT  
		Size: 184.8 MB (184848592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6d93007d89727b40b8e1ce9b355931b583e548e9a1e09a8c8691118f792ce2`  
		Last Modified: Thu, 16 Mar 2023 04:37:38 GMT  
		Size: 45.7 MB (45683872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d90ad77de40a959ed0a4ee3cd95ee6a5c4e43bbafd0bbf47f0d35ea01560424`  
		Last Modified: Thu, 16 Mar 2023 04:37:28 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519700feb1fe25864c672bf6c905e892e5966020d28a23657f7947e94bdc42d3`  
		Last Modified: Thu, 16 Mar 2023 04:37:28 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
