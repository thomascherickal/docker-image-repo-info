<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.12`](#logstash71712)
-	[`logstash:8.9.1`](#logstash891)

## `logstash:7.17.12`

```console
$ docker pull logstash@sha256:2fd41b546f9577408c8d48220521ab567ae1901d0d0a1eeffd30b2cc9f5d3918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.12` - linux; amd64

```console
$ docker pull logstash@sha256:7ee30dead16a7399ff8ebb74aa7980de7d0a18a03944b6dca574b1f8562dcd97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.8 MB (440800786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5b22368b89f6663d1717846f2515e63c84a4e62d22eca2ad47d39aeebbc8ae`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 10:38:07 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 18 Jul 2023 10:38:07 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.12-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.12 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
WORKDIR /usr/share/logstash
# Tue, 18 Jul 2023 10:38:23 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 18 Jul 2023 10:38:23 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Jul 2023 10:38:23 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ADD config/log4j2.properties config/ # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 18 Jul 2023 10:38:23 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
USER 1000
# Tue, 18 Jul 2023 10:38:23 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 18 Jul 2023 10:38:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.12 org.opencontainers.image.version=7.17.12 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-07-18T10:23:11+00:00 org.opencontainers.image.created=2023-07-18T10:23:11+00:00
# Tue, 18 Jul 2023 10:38:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1252d9f3b297e5c3c6f7a6b1052bb8c4774203031e96ec19e180a66ae7b61c3`  
		Last Modified: Thu, 03 Aug 2023 07:24:58 GMT  
		Size: 43.9 MB (43942679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e999dd0a3d26da5c89e4b7cfd15b74f31062e90ae64b9242a3d66dc71585c9`  
		Last Modified: Thu, 03 Aug 2023 07:24:48 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e09a86198b4c2e0ac06fb4cfe12e77ab8a68aa2a48cd37781406521faa6bca`  
		Last Modified: Thu, 03 Aug 2023 07:25:21 GMT  
		Size: 366.5 MB (366458608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2926ddeca1dc60e7ab1599046df086177ac00bee5d78cc1f065e03aafc2e657`  
		Last Modified: Thu, 03 Aug 2023 07:24:47 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94275b63b2f4e420a003e8de4e445d7df4fdf37d1510f64de3cccc17c6f9ab88`  
		Last Modified: Thu, 03 Aug 2023 07:24:47 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1555d37737bb0ecb1a0f5bbfac985e9b32c02dd5d0d4802ee7bed408818bcb0e`  
		Last Modified: Thu, 03 Aug 2023 07:24:41 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01e2f66b7c97d64dae2561b516ead6a0b4d6359e2a704539d4998e27622b5af`  
		Last Modified: Thu, 03 Aug 2023 07:24:41 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9bf571b75c9ad6eb46d9061a6dcd341403fbb9b2e8a0a70a172388c7a0d5d`  
		Last Modified: Thu, 03 Aug 2023 07:24:41 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee26d382606e60f1e0768a3b889cdb3b6413c3c55b3abad3747290da35c618`  
		Last Modified: Thu, 03 Aug 2023 07:24:43 GMT  
		Size: 1.8 MB (1812378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7ff156fedab31f1acf57892cc8d66c9503acb37e662386bc7f06ed75d19279`  
		Last Modified: Thu, 03 Aug 2023 07:24:42 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7ff156fedab31f1acf57892cc8d66c9503acb37e662386bc7f06ed75d19279`  
		Last Modified: Thu, 03 Aug 2023 07:24:42 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.12` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:d70a822a314243d0ba3f1ecb557c06e65bec667324d6f11faaf203ea019a59d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.9 MB (427949674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a1e5828f0eeffbfb3bfe2704646d23ac468b82bb1dd44627ae3c81a32da4e4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 10:37:27 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 18 Jul 2023 10:37:27 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.12-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.12 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
WORKDIR /usr/share/logstash
# Tue, 18 Jul 2023 10:37:38 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 18 Jul 2023 10:37:38 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Jul 2023 10:37:38 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
ADD config/log4j2.properties config/ # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 18 Jul 2023 10:37:39 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 10:37:39 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 10:37:39 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 18 Jul 2023 10:37:39 GMT
USER 1000
# Tue, 18 Jul 2023 10:37:39 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 18 Jul 2023 10:37:39 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.12 org.opencontainers.image.version=7.17.12 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-07-18T10:24:54+00:00 org.opencontainers.image.created=2023-07-18T10:24:54+00:00
# Tue, 18 Jul 2023 10:37:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f656e2e146169db0197119b3cfff78c553a228761fdf62d4b88d4d088a1290`  
		Last Modified: Wed, 23 Aug 2023 23:49:34 GMT  
		Size: 35.8 MB (35824273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed7b6342b1c5d17a38bda4d4872243564a3e920da950553dcfd1ba0a6450e0d`  
		Last Modified: Wed, 23 Aug 2023 23:49:30 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cad957d9dc297ba08b75d3341facce9f9e16426996b56bb3c0855831bfdf6e6`  
		Last Modified: Wed, 23 Aug 2023 23:49:51 GMT  
		Size: 363.2 MB (363227400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d2a71cf994720643a08bb67a56a8105ea88ec156f5e282c74bf770e47ee924`  
		Last Modified: Wed, 23 Aug 2023 23:49:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5238d7e910b0e8042c04ae6c4d879bb2802b01f7aab6722af443b1d7dabd99`  
		Last Modified: Wed, 23 Aug 2023 23:49:30 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba297f4b40223b8fdad514908eda5ea58d1cdedad45287ce461621292f065f32`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0560c0b3ce97853c8bf46909e51b1a1df082ec80fa578088334f6053ed0720f8`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 301.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0081570ecad3a57b2a9489baeea7251820b2a3e0e6ab115413f4b996416e2036`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 2.8 KB (2849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f281dde0d67cb6236f4e8813495726c0e06086f0eb8a0da881a890a7de52b0d`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 1.7 MB (1692529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d0cb7d2cae30387d1717267cdcfd8fd096cd47c23b86a3a5ca2d88ef0172da`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d0cb7d2cae30387d1717267cdcfd8fd096cd47c23b86a3a5ca2d88ef0172da`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.9.1`

```console
$ docker pull logstash@sha256:0bb447991e28a292f628e8d2d8348aa7bf04b1b4c15420e757ff4082976b1894
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.9.1` - linux; amd64

```console
$ docker pull logstash@sha256:c6426f31ecd51af6f42d09e1e0fa06a659876cda6e82d30dced4c57aac3385e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.8 MB (423846956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6936c50aa9f5575bda6355a4483442bb93564ab579e1c41eb1061d39e6f291f2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Wed, 09 Aug 2023 09:33:59 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 09 Aug 2023 09:34:00 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.9.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.9.1 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
WORKDIR /usr/share/logstash
# Wed, 09 Aug 2023 09:34:15 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 09 Aug 2023 09:34:15 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 09:34:15 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
COPY config/log4j2.properties config/ # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 09 Aug 2023 09:34:16 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
USER 1000
# Wed, 09 Aug 2023 09:34:16 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 09 Aug 2023 09:34:16 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.9.1 org.opencontainers.image.version=8.9.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-08-09T09:16:22+00:00 org.opencontainers.image.created=2023-08-09T09:16:22+00:00
# Wed, 09 Aug 2023 09:34:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5359ae0673f6465c56eef216725f93611ccbd885a57a2e45db4327b6e2d299`  
		Last Modified: Mon, 21 Aug 2023 01:12:58 GMT  
		Size: 44.2 MB (44199436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db56260ef5189b04b8bc545509160efe39418817da141051932c823f11658b41`  
		Last Modified: Mon, 21 Aug 2023 01:12:42 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775fc9f3b712d34a2e72897f65c9eb64a2a8e6760704ed92061a61f310747714`  
		Last Modified: Mon, 21 Aug 2023 01:14:26 GMT  
		Size: 349.2 MB (349211378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eacb679e6c68b4a6f96c0301bbf6707ae5b40cb09bd49429e593b3e937c573`  
		Last Modified: Mon, 21 Aug 2023 01:12:39 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371c474647f3a9e7999594e7027ab6775dcf8f036afa02c4a3d765cb64e10502`  
		Last Modified: Mon, 21 Aug 2023 01:12:37 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d330bd7cfeed9bcd7ac5a551003f84ec670d9f200e27e84b95afaecf9efd6e1`  
		Last Modified: Mon, 21 Aug 2023 01:12:37 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b9fdbb7215070b6f1da81f59b564195f2e8eb52c31660b36b29736e10ce223`  
		Last Modified: Mon, 21 Aug 2023 01:12:33 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0ff13c9e7e53683a04815aa2aba5ee38326492dc85111b86fdb03e82ec5475`  
		Last Modified: Mon, 21 Aug 2023 01:12:32 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676641b254abdc3e180c98dae3023debeb83f2f0f895f00d6bd402c15062ccb6`  
		Last Modified: Mon, 21 Aug 2023 01:12:32 GMT  
		Size: 3.7 KB (3658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2084757ec44b4717016898ddfa1b87fac148998c34d61062ff6c4102b1f6c7`  
		Last Modified: Mon, 21 Aug 2023 01:12:34 GMT  
		Size: 1.8 MB (1845755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e194c1340f610d95bfa4e2674a249a7ca7da20def3b0999101a940c18f9ea4b`  
		Last Modified: Mon, 21 Aug 2023 01:12:29 GMT  
		Size: 713.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e194c1340f610d95bfa4e2674a249a7ca7da20def3b0999101a940c18f9ea4b`  
		Last Modified: Mon, 21 Aug 2023 01:12:29 GMT  
		Size: 713.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.9.1` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:f05007232cbea8260b19985dc93f678d6df21f6573425f3189b69c8cfc3f527f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.9 MB (412878009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35359e0ff01a56a25d15b2a07eb80f539804b59228f2044974c60c0682a17c41`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 09 Aug 2023 09:33:45 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 09 Aug 2023 09:33:46 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.9.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.9.1 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
WORKDIR /usr/share/logstash
# Wed, 09 Aug 2023 09:33:57 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 09 Aug 2023 09:33:57 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 09:33:57 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY config/log4j2.properties config/ # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 09 Aug 2023 09:33:57 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 09 Aug 2023 09:33:58 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 09 Aug 2023 09:33:58 GMT
USER 1000
# Wed, 09 Aug 2023 09:33:58 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 09 Aug 2023 09:33:58 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.9.1 org.opencontainers.image.version=8.9.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-08-09T09:18:39+00:00 org.opencontainers.image.created=2023-08-09T09:18:39+00:00
# Wed, 09 Aug 2023 09:33:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f56f1fc0d4f5cceae94a8523ca467ed142176439825de68c798e80192e565`  
		Last Modified: Wed, 23 Aug 2023 23:49:05 GMT  
		Size: 35.9 MB (35932005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8e875a123e6aa7ec6ac07589c20ef9db6fe2ae7c22d1e4023e494dbb6fb817`  
		Last Modified: Wed, 23 Aug 2023 23:49:00 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add229aa6531457e942490d0c9641318aad1be6f4e3e105159a8d329c862656c`  
		Last Modified: Wed, 23 Aug 2023 23:49:21 GMT  
		Size: 348.0 MB (348003915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e855164e968b4367c4c4520a17314de145b5fa341388d77e275fbb707a0d45eb`  
		Last Modified: Wed, 23 Aug 2023 23:48:59 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4ff0af73d95373ad3d295cf48a86d7b9149ee050e6a1d235d64ad3c84c659d`  
		Last Modified: Wed, 23 Aug 2023 23:48:59 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122591da54f2a672df995488e8ce0f44d3520f39f6ab06047bc9ffd3b648c8f8`  
		Last Modified: Wed, 23 Aug 2023 23:48:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a536cfd44c31fb9c2e7015ace6b05bdecc5a283178b849ddf44a062d7e7afb3d`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7665b9b744acfb88017f4c5f9a9a40eaf20fe07989549cfc32d9fc631498239c`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf44f9ce281a1091f5f597c047ab5bcca248833a9907cc921f18b2e879cfb06c`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 3.7 KB (3663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6ee346489fef9a8fbbff680574d521c63615e1e234f022f0214abe781c9452`  
		Last Modified: Wed, 23 Aug 2023 23:48:58 GMT  
		Size: 1.7 MB (1731755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67393b314f805c926ccd95d69053134780f725a101a7c19d5e504c7ad4fa228a`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67393b314f805c926ccd95d69053134780f725a101a7c19d5e504c7ad4fa228a`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
