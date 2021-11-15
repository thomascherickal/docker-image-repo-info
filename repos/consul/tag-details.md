<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.4`](#consul1104)
-	[`consul:1.11.0-beta`](#consul1110-beta)
-	[`consul:1.11.0-beta2`](#consul1110-beta2)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.17`](#consul1817)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.11`](#consul1911)
-	[`consul:latest`](#consullatest)

## `consul:1.10`

```console
$ docker pull consul@sha256:483b592fa76d734882cf7336df94a5bf6f9e808a78b1a1ba17002a2aaf80da46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:4fc771d6614f6d7af92653e006157b9c98a05098e43dc485d29d9c846abcc33d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43242800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9814b25e52bae10d44d9953bad57d86e8577283652bc9443be9738031389c48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:58:14 GMT
ARG CONSUL_VERSION=1.10.3
# Fri, 12 Nov 2021 21:58:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 12 Nov 2021 21:58:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 12 Nov 2021 21:58:17 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 12 Nov 2021 21:58:30 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 12 Nov 2021 21:58:32 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 12 Nov 2021 21:58:35 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:58:35 GMT
VOLUME [/consul/data]
# Fri, 12 Nov 2021 21:58:36 GMT
EXPOSE 8300
# Fri, 12 Nov 2021 21:58:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 12 Nov 2021 21:58:36 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 12 Nov 2021 21:58:37 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 21:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 21:58:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79efaa79e0b89d613b7eeb02676f2c706bf77bac920e8657f0f9badfb6205340`  
		Last Modified: Fri, 12 Nov 2021 22:00:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6fccdd38073e2a0303fb7450154fb88dd5211f8abbd8ab1b55e2514a24cb1`  
		Last Modified: Fri, 12 Nov 2021 22:00:07 GMT  
		Size: 40.4 MB (40417007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a1a23e6dad553737585a3b60948d19896dd3c8aeb3ec7e62e0bf03560f416e`  
		Last Modified: Fri, 12 Nov 2021 22:00:01 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae16349669345cc0fb16abc18cd48c1dbf94910caaee5431326c3cf34882559`  
		Last Modified: Fri, 12 Nov 2021 22:00:01 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fa79365c2a7793d97996a84e1a8e28dec95f530224a746f6d4cdca6dfe5f73`  
		Last Modified: Fri, 12 Nov 2021 22:00:01 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:89cd92136a7b8ebd035cb1a0e39b8e96abc49edf60c9200a27f117054b53932c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39269139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd4b0d9415b5a09650d466ee78ea76f2f5f821de5e796590f9339aa0c50e30b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:03:14 GMT
ARG CONSUL_VERSION=1.10.3
# Sat, 13 Nov 2021 06:03:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:03:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:03:17 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:03:29 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:03:31 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:03:33 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:03:34 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:03:34 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:03:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:03:35 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:03:36 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:03:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:03:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95e092b4de70f76b87ef5e2952153af28de56b56c428d170b0f028fb6afbf1d`  
		Last Modified: Sat, 13 Nov 2021 06:06:08 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598923641df439f939be74ba7dc244ef98d48641e316ff947702b24a279c956d`  
		Last Modified: Sat, 13 Nov 2021 06:06:27 GMT  
		Size: 36.6 MB (36632428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b856a08c888ad010360a1dd58e1196cab9d0a174889c005fd0dd1c23a5225c4`  
		Last Modified: Sat, 13 Nov 2021 06:06:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde4ced118232a40da2c756413e2ca1148a45efc645d9f750f232a1dcd7f945f`  
		Last Modified: Sat, 13 Nov 2021 06:06:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e826ae63c559c7b16801bd6e94f70546fbf8739bbb8a33eae3edd323fd2797b7`  
		Last Modified: Sat, 13 Nov 2021 06:06:08 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:49806d20f5bec7cfebaee85b402e0507ecaee84d21875b1666dd145595e76bb9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39197224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79533321836233fbf353f989f599b83489cf6bf766b81ca69b63c2aa78807d37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:15:46 GMT
ARG CONSUL_VERSION=1.10.3
# Sat, 13 Nov 2021 11:15:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 11:15:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 11:15:49 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 11:15:55 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 11:15:55 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 11:15:56 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:15:57 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 11:15:58 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 11:15:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 11:16:00 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 11:16:02 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 11:16:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:16:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af37d8c363d19fa997a18af0e4843fd2f676bb004307d4ad3871b967db1ad181`  
		Last Modified: Sat, 13 Nov 2021 11:17:38 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48713568c234663e5570c3039860b7e2b9be32f1d1044864c25d61fb19a20546`  
		Last Modified: Sat, 13 Nov 2021 11:17:43 GMT  
		Size: 36.5 MB (36474278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2aae487100b5ebe714e5b1f05e968449c0486d160860f20cd3fbc0013dd656`  
		Last Modified: Sat, 13 Nov 2021 11:17:38 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95de985c0b90328a625f0a5932f1f05f0978332a73572d2e3046a7b723882d2`  
		Last Modified: Sat, 13 Nov 2021 11:17:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474b8a1f74bc7aebca99d417b6bff154a2ab0d345ff227d3b1a32d89e781065`  
		Last Modified: Sat, 13 Nov 2021 11:17:38 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; 386

```console
$ docker pull consul@sha256:f6d4990606abae58cfa07041438a83774585b1976889aa17ecfb69c10582149d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42624588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0266e05a345c091de13c2cf497e8d5c997539a31384988e30a540f6338d8e095`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:18:54 GMT
ARG CONSUL_VERSION=1.10.3
# Sat, 13 Nov 2021 06:18:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:18:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:18:56 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:19:06 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:19:07 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:19:08 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:19:08 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:19:08 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:19:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:19:09 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:19:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:19:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:19:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ad71c51a3aaa36ca93ff2d29be265437f8d6a6a3265229463a32d757ab063c`  
		Last Modified: Sat, 13 Nov 2021 06:20:36 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264e1a84ec19e245b5b17560ae89a7a20d673c5065b8e31ad33e1dec79c3a5fc`  
		Last Modified: Sat, 13 Nov 2021 06:20:42 GMT  
		Size: 39.8 MB (39792406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52249b1ddd029a0a2974e3e28a7d4ba4eb74ba1428eba364aab8c0634680193`  
		Last Modified: Sat, 13 Nov 2021 06:20:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e3c995ef13035d9e1361df724e4dbb2f695c7fdf5a1a5dac866ececfd2f54`  
		Last Modified: Sat, 13 Nov 2021 06:20:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefa7778ca9c4c1248a35f60f616d57440c6dda91f0b4afcbf7b464258fa72cf`  
		Last Modified: Sat, 13 Nov 2021 06:20:36 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.4`

**does not exist** (yet?)

## `consul:1.11.0-beta`

```console
$ docker pull consul@sha256:0101ed8ed924388d203962c7f6cd00c64946a2915aa307ae6fdb77257f35afff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:e57b5bd1735f5669571dd93cb358dafcc1274e123f85ec9878f40ba0b506bf22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43713511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33a1fbcf9760adfc346281ab93087515248a09acd754cfa38ad65dd048a23e67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:57:45 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Fri, 12 Nov 2021 21:57:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 12 Nov 2021 21:57:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 12 Nov 2021 21:57:46 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 12 Nov 2021 21:58:02 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 12 Nov 2021 21:58:05 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 12 Nov 2021 21:58:07 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:58:07 GMT
VOLUME [/consul/data]
# Fri, 12 Nov 2021 21:58:08 GMT
EXPOSE 8300
# Fri, 12 Nov 2021 21:58:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 12 Nov 2021 21:58:09 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 12 Nov 2021 21:58:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 21:58:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 21:58:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9dd9907ca9dba4bf6d73592e3433bb41bfd6758f9fda5deee3ba72629b90c0`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ce0fdfb8f1545e60331c6ceb496bd4ff2cedab6c4e0533ab3d9c5132308624`  
		Last Modified: Fri, 12 Nov 2021 21:59:51 GMT  
		Size: 40.9 MB (40887721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c10085b0fae3b6f6041a1de3e35988aa036d8fd1e5a6f67aaff584f889545d`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99692da936ecbe3f732798a699a03861ea39fc25a2664db7e8fd96fa3a05b24c`  
		Last Modified: Fri, 12 Nov 2021 21:59:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e52fae0f8177dd8b49904fe878aaeabaa0eb44d2e78187ff1357a4e88eba7`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:409f4b4355391f1bcc0b8bd49175b308adcc70ddca9bd5dc2dcb3977c5eb23aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39508868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2fcd863378dba6a3d8e0d211cb0030306cf1eeda473f430c45b66185d9f40dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:39 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 06:02:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:02:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:02:42 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:02:55 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:02:57 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:02:59 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:02:59 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:03:00 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:03:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:03:01 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:03:01 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:03:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:03:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2d7260b8a655c8d28c28f40ef7d386ecdf21ec4e683fca1ada03fb077990b1`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d05d8b05f792a5f378b768ab68755d34efcd88553097ba4c11fe6fd0a4fe9b7`  
		Last Modified: Sat, 13 Nov 2021 06:05:56 GMT  
		Size: 36.9 MB (36872153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4c08e221c3a9944278928e0d5a5349f02e20378f200537c7bc0abc72fc4c5b`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc684001062a2334874602425ae1f7f3321952ce632b97090c30715e183b3b6e`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5703c46ca3d761e767f57a57cc7a942a7fd182112bbb0067a92544c78775fec6`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:fb76a00c0c2adc167cd5c1aeca7241360b4a1aa891a892b0a78359a69e206a42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39287714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ebbfccc7daa528654052fa7daeffb5ebbd9e9e26102394b284b36249c55be2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:15:15 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 11:15:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 11:15:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 11:15:18 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 11:15:30 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 11:15:31 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 11:15:32 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:15:33 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 11:15:34 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 11:15:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 11:15:36 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 11:15:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 11:15:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:15:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144af28d402c6aa398c230374e0796f8b1bc72bc894128628950b7e9809cb014`  
		Last Modified: Sat, 13 Nov 2021 11:17:23 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f6468fc5c085fb9f1f7f5be01d4280e6d581d4c0288eb7c853d68b70f84189`  
		Last Modified: Sat, 13 Nov 2021 11:17:28 GMT  
		Size: 36.6 MB (36564764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910209e84ce7afdb47a37c422bb2f445b7a4c4475ad552485d2ee6266a607fc2`  
		Last Modified: Sat, 13 Nov 2021 11:17:23 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287bbf38f5b8c1472195d191f1bed4a366432659146c5082d51de5ea49d59678`  
		Last Modified: Sat, 13 Nov 2021 11:17:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c8e4ce91e5c66b30bdf7716289d2386f28e41ad88c5e9f5690556b9636dd05`  
		Last Modified: Sat, 13 Nov 2021 11:17:22 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; 386

```console
$ docker pull consul@sha256:c329aff5d47eba46e1f6992fbe91dcf9010d6f80005286be9155f965921e7975
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42543628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb87f43018f823068831b78d7e4d452fe84225256e1edaf0aa81e8387567bbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:18:29 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 06:18:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:18:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:18:31 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:18:45 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:18:46 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:18:47 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:18:47 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:18:47 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:18:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:18:48 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:18:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:18:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c847a2ae3f27130e208c92ba400b0bc215dfbd6e6dc859cd2e39ad3aa520a`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a3c64b15b1543034c6e04bb4f1ffb5db0907892bf0e51163848219a87482d`  
		Last Modified: Sat, 13 Nov 2021 06:20:24 GMT  
		Size: 39.7 MB (39711445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bfeef4b841e5af9bbff9cb8f23fcee225725b3fede95993108c92b9061c9e9`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472433ffd68a273b7d32b1483f7cd063212e7d8dab63fec46149bda5b1bd7012`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6aec6a6bafe0942f394cf46f8857811ba95bf92af292b58b37ef99635d59af`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.0-beta2`

```console
$ docker pull consul@sha256:0101ed8ed924388d203962c7f6cd00c64946a2915aa307ae6fdb77257f35afff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.0-beta2` - linux; amd64

```console
$ docker pull consul@sha256:e57b5bd1735f5669571dd93cb358dafcc1274e123f85ec9878f40ba0b506bf22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43713511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33a1fbcf9760adfc346281ab93087515248a09acd754cfa38ad65dd048a23e67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:57:45 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Fri, 12 Nov 2021 21:57:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 12 Nov 2021 21:57:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 12 Nov 2021 21:57:46 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 12 Nov 2021 21:58:02 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 12 Nov 2021 21:58:05 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 12 Nov 2021 21:58:07 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:58:07 GMT
VOLUME [/consul/data]
# Fri, 12 Nov 2021 21:58:08 GMT
EXPOSE 8300
# Fri, 12 Nov 2021 21:58:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 12 Nov 2021 21:58:09 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 12 Nov 2021 21:58:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 21:58:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 21:58:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9dd9907ca9dba4bf6d73592e3433bb41bfd6758f9fda5deee3ba72629b90c0`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ce0fdfb8f1545e60331c6ceb496bd4ff2cedab6c4e0533ab3d9c5132308624`  
		Last Modified: Fri, 12 Nov 2021 21:59:51 GMT  
		Size: 40.9 MB (40887721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c10085b0fae3b6f6041a1de3e35988aa036d8fd1e5a6f67aaff584f889545d`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99692da936ecbe3f732798a699a03861ea39fc25a2664db7e8fd96fa3a05b24c`  
		Last Modified: Fri, 12 Nov 2021 21:59:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e52fae0f8177dd8b49904fe878aaeabaa0eb44d2e78187ff1357a4e88eba7`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta2` - linux; arm variant v6

```console
$ docker pull consul@sha256:409f4b4355391f1bcc0b8bd49175b308adcc70ddca9bd5dc2dcb3977c5eb23aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39508868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2fcd863378dba6a3d8e0d211cb0030306cf1eeda473f430c45b66185d9f40dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:39 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 06:02:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:02:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:02:42 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:02:55 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:02:57 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:02:59 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:02:59 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:03:00 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:03:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:03:01 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:03:01 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:03:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:03:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2d7260b8a655c8d28c28f40ef7d386ecdf21ec4e683fca1ada03fb077990b1`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d05d8b05f792a5f378b768ab68755d34efcd88553097ba4c11fe6fd0a4fe9b7`  
		Last Modified: Sat, 13 Nov 2021 06:05:56 GMT  
		Size: 36.9 MB (36872153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4c08e221c3a9944278928e0d5a5349f02e20378f200537c7bc0abc72fc4c5b`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc684001062a2334874602425ae1f7f3321952ce632b97090c30715e183b3b6e`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5703c46ca3d761e767f57a57cc7a942a7fd182112bbb0067a92544c78775fec6`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:fb76a00c0c2adc167cd5c1aeca7241360b4a1aa891a892b0a78359a69e206a42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39287714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ebbfccc7daa528654052fa7daeffb5ebbd9e9e26102394b284b36249c55be2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:15:15 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 11:15:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 11:15:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 11:15:18 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 11:15:30 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 11:15:31 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 11:15:32 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:15:33 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 11:15:34 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 11:15:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 11:15:36 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 11:15:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 11:15:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:15:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144af28d402c6aa398c230374e0796f8b1bc72bc894128628950b7e9809cb014`  
		Last Modified: Sat, 13 Nov 2021 11:17:23 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f6468fc5c085fb9f1f7f5be01d4280e6d581d4c0288eb7c853d68b70f84189`  
		Last Modified: Sat, 13 Nov 2021 11:17:28 GMT  
		Size: 36.6 MB (36564764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910209e84ce7afdb47a37c422bb2f445b7a4c4475ad552485d2ee6266a607fc2`  
		Last Modified: Sat, 13 Nov 2021 11:17:23 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287bbf38f5b8c1472195d191f1bed4a366432659146c5082d51de5ea49d59678`  
		Last Modified: Sat, 13 Nov 2021 11:17:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c8e4ce91e5c66b30bdf7716289d2386f28e41ad88c5e9f5690556b9636dd05`  
		Last Modified: Sat, 13 Nov 2021 11:17:22 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta2` - linux; 386

```console
$ docker pull consul@sha256:c329aff5d47eba46e1f6992fbe91dcf9010d6f80005286be9155f965921e7975
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42543628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb87f43018f823068831b78d7e4d452fe84225256e1edaf0aa81e8387567bbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:18:29 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 06:18:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:18:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:18:31 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:18:45 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:18:46 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:18:47 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:18:47 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:18:47 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:18:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:18:48 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:18:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:18:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c847a2ae3f27130e208c92ba400b0bc215dfbd6e6dc859cd2e39ad3aa520a`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a3c64b15b1543034c6e04bb4f1ffb5db0907892bf0e51163848219a87482d`  
		Last Modified: Sat, 13 Nov 2021 06:20:24 GMT  
		Size: 39.7 MB (39711445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bfeef4b841e5af9bbff9cb8f23fcee225725b3fede95993108c92b9061c9e9`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472433ffd68a273b7d32b1483f7cd063212e7d8dab63fec46149bda5b1bd7012`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6aec6a6bafe0942f394cf46f8857811ba95bf92af292b58b37ef99635d59af`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:40658eb31adbc2907781809f4dd04eb5c0f618032a4ab3922606da1a3006f8fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:546d194b2fa656448e8b8dc8c82e14aa74df609b01cc1a7512a548d68c3a59a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47442415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:594e22f602fd253a4ccf65411b17591b42f00b3c73337ac7b600dc437ec0e1e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:59:08 GMT
ARG CONSUL_VERSION=1.8.16
# Fri, 12 Nov 2021 21:59:08 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 12 Nov 2021 21:59:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 12 Nov 2021 21:59:09 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 12 Nov 2021 21:59:22 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 12 Nov 2021 21:59:23 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 12 Nov 2021 21:59:24 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:59:24 GMT
VOLUME [/consul/data]
# Fri, 12 Nov 2021 21:59:25 GMT
EXPOSE 8300
# Fri, 12 Nov 2021 21:59:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 12 Nov 2021 21:59:25 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 12 Nov 2021 21:59:25 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 21:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 21:59:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf254dbeaa3fef95c5677f071ae3d345825fa845e6f4b5ed890c45f76871dfd`  
		Last Modified: Fri, 12 Nov 2021 22:00:37 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c95ea807a3d5777523ccb77a9277ec7e2aa1ab3739ff5cadde9a79db9a5179`  
		Last Modified: Fri, 12 Nov 2021 22:00:43 GMT  
		Size: 44.6 MB (44616621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b1a4a14828149fa5edc5044f90b651985c756dd381e637361fe837e055e236`  
		Last Modified: Fri, 12 Nov 2021 22:00:37 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651f3beee8b2a2a0a5fbef50eacae52d3d8b8e5f323a5ac23face007bfb8dba7`  
		Last Modified: Fri, 12 Nov 2021 22:00:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053af3dfc6f8374f6aec29ada8e523e370405df63219e60f9b6625f86a38e9e2`  
		Last Modified: Fri, 12 Nov 2021 22:00:37 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:4edfc14afdc0f37429cebb0dbe241231461df005386af7bd9c753623f98d5df2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42647095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d314364247bfbb6794e1fcebbf3f5d52a52a695123bc7872399cd62a0e48edf1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:04:25 GMT
ARG CONSUL_VERSION=1.8.16
# Sat, 13 Nov 2021 06:04:26 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:04:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:04:29 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:04:40 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:04:43 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:04:45 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:04:46 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:04:46 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:04:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:04:47 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:04:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:04:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:04:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf4ef515c98c7a84eb35f5f5720cd2828c46fa3cc928aaaa143ae8cf1e2f3b0`  
		Last Modified: Sat, 13 Nov 2021 06:07:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf2a49b395d46e338b5f9aa342bf8c5fed30384e74a4938eb77b32e43dd8658`  
		Last Modified: Sat, 13 Nov 2021 06:07:22 GMT  
		Size: 40.0 MB (40010378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd78246daf38720d3035adde8b92496db5795856ae20c1a2806df6ca2b557ad8`  
		Last Modified: Sat, 13 Nov 2021 06:07:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88374c41dbe010b7a63d28ae07dc13e2a768612e3c5beed3ef1ac6988bc1dd2`  
		Last Modified: Sat, 13 Nov 2021 06:07:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa636a5abd48d6a8dd0cec8c360d3c933de0b2416a11a621b79f7dd0360b74`  
		Last Modified: Sat, 13 Nov 2021 06:07:10 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:96501bd6b1f4a9098da11495dbb25fd01b8fee53996391e6df4302e065b808d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42839823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e5c748166a16a08d140df6244130ba958c4c90c5a370908e2ca19ae9ea887f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:16:40 GMT
ARG CONSUL_VERSION=1.8.16
# Sat, 13 Nov 2021 11:16:41 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 11:16:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 11:16:43 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 11:16:49 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 11:16:49 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 11:16:50 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:16:51 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 11:16:52 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 11:16:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 11:16:54 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 11:16:56 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 11:16:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:16:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e491289e1e0a27e735bdd7a474dbea5ee6f065e1b6e795418bfa24496c5349`  
		Last Modified: Sat, 13 Nov 2021 11:18:13 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500f73ec8c059633a9b25634986e7c0d97f7e4932fbcf52665b2b740e41fcb53`  
		Last Modified: Sat, 13 Nov 2021 11:18:19 GMT  
		Size: 40.1 MB (40116872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea4c578d4154ceb82c75b549635ed70f32b2bdf4c61080b2cdc52713335cd7c`  
		Last Modified: Sat, 13 Nov 2021 11:18:13 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa2b11a9bb900a8d6ec40528529c43c2b1664197c2a15dc583938596de7efa5`  
		Last Modified: Sat, 13 Nov 2021 11:18:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bcaffa0581f647d9b3e3d88d088d545811337431a97f68d6e315c05e4e17`  
		Last Modified: Sat, 13 Nov 2021 11:18:13 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:b5417e0c8383a779c8a901b4c03301e2419ebacd39241574bb000ec17f355cf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (46997597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3801dceae3828af9b3aceb1ce1074f927daf33acd795456a4589098baf43324f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:19:35 GMT
ARG CONSUL_VERSION=1.8.16
# Sat, 13 Nov 2021 06:19:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:19:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:19:36 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:19:44 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:19:45 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:19:46 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:19:46 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:19:47 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:19:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:19:47 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:19:47 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:19:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd997c8b6363c68575b61009e8ca5d1384341243dd890de5eeda3eb497f77bb`  
		Last Modified: Sat, 13 Nov 2021 06:21:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f76a08b1620e00334bdb461749243b6a43e767557e948b776d4672a08a4f137`  
		Last Modified: Sat, 13 Nov 2021 06:21:23 GMT  
		Size: 44.2 MB (44165418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f744f10f839222456505d1523f900e18b943259c3096857a2592395f77b084`  
		Last Modified: Sat, 13 Nov 2021 06:21:17 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e80487615705b444e547ffcd0bb3ea8aceca2dd68b6ceef1c3ab95347f16452`  
		Last Modified: Sat, 13 Nov 2021 06:21:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c137926072307d795ed8d9de2f02e6a20c9788cf901d3bb619ec49f20292439e`  
		Last Modified: Sat, 13 Nov 2021 06:21:17 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.17`

**does not exist** (yet?)

## `consul:1.9`

```console
$ docker pull consul@sha256:923ddd2643e00168053a95a9368dd3d6241e35d84e983dc2d7198e8ec4ccbaa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:d13741d433f3ee09978212eea3816f30d05bcee5eae19dbbec480770326c65df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45906650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8caacaa9c797a072acd2548987b06e63f13aeaf90d3e8b7745e6451f19d436c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:58:44 GMT
ARG CONSUL_VERSION=1.9.10
# Fri, 12 Nov 2021 21:58:44 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 12 Nov 2021 21:58:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 12 Nov 2021 21:58:46 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 12 Nov 2021 21:58:58 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 12 Nov 2021 21:58:59 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 12 Nov 2021 21:59:01 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:59:02 GMT
VOLUME [/consul/data]
# Fri, 12 Nov 2021 21:59:02 GMT
EXPOSE 8300
# Fri, 12 Nov 2021 21:59:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 12 Nov 2021 21:59:03 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 12 Nov 2021 21:59:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 21:59:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 21:59:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e2c1f7906065a4cd42e4d62b6b0bb1210343968bec2332b455f12275ad80c7`  
		Last Modified: Fri, 12 Nov 2021 22:00:20 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726648a6f1d4dfbdd112cdebd05f18100c5faa4393a314bd14be947e20de583f`  
		Last Modified: Fri, 12 Nov 2021 22:00:27 GMT  
		Size: 43.1 MB (43080860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb402eaf5bebb1aa06118318c62217955732df2610d038250b4320665cb28a60`  
		Last Modified: Fri, 12 Nov 2021 22:00:20 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a7593bd225039971e09dd20556347c1ef097f2d4ca4b61534b49dd04743715`  
		Last Modified: Fri, 12 Nov 2021 22:00:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe1eecc2c3ab6ff464433c7bcd422b6852761752b1569a34d24a7c35918b236`  
		Last Modified: Fri, 12 Nov 2021 22:00:20 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:68735b0af8ad58f5783892d9cd7a072367e3c5acc9841deff279771c6610ef52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41089948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:510575fe5907c1ea33f4f5381765bfa9f9e7d35967335233de5050651722bd71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:03:50 GMT
ARG CONSUL_VERSION=1.9.10
# Sat, 13 Nov 2021 06:03:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:03:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:03:54 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:04:05 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:04:07 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:04:10 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:04:10 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:04:11 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:04:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:04:12 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:04:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:04:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f2254d0cdcef69ac73640a6cc81362f1ef51b50d379756688f4812fcd571af`  
		Last Modified: Sat, 13 Nov 2021 06:06:44 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b99f6f7345bc41a816ddc999ed6e1200cdc60082abe484180bd44f1dd471172`  
		Last Modified: Sat, 13 Nov 2021 06:06:57 GMT  
		Size: 38.5 MB (38453237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa73ecab166d1aa41bbb57b7f8cdad4e68e22ea5ca6e27eb9e844ca2cdcc6b9`  
		Last Modified: Sat, 13 Nov 2021 06:06:44 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d112ea0b69b8c2f4cbad40bb296032d9e14b28179c046e7185c621264fb4026`  
		Last Modified: Sat, 13 Nov 2021 06:06:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e29fe5d164369c89b9a2d187450583c34069ecdf4cce4892d8514aab525592a`  
		Last Modified: Sat, 13 Nov 2021 06:06:44 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0625a3215b7cbf1a19eab5f8abe39208579e4b937d27d0eeb08687d4852756e3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41347096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99cf4eff9dc96149f3c68825831ea4ed45907c447932aef2c176a566b035639b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:16:09 GMT
ARG CONSUL_VERSION=1.9.10
# Sat, 13 Nov 2021 11:16:10 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 11:16:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 11:16:12 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 11:16:23 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 11:16:24 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 11:16:25 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:16:26 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 11:16:27 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 11:16:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 11:16:29 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 11:16:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 11:16:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:16:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d103d72fa4eb268a6f837f0785cdfda4307ac0376b71691da88f4db3136c0154`  
		Last Modified: Sat, 13 Nov 2021 11:17:57 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ecf5518a05936f8aafebc68040509889965fd914e880c2342c6e4451681f83`  
		Last Modified: Sat, 13 Nov 2021 11:18:02 GMT  
		Size: 38.6 MB (38624145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796e6e3bd876a22c282e2f7a80632d81e23ad500a8a553495036781c1893e9a9`  
		Last Modified: Sat, 13 Nov 2021 11:17:57 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdb3f2ca797e573a3f308efbc1344b4ce03245c147976ce7b6773ba2fcfd588`  
		Last Modified: Sat, 13 Nov 2021 11:17:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d915e69a6d5494c2e7d33767b0511e28c9e2a79c318b2bd63cff6c9bab734559`  
		Last Modified: Sat, 13 Nov 2021 11:17:57 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:55669dfe9f36283013fe5df4242a4018d0f867c48edbed31865846791264572b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45280360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67273333547d454a13e319b3d146cb12cfb8fe64a6744d026015afb23657d7f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:19:16 GMT
ARG CONSUL_VERSION=1.9.10
# Sat, 13 Nov 2021 06:19:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:19:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:19:17 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:19:25 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:19:26 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:19:27 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:19:27 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:19:28 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:19:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:19:28 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:19:28 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:19:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:19:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77ae2949f0c68422ea7eb3c79cdee4b8016a48f3c056625d981fda2126a4f92`  
		Last Modified: Sat, 13 Nov 2021 06:20:58 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333790003bf543bc1470abdabe948ff03bfc53fae887d0928559e96eaf0fac3f`  
		Last Modified: Sat, 13 Nov 2021 06:21:05 GMT  
		Size: 42.4 MB (42448180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c44e93225d9f849ee5d8490adcfd304fd24cc989d6637b07d32aa67c9d7a6d`  
		Last Modified: Sat, 13 Nov 2021 06:20:57 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a156e59d99bb9c6105ba227d4028a1add1fac8f08518475a70849a924c136a`  
		Last Modified: Sat, 13 Nov 2021 06:20:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59ca8eeaf0ca7d2fde65e0b7259bf8923ba973e6dfa858596c7ee50c019d736`  
		Last Modified: Sat, 13 Nov 2021 06:20:57 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.11`

**does not exist** (yet?)

## `consul:latest`

```console
$ docker pull consul@sha256:483b592fa76d734882cf7336df94a5bf6f9e808a78b1a1ba17002a2aaf80da46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:4fc771d6614f6d7af92653e006157b9c98a05098e43dc485d29d9c846abcc33d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43242800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9814b25e52bae10d44d9953bad57d86e8577283652bc9443be9738031389c48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:58:14 GMT
ARG CONSUL_VERSION=1.10.3
# Fri, 12 Nov 2021 21:58:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 12 Nov 2021 21:58:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 12 Nov 2021 21:58:17 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 12 Nov 2021 21:58:30 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 12 Nov 2021 21:58:32 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 12 Nov 2021 21:58:35 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:58:35 GMT
VOLUME [/consul/data]
# Fri, 12 Nov 2021 21:58:36 GMT
EXPOSE 8300
# Fri, 12 Nov 2021 21:58:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 12 Nov 2021 21:58:36 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 12 Nov 2021 21:58:37 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 21:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 21:58:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79efaa79e0b89d613b7eeb02676f2c706bf77bac920e8657f0f9badfb6205340`  
		Last Modified: Fri, 12 Nov 2021 22:00:01 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b6fccdd38073e2a0303fb7450154fb88dd5211f8abbd8ab1b55e2514a24cb1`  
		Last Modified: Fri, 12 Nov 2021 22:00:07 GMT  
		Size: 40.4 MB (40417007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a1a23e6dad553737585a3b60948d19896dd3c8aeb3ec7e62e0bf03560f416e`  
		Last Modified: Fri, 12 Nov 2021 22:00:01 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae16349669345cc0fb16abc18cd48c1dbf94910caaee5431326c3cf34882559`  
		Last Modified: Fri, 12 Nov 2021 22:00:01 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fa79365c2a7793d97996a84e1a8e28dec95f530224a746f6d4cdca6dfe5f73`  
		Last Modified: Fri, 12 Nov 2021 22:00:01 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:89cd92136a7b8ebd035cb1a0e39b8e96abc49edf60c9200a27f117054b53932c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39269139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd4b0d9415b5a09650d466ee78ea76f2f5f821de5e796590f9339aa0c50e30b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:03:14 GMT
ARG CONSUL_VERSION=1.10.3
# Sat, 13 Nov 2021 06:03:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:03:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:03:17 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:03:29 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:03:31 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:03:33 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:03:34 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:03:34 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:03:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:03:35 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:03:36 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:03:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:03:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95e092b4de70f76b87ef5e2952153af28de56b56c428d170b0f028fb6afbf1d`  
		Last Modified: Sat, 13 Nov 2021 06:06:08 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598923641df439f939be74ba7dc244ef98d48641e316ff947702b24a279c956d`  
		Last Modified: Sat, 13 Nov 2021 06:06:27 GMT  
		Size: 36.6 MB (36632428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b856a08c888ad010360a1dd58e1196cab9d0a174889c005fd0dd1c23a5225c4`  
		Last Modified: Sat, 13 Nov 2021 06:06:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde4ced118232a40da2c756413e2ca1148a45efc645d9f750f232a1dcd7f945f`  
		Last Modified: Sat, 13 Nov 2021 06:06:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e826ae63c559c7b16801bd6e94f70546fbf8739bbb8a33eae3edd323fd2797b7`  
		Last Modified: Sat, 13 Nov 2021 06:06:08 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:49806d20f5bec7cfebaee85b402e0507ecaee84d21875b1666dd145595e76bb9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39197224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79533321836233fbf353f989f599b83489cf6bf766b81ca69b63c2aa78807d37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:15:46 GMT
ARG CONSUL_VERSION=1.10.3
# Sat, 13 Nov 2021 11:15:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 11:15:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 11:15:49 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 11:15:55 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 11:15:55 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 11:15:56 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:15:57 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 11:15:58 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 11:15:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 11:16:00 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 11:16:02 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 11:16:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:16:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af37d8c363d19fa997a18af0e4843fd2f676bb004307d4ad3871b967db1ad181`  
		Last Modified: Sat, 13 Nov 2021 11:17:38 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48713568c234663e5570c3039860b7e2b9be32f1d1044864c25d61fb19a20546`  
		Last Modified: Sat, 13 Nov 2021 11:17:43 GMT  
		Size: 36.5 MB (36474278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2aae487100b5ebe714e5b1f05e968449c0486d160860f20cd3fbc0013dd656`  
		Last Modified: Sat, 13 Nov 2021 11:17:38 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95de985c0b90328a625f0a5932f1f05f0978332a73572d2e3046a7b723882d2`  
		Last Modified: Sat, 13 Nov 2021 11:17:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474b8a1f74bc7aebca99d417b6bff154a2ab0d345ff227d3b1a32d89e781065`  
		Last Modified: Sat, 13 Nov 2021 11:17:38 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:f6d4990606abae58cfa07041438a83774585b1976889aa17ecfb69c10582149d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42624588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0266e05a345c091de13c2cf497e8d5c997539a31384988e30a540f6338d8e095`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:18:54 GMT
ARG CONSUL_VERSION=1.10.3
# Sat, 13 Nov 2021 06:18:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:18:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:18:56 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:19:06 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:19:07 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:19:08 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:19:08 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:19:08 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:19:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:19:09 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:19:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:19:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:19:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ad71c51a3aaa36ca93ff2d29be265437f8d6a6a3265229463a32d757ab063c`  
		Last Modified: Sat, 13 Nov 2021 06:20:36 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264e1a84ec19e245b5b17560ae89a7a20d673c5065b8e31ad33e1dec79c3a5fc`  
		Last Modified: Sat, 13 Nov 2021 06:20:42 GMT  
		Size: 39.8 MB (39792406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52249b1ddd029a0a2974e3e28a7d4ba4eb74ba1428eba364aab8c0634680193`  
		Last Modified: Sat, 13 Nov 2021 06:20:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e3c995ef13035d9e1361df724e4dbb2f695c7fdf5a1a5dac866ececfd2f54`  
		Last Modified: Sat, 13 Nov 2021 06:20:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefa7778ca9c4c1248a35f60f616d57440c6dda91f0b4afcbf7b464258fa72cf`  
		Last Modified: Sat, 13 Nov 2021 06:20:36 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
