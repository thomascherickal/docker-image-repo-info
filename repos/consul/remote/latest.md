## `consul:latest`

```console
$ docker pull consul@sha256:ee0735e34f80030c46002f71bc594f25e3f586202da8784b43b4050993ef2445
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:a1a933572cb6f6388501c535af455f77e687c62ff97ed72cd16301b8b535eae0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49530995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8382d411eded180b186fa0dafa69be7eb8900927334e9bab5890768214face2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 18:27:05 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 18:27:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 18:27:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 18:27:06 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 18:27:11 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 18:27:12 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 18:27:12 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:27:12 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 18:27:12 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 18:27:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 18:27:13 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 18:27:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 18:27:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:27:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa48d4bd8bb86e29ae52b54a2008aa622c3781fd6acfa2e44cd5cf859c43b71`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3ef9b012a54ea43a997ab9743977bc7de3f516332dcd8999f4a4910b14122a`  
		Last Modified: Mon, 06 Jun 2022 18:27:35 GMT  
		Size: 46.7 MB (46713053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d239fc798a4c5e4c738352dbdcdd697322a05c5b89a9cd9ccc97a3abf1f2eb46`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199124be58be7085ef632c2297dde8e22271f783567ed177c68c6a2783bb7aec`  
		Last Modified: Mon, 06 Jun 2022 18:27:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3ccfe93b8bfca6058f2fab81810f5ba9c826430efab6bdd28121f00659804f`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:562c2055e7b6163ad791098ab5f7fb763f7b58ef1b3a365326ddeb200af5bc07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47418871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ddedc80aeddd358a9aff2ade7924f8f3a0d19d7bf1a70abebfd2496501abb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:49:33 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:49:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:49:35 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:49:49 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:49:51 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:49:52 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:49:53 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:49:53 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:49:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:49:54 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:49:54 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:49:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172c64f605f02c13d89a26d7e1de51cf5f9989f437513d0bb157426ce7c9bddb`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b94fb31045febe567631bd92baee9f2f2910606e6f037fc6a6e2a54cbd4d9`  
		Last Modified: Mon, 06 Jun 2022 17:51:20 GMT  
		Size: 44.8 MB (44793515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714921570995a97c88cc9e28f77625ad774b2608eeb728e8e341e98e6a256124`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adf595d95028707c1de711e10c2f3fa391c3e0a1521bf76b6590ba8d920e9c9`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3f382a916bc2905df02883c1cd108693474e87b57c30644c7f2eb5d2eed41e`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c945c9f9d79e884233267d9c02105ffc460399dfaf09f31f38b7d7b1f43ab918
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47164176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4164dd78d95ff52b3c182bc2bf7ec45d64e72ce6c393cea25215d8bacea3577d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:47:05 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:47:06 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:47:07 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:47:08 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:47:14 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:47:15 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:47:15 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:47:16 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:47:17 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:47:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:47:19 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:47:21 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:47:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852dd48866308bd671353173a738be13359e088984374548057b76df8a03bdd9`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f57f7ce3f084ee916ca7c8580644f9e0e4e1e6b07b13b5720e572981816050`  
		Last Modified: Mon, 06 Jun 2022 17:47:58 GMT  
		Size: 44.4 MB (44444379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120c060cfede9a3c8d97bfb29222215dad767dfe20514beb78bf941e888e8cad`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be076a16914a6d835a25711f47eac0a9690a1ab7a7362915519b039a761d3d5d`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890c17b7a032ee37b9a6fe51b9dfdfa53b209f35799c507be8ab046f942b3497`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:c7ee39a9eace8e5a94fbb79b8c659651a058a0ccccba3f3cd7218835ed75f5db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48612065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36be6b9b2a08cdf391475699a481ac9186505965fe95ca32e6caebddae126f89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:42:20 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:42:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:42:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:42:23 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:42:31 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:42:31 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:42:32 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:42:33 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:42:34 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:42:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:42:36 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:42:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:42:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:42:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c036d14492d1b2b557706d2e054d0380f769c81beceb949ed0600c7f58b9851b`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0356a6434d39e3976b4b6f9235bb3c740e70d4149e5c6b710c3653b247d0f07`  
		Last Modified: Mon, 06 Jun 2022 17:43:17 GMT  
		Size: 45.8 MB (45789766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5905d9eeb35e30123e93ddc94dadd6168fea4ecdd6a17474253b445809c33c`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891d5fc673fe12e6017707d85a284b60cd6f8bb339dfe4ed5f5d3565b77f0960`  
		Last Modified: Mon, 06 Jun 2022 17:43:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88d95e4cc9f19bd80a9f01ff330451cea70f9ce4e0e42aca657ccce2c513416`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
