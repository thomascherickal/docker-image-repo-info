## `neo4j:enterprise-ubi8`

```console
$ docker pull neo4j@sha256:6d684e23849b05bed6e9d589f60036368c33d70465352612d4f8b676153c730f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:e3ba36cc8116e106a391077d1d52df2a0237c9f57985ff0c1f6af26ebf4327ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **578.0 MB (578015099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef573daca717ad7adc8ecf3366146eb511ddc62c3e6e5556d4278c4fa2dd71eb`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 03:26:53 GMT
ADD file:47589af4a3da87e21edebcff87ac699aa8818e369afb7b60c9a26f193942db3e in / 
# Wed, 01 Nov 2023 03:26:53 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 01 Nov 2023 03:26:54 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 01 Nov 2023 03:26:54 GMT
ADD multi:1d8f8a6ff2fa00884e209245ce9248e4cee06aa7f27bdf4f90dc2edc3498c511 in /etc/yum.repos.d/ 
# Wed, 01 Nov 2023 03:26:54 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 01 Nov 2023 03:26:54 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.9"
# Wed, 01 Nov 2023 03:26:54 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 01 Nov 2023 03:26:54 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 01 Nov 2023 03:26:54 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 01 Nov 2023 03:26:54 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 01 Nov 2023 03:26:54 GMT
LABEL io.openshift.expose-services=""
# Wed, 01 Nov 2023 03:26:54 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 01 Nov 2023 03:26:54 GMT
ENV container oci
# Wed, 01 Nov 2023 03:26:54 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 03:26:54 GMT
CMD ["/bin/bash"]
# Wed, 01 Nov 2023 03:26:55 GMT
RUN rm -rf /var/log/*
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL release=1029
# Wed, 01 Nov 2023 03:26:55 GMT
ADD file:732950e4831bd3dbf3c279f66da444e65ecc2962a326463fc1748a7ef063d841 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.9-1029.json 
# Wed, 01 Nov 2023 03:26:55 GMT
ADD file:b361c9d04ed3cbb92e69fd3858c1b12aecbd2de1bf55967db6159058c4a49e12 in /root/buildinfo/Dockerfile-ubi8-minimal-8.9-1029 
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-11-01T03:17:36" "architecture"="x86_64" "vcs-type"="git" "vcs-ref"="7e7670a8c8c9a3be83beaa2787f3703b404d4a1d" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.9-1029"
# Wed, 01 Nov 2023 03:26:56 GMT
RUN rm -f '/etc/yum.repos.d/repo-3b08a.repo' '/etc/yum.repos.d/repo-4c95e.repo'
# Wed, 01 Nov 2023 03:26:56 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 01 Nov 2023 03:26:57 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Fri, 15 Dec 2023 20:25:51 GMT
ENV JAVA_HOME=/usr
# Fri, 15 Dec 2023 20:27:49 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y dnf;     dnf install -y         findutils         gcc         git         gzip         hostname         java-17         jq         make         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     git clone https://github.com/ncopa/su-exec.git;     cd su-exec;     git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af;     echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c;     echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c;     make;     mv /su-exec/su-exec /usr/bin/su-exec;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc /su-exec;     dnf remove -y gcc git make;     dnf autoremove;     dnf clean all
# Fri, 15 Dec 2023 20:28:00 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:28:00 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:28:00 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:28:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 20:28:11 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:28:11 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:28:11 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:28:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:28:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:28:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f4a3c904e5565efee16dbcb82838bbb64a39f8261e4531648bc591c528236c24`  
		Last Modified: Wed, 15 Nov 2023 18:35:34 GMT  
		Size: 39.3 MB (39341714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dda4a0acb5ab684d16d48c8d5323361f87dddfd9a10f08dbb00c7b4ca55ab1e`  
		Last Modified: Fri, 15 Dec 2023 20:30:25 GMT  
		Size: 152.2 MB (152158147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5596a79f49cda7601c69d4b3fb937fa94fadc4e7bde0cd7c1c3a01ddae8ea6c5`  
		Last Modified: Fri, 15 Dec 2023 20:30:45 GMT  
		Size: 9.5 KB (9486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f19a74dc54dccef581bf70b00138db5228621c1eb5efeb565228d7cba25edc0`  
		Last Modified: Fri, 15 Dec 2023 20:31:02 GMT  
		Size: 386.5 MB (386505752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:131ee2c8e2034705fdcb90abd05e88900a4f5efdea66ed4d62f3b132773aab5c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.9 MB (574918918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9698568f5adf580f2f476bc3ac3980e58d6ae295c18f598f2f901a216054cad`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Nov 2023 03:26:54 GMT
ADD file:2268389f6691723ff73eafb7f91e3fc2326d5d821040b1e7b1f16f6ca6a450c7 in / 
# Wed, 01 Nov 2023 03:26:55 GMT
RUN mv -f /etc/yum.repos.d/ubi.repo /tmp || :
# Wed, 01 Nov 2023 03:26:55 GMT
ADD file:ecc29a1455ca1b7c82018555e16e2e802135974523df6748e431f8707e759ddd in /tmp/tls-ca-bundle.pem 
# Wed, 01 Nov 2023 03:26:55 GMT
ADD multi:1d8f8a6ff2fa00884e209245ce9248e4cee06aa7f27bdf4f90dc2edc3498c511 in /etc/yum.repos.d/ 
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL maintainer="Red Hat, Inc."
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL com.redhat.component="ubi8-minimal-container"       name="ubi8-minimal"       version="8.9"
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL com.redhat.license_terms="https://www.redhat.com/en/about/red-hat-end-user-license-agreements#UBI"
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL summary="Provides the latest release of the minimal Red Hat Universal Base Image 8."
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL description="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly."
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL io.k8s.display-name="Red Hat Universal Base Image 8 Minimal"
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL io.openshift.expose-services=""
# Wed, 01 Nov 2023 03:26:55 GMT
LABEL io.openshift.tags="minimal rhel8"
# Wed, 01 Nov 2023 03:26:55 GMT
ENV container oci
# Wed, 01 Nov 2023 03:26:55 GMT
ENV PATH /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 03:26:55 GMT
CMD ["/bin/bash"]
# Wed, 01 Nov 2023 03:26:56 GMT
RUN rm -rf /var/log/*
# Wed, 01 Nov 2023 03:26:56 GMT
LABEL release=1029
# Wed, 01 Nov 2023 03:26:57 GMT
ADD file:aa421ceadf9415f2c5b67b3b5d9a8543215bfc83157831e4d93bf5ac187a6549 in /root/buildinfo/content_manifests/ubi8-minimal-container-8.9-1029.json 
# Wed, 01 Nov 2023 03:26:57 GMT
ADD file:075dfdece656aa5ed8d1c9a45607ce60c4b2c2025f8cd0516d52cecf2e8331f0 in /root/buildinfo/Dockerfile-ubi8-minimal-8.9-1029 
# Wed, 01 Nov 2023 03:26:57 GMT
LABEL "distribution-scope"="public" "vendor"="Red Hat, Inc." "build-date"="2023-11-01T03:17:36" "architecture"="aarch64" "vcs-type"="git" "vcs-ref"="7e7670a8c8c9a3be83beaa2787f3703b404d4a1d" "io.k8s.description"="The Universal Base Image Minimal is a stripped down image that uses microdnf as a package manager. This base image is freely redistributable, but Red Hat only supports Red Hat technologies through subscriptions for Red Hat products. This image is maintained by Red Hat and updated regularly." "url"="https://access.redhat.com/containers/#/registry.access.redhat.com/ubi8-minimal/images/8.9-1029"
# Wed, 01 Nov 2023 03:26:58 GMT
RUN rm -f '/etc/yum.repos.d/repo-3b08a.repo' '/etc/yum.repos.d/repo-4c95e.repo'
# Wed, 01 Nov 2023 03:26:59 GMT
RUN rm -f /tmp/tls-ca-bundle.pem
# Wed, 01 Nov 2023 03:27:01 GMT
RUN mv -fZ /tmp/ubi.repo /etc/yum.repos.d/ubi.repo || :
# Fri, 15 Dec 2023 19:54:50 GMT
ENV JAVA_HOME=/usr
# Fri, 15 Dec 2023 19:56:44 GMT
RUN set -eux;     arch="$(uname -m)";     case "${arch}" in         'x86_64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini";             tinisha="93dcc18adc78c65a028a84799ecf8ad40c936fdfc5f2a57b1acda5a8117fa82c";             ;;         'aarch64')             tiniurl="https://github.com/krallin/tini/releases/download/v0.19.0/tini-arm64";             tinisha="07952557df20bfd2a95f9bef198b445e006171969499a1d361bd9e6f8e5e0e81";             ;;         *) echo >&2 "Neo4j does not currently have a docker image for architecture $arch"; exit 1 ;;     esac;     microdnf install -y dnf;     dnf install -y         findutils         gcc         git         gzip         hostname         java-17         jq         make         procps         shadow-utils         tar         wget         which;     wget -q ${tiniurl} -O /usr/bin/tini;     wget -q ${tiniurl}.asc -O tini.asc;     echo "${tinisha}"  /usr/bin/tini | sha256sum -c --strict --quiet;     chmod a+x /usr/bin/tini;     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys         595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7         B42F6819007F00F88E364FD4036A9C25BF357DD4;     gpg --batch --verify tini.asc /usr/bin/tini;     git clone https://github.com/ncopa/su-exec.git;     cd su-exec;     git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af;     echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c;     echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c;     make;     mv /su-exec/su-exec /usr/bin/su-exec;     gpgconf --kill all;     rm -rf "$GNUPGHOME" tini.asc /su-exec;     dnf remove -y gcc git make;     dnf autoremove;     dnf clean all
# Fri, 15 Dec 2023 19:56:58 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:56:58 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:56:58 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:57:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 19:57:11 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:57:11 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:57:11 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:57:11 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:57:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:57:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:efe07ddbececa05537c13805b89ed74cb770f1dde30ddcae0a6c60ccd010ea2f`  
		Last Modified: Wed, 15 Nov 2023 19:35:11 GMT  
		Size: 37.7 MB (37682884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf521cc5c8f1be6b54de00852644988a52cd4537fa3ef91f686317332ebdc910`  
		Last Modified: Fri, 15 Dec 2023 19:59:10 GMT  
		Size: 150.7 MB (150720739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c1a7f1532d7afed323187195c037c824035dbff9315c4be0b555f83888d77e`  
		Last Modified: Fri, 15 Dec 2023 19:59:30 GMT  
		Size: 9.5 KB (9486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13f87ea7b807edecd8a1c6bbf219d7b5b05cf40dbf0517a131b4dc73cecee53`  
		Last Modified: Fri, 15 Dec 2023 19:59:43 GMT  
		Size: 386.5 MB (386505809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
