## `consul:latest`

```console
$ docker pull consul@sha256:c7ac5b7a23cab94ce207da2722fe37666d6d31dd0de585798149f92a1bd59628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:0e1bf46d11fc1206b823adee771d4a828c1e43ffbc61eb0f3bd1b9c4c2e9555c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45660975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28efe5fcc0492ee7af47f817357211e3e0e079d76d208f83fb67190fc1005c24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 20:14:28 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 20:14:29 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 20:14:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 20:14:30 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 20:14:35 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 20:14:37 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 20:14:39 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:14:39 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 20:14:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 20:14:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:14:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6f7401278b6047ca51b04eaa48718d1ad2217d17cfa7aacd0f88cd75087ef`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42903c65e0ffb2011b9dd5455c10767b28d080882f7b5e147dfcdae436589415`  
		Last Modified: Wed, 14 Apr 2021 20:16:02 GMT  
		Size: 42.9 MB (42857116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7545c107e7a73790423708f86188c0f57b1f3047db4b363546f26dbf95b752d`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f837edf7afc74be22f4b914b3e9050371bcab6111de42aaf802c2711006836d`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959978e907f3ffccec3ec6bcc1486bba7e9431b596593b89ed84b472ec89e27`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:57f0b9e1d87c0a5ef6946bbd6a1767d1630d5f3e238cd84e04312dbbb0472084
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40911088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d290d4e40b5f15fcadae2f208f0d12a0b2b75c21b0202d4ee126628c3e50db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:48:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:48:51 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 19:48:52 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 19:48:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:48:59 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:50:03 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:50:07 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:50:10 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:50:10 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:50:11 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:50:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:50:13 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:50:13 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:50:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:50:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab416f4b1ee1c7c4f0f327a9548c6fa41fc8b61b7ff80bb072ab5eafbfe81aa`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f9bff852385f80d92506250cb34641498caaf3ce2ce6774bdeb80d5fa1611f`  
		Last Modified: Wed, 14 Apr 2021 19:52:13 GMT  
		Size: 38.3 MB (38302542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45821997bb09bd9c2430bf007cca645d38ae22f9cd53c846f84f8ed54f70aa64`  
		Last Modified: Wed, 14 Apr 2021 19:52:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53516a4fc57619782eda8f42b4918106984adb2bdabaca7b3f7c1c0a65eeb0`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c919202793e92b538f208f3ee0e5f7e92e03111769f68f8ab0d94438916bca41`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:794c24fbbd979bf5af6af9630d7d9325aa6f01f668f4bca857204c5994c54b3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41126204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a825e2fced0b53948b4f9e7bfc5d1609481cc108c2d60c1c6fd96b2643c9736a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:22:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:22:51 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 19:22:52 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 19:22:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:22:56 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:23:03 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:23:06 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:23:09 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:23:10 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:23:11 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:23:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:23:13 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:23:14 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:23:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:23:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b96788e82b6af129f934f44e3be6e11bd50c5aa4aa7f153d5c23ccb0dc12cf`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:face225286cec8239bf7c33e3977ca020cbc18e6b8cd3865c520feb00357f466`  
		Last Modified: Wed, 14 Apr 2021 19:24:57 GMT  
		Size: 38.4 MB (38412219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fb33ef170a52b1969e77c98378e9677623a19a6c6c17b581a3b345a3f9d387`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3befdfcaca0963f39f847c37604e9867e38aaca2fa8bbfde33c3515e22ec18`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b246d545ee670f4fd4a8233c1a1fb4233cba1d92c226cf5fad4566571d125075`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:f7b2894fa2b2cce628874cb34c141e154a36af139a2ce7cf8ea879057ec1f36a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44978347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e6b7fa39b52e886a1bcecc2e7cca9076c09427848558ee7631e8b5a9a924e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 18:55:36 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 18:55:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 18:55:37 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 18:55:44 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 18:55:45 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 18:55:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 18:55:46 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 18:55:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 18:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 18:55:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3831ff37459cebceaf36d2175d922fea9abe8aa2d956f29596fcce2b12cc90d`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf5d944668f1ce4efe25c8da04427ff173e57ba09ae72f16313fe5fd01d77b`  
		Last Modified: Wed, 14 Apr 2021 18:56:48 GMT  
		Size: 42.2 MB (42179261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f75e489a23c08e7c8d80a390517626ae20d9bc1900e38f640c3ceb3c452289`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9108803843267de412c0c6aa141a1d17bc55047f1b59d3602ce336005d6a81`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77f9b370fadecaa06e11cd41a1054987b24cf57a0b49c6b4d3f1c4a64928e40`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
