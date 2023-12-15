<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.28`](#neo4j4428)
-	[`neo4j:4.4.28-community`](#neo4j4428-community)
-	[`neo4j:4.4.28-enterprise`](#neo4j4428-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-bullseye`](#neo4j5-bullseye)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-community-bullseye`](#neo4j5-community-bullseye)
-	[`neo4j:5-community-ubi8`](#neo4j5-community-ubi8)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5-enterprise-bullseye`](#neo4j5-enterprise-bullseye)
-	[`neo4j:5-enterprise-ubi8`](#neo4j5-enterprise-ubi8)
-	[`neo4j:5-ubi8`](#neo4j5-ubi8)
-	[`neo4j:5.15`](#neo4j515)
-	[`neo4j:5.15-bullseye`](#neo4j515-bullseye)
-	[`neo4j:5.15-community`](#neo4j515-community)
-	[`neo4j:5.15-community-bullseye`](#neo4j515-community-bullseye)
-	[`neo4j:5.15-community-ubi8`](#neo4j515-community-ubi8)
-	[`neo4j:5.15-enterprise`](#neo4j515-enterprise)
-	[`neo4j:5.15-enterprise-bullseye`](#neo4j515-enterprise-bullseye)
-	[`neo4j:5.15-enterprise-ubi8`](#neo4j515-enterprise-ubi8)
-	[`neo4j:5.15-ubi8`](#neo4j515-ubi8)
-	[`neo4j:5.15.0`](#neo4j5150)
-	[`neo4j:5.15.0-bullseye`](#neo4j5150-bullseye)
-	[`neo4j:5.15.0-community`](#neo4j5150-community)
-	[`neo4j:5.15.0-community-bullseye`](#neo4j5150-community-bullseye)
-	[`neo4j:5.15.0-community-ubi8`](#neo4j5150-community-ubi8)
-	[`neo4j:5.15.0-enterprise`](#neo4j5150-enterprise)
-	[`neo4j:5.15.0-enterprise-bullseye`](#neo4j5150-enterprise-bullseye)
-	[`neo4j:5.15.0-enterprise-ubi8`](#neo4j5150-enterprise-ubi8)
-	[`neo4j:5.15.0-ubi8`](#neo4j5150-ubi8)
-	[`neo4j:bullseye`](#neo4jbullseye)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:community-bullseye`](#neo4jcommunity-bullseye)
-	[`neo4j:community-ubi8`](#neo4jcommunity-ubi8)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:enterprise-bullseye`](#neo4jenterprise-bullseye)
-	[`neo4j:enterprise-ubi8`](#neo4jenterprise-ubi8)
-	[`neo4j:latest`](#neo4jlatest)
-	[`neo4j:ubi8`](#neo4jubi8)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:58821a9b6f2be798782ea9b92affbac926647688ab9a1d727bada80132de93a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:0cc2304afc87557e0adac8154f9f7dd97db179fa4de2f9606c4fa1100e6bea4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297351612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92605d7d706ad3b955b9f6cc5eb676a69edc9c265430a967de9acad2100c1965`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:39:06 GMT
COPY dir:d20aeb749bf0b3fe533952f7903b6aa08724fe8bf03e369130d4e2a6ff71bd3f in /opt/java/openjdk 
# Sat, 02 Dec 2023 07:39:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f00e23cf063836a6c39fe0baef42f7ade86d7a096548dcccb4620aa0e1a2a6a NEO4J_TARBALL=neo4j-community-4.4.28-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 07:39:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 07:39:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 07:39:09 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 07:39:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 07:39:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:39:38 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 07:39:38 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 07:39:38 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 07:39:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:39:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e28bbb7ed8d446eab9126cf70b8a8696a1b2c97ace981f72b9e7fa4a8fa7e1`  
		Last Modified: Sat, 02 Dec 2023 07:43:21 GMT  
		Size: 145.3 MB (145266435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0609e7d73a5c1db314d18988189cf0542c93b2b5b3fad6064837df9fcc70f00a`  
		Last Modified: Sat, 02 Dec 2023 07:43:09 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbd2488daaa37df4a60545b9d2c8f0eaffb97cd04e4409a0e0bd232cb1546fe`  
		Last Modified: Sat, 02 Dec 2023 07:43:09 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20b7755b77acacf6b35dc48bbffc1537c8ca86e3a1f1d1825a8c7caacb23045`  
		Last Modified: Sat, 02 Dec 2023 07:43:15 GMT  
		Size: 120.7 MB (120654077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:d5a6c165f8c5441441634400b01c301d1e8c2747577f32e7fa29e3f3e4fa942c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292699562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32c762fcddaa1dd67bdd1ccf8f300900298434a55c572fc796856acfa2ba55c3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:45:58 GMT
COPY dir:201fdbb3aef6b177b9038d3dd5bbe865568281c78c7bc0c153b57943d571a0b6 in /opt/java/openjdk 
# Sat, 02 Dec 2023 11:55:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f00e23cf063836a6c39fe0baef42f7ade86d7a096548dcccb4620aa0e1a2a6a NEO4J_TARBALL=neo4j-community-4.4.28-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 11:55:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 11:55:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 11:55:09 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 11:55:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 11:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 11:55:36 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 11:55:36 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 11:55:36 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 11:55:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 11:55:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c9736680f80d26b6300f944e7ba80ac7f1a756c950bdf599346e7954ad2dff`  
		Last Modified: Sat, 02 Dec 2023 09:04:30 GMT  
		Size: 142.0 MB (142001789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0052c0ee1539da703ca76e0b52e164012b1a23b80865d07784a2dbf00164ea`  
		Last Modified: Sat, 02 Dec 2023 11:58:41 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53da938b15194a167297081c5683008de76f1c926337793487f93995a74ccf11`  
		Last Modified: Sat, 02 Dec 2023 11:58:41 GMT  
		Size: 9.4 KB (9418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e244f831fb37ad9fd4cf1c9aeddf80c67dc937ea40b5935a244e7757ec8b98`  
		Last Modified: Sat, 02 Dec 2023 11:58:46 GMT  
		Size: 120.6 MB (120620349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:58821a9b6f2be798782ea9b92affbac926647688ab9a1d727bada80132de93a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:0cc2304afc87557e0adac8154f9f7dd97db179fa4de2f9606c4fa1100e6bea4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297351612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92605d7d706ad3b955b9f6cc5eb676a69edc9c265430a967de9acad2100c1965`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:39:06 GMT
COPY dir:d20aeb749bf0b3fe533952f7903b6aa08724fe8bf03e369130d4e2a6ff71bd3f in /opt/java/openjdk 
# Sat, 02 Dec 2023 07:39:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f00e23cf063836a6c39fe0baef42f7ade86d7a096548dcccb4620aa0e1a2a6a NEO4J_TARBALL=neo4j-community-4.4.28-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 07:39:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 07:39:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 07:39:09 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 07:39:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 07:39:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:39:38 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 07:39:38 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 07:39:38 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 07:39:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:39:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e28bbb7ed8d446eab9126cf70b8a8696a1b2c97ace981f72b9e7fa4a8fa7e1`  
		Last Modified: Sat, 02 Dec 2023 07:43:21 GMT  
		Size: 145.3 MB (145266435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0609e7d73a5c1db314d18988189cf0542c93b2b5b3fad6064837df9fcc70f00a`  
		Last Modified: Sat, 02 Dec 2023 07:43:09 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbd2488daaa37df4a60545b9d2c8f0eaffb97cd04e4409a0e0bd232cb1546fe`  
		Last Modified: Sat, 02 Dec 2023 07:43:09 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20b7755b77acacf6b35dc48bbffc1537c8ca86e3a1f1d1825a8c7caacb23045`  
		Last Modified: Sat, 02 Dec 2023 07:43:15 GMT  
		Size: 120.7 MB (120654077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:d5a6c165f8c5441441634400b01c301d1e8c2747577f32e7fa29e3f3e4fa942c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292699562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32c762fcddaa1dd67bdd1ccf8f300900298434a55c572fc796856acfa2ba55c3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:45:58 GMT
COPY dir:201fdbb3aef6b177b9038d3dd5bbe865568281c78c7bc0c153b57943d571a0b6 in /opt/java/openjdk 
# Sat, 02 Dec 2023 11:55:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f00e23cf063836a6c39fe0baef42f7ade86d7a096548dcccb4620aa0e1a2a6a NEO4J_TARBALL=neo4j-community-4.4.28-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 11:55:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 11:55:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 11:55:09 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 11:55:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 11:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 11:55:36 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 11:55:36 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 11:55:36 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 11:55:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 11:55:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c9736680f80d26b6300f944e7ba80ac7f1a756c950bdf599346e7954ad2dff`  
		Last Modified: Sat, 02 Dec 2023 09:04:30 GMT  
		Size: 142.0 MB (142001789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0052c0ee1539da703ca76e0b52e164012b1a23b80865d07784a2dbf00164ea`  
		Last Modified: Sat, 02 Dec 2023 11:58:41 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53da938b15194a167297081c5683008de76f1c926337793487f93995a74ccf11`  
		Last Modified: Sat, 02 Dec 2023 11:58:41 GMT  
		Size: 9.4 KB (9418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e244f831fb37ad9fd4cf1c9aeddf80c67dc937ea40b5935a244e7757ec8b98`  
		Last Modified: Sat, 02 Dec 2023 11:58:46 GMT  
		Size: 120.6 MB (120620349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:22a8909b929765b92558c40f6ea7717e9145017d54984e790a5231769587d50b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:95047e3c76d3481d3728bca1f30fe4221fb36da69d13c40f15997aa1fff968bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.9 MB (401907379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0849facd0a7645b7f70420e538ba34451812115a7be15a83369dc49779a0e728`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:39:06 GMT
COPY dir:d20aeb749bf0b3fe533952f7903b6aa08724fe8bf03e369130d4e2a6ff71bd3f in /opt/java/openjdk 
# Sat, 02 Dec 2023 07:39:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=57dab47060e05c353c0c6741d9bbd0b8bc05677e5c5e16592ebdaf1ec90b1678 NEO4J_TARBALL=neo4j-enterprise-4.4.28-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 07:39:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 07:39:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 07:39:45 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 07:40:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 07:40:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:40:21 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 07:40:21 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 07:40:21 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 07:40:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:40:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e28bbb7ed8d446eab9126cf70b8a8696a1b2c97ace981f72b9e7fa4a8fa7e1`  
		Last Modified: Sat, 02 Dec 2023 07:43:21 GMT  
		Size: 145.3 MB (145266435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defc888d987870a51f472b728fd09b7235ee48e4bd61871c14aae8eee642bbce`  
		Last Modified: Sat, 02 Dec 2023 07:43:33 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df57ee89926a2202b735f6116042a537af3272578bdbabdfb1f22b291e372546`  
		Last Modified: Sat, 02 Dec 2023 07:43:33 GMT  
		Size: 9.4 KB (9415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4778b5c7eefb485b3983316f5612bc946ca41ade136936eb81e1c8fa08182d2c`  
		Last Modified: Sat, 02 Dec 2023 07:43:42 GMT  
		Size: 225.2 MB (225209847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:02e9296a7db24d8e30960f52cd134b2a25e289e6f738a0e9d3beca22c6917f25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.3 MB (397252348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42df89dcc0eb7a9e9748bb59ef476c82cd6eb8b19c918e10269900711da9c1a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:45:58 GMT
COPY dir:201fdbb3aef6b177b9038d3dd5bbe865568281c78c7bc0c153b57943d571a0b6 in /opt/java/openjdk 
# Sat, 02 Dec 2023 11:55:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=57dab47060e05c353c0c6741d9bbd0b8bc05677e5c5e16592ebdaf1ec90b1678 NEO4J_TARBALL=neo4j-enterprise-4.4.28-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 11:55:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 11:55:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 11:55:43 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 11:56:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 11:56:08 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 11:56:08 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 11:56:08 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 11:56:08 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 11:56:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 11:56:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c9736680f80d26b6300f944e7ba80ac7f1a756c950bdf599346e7954ad2dff`  
		Last Modified: Sat, 02 Dec 2023 09:04:30 GMT  
		Size: 142.0 MB (142001789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf5642a1b8a5b80fbfdde4a35694e65df68820097bab5700262a1654ef1248e`  
		Last Modified: Sat, 02 Dec 2023 11:58:58 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f250da6740af78797be267bd6077033ffdbd37599bf9e285705ed2a633d1072c`  
		Last Modified: Sat, 02 Dec 2023 11:58:59 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77b2f4763eceb909f9aeb3cb0733d1818c64fe5bf1802e1564c617e0d9678cf`  
		Last Modified: Sat, 02 Dec 2023 11:59:07 GMT  
		Size: 225.2 MB (225173133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.28`

```console
$ docker pull neo4j@sha256:58821a9b6f2be798782ea9b92affbac926647688ab9a1d727bada80132de93a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.28` - linux; amd64

```console
$ docker pull neo4j@sha256:0cc2304afc87557e0adac8154f9f7dd97db179fa4de2f9606c4fa1100e6bea4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297351612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92605d7d706ad3b955b9f6cc5eb676a69edc9c265430a967de9acad2100c1965`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:39:06 GMT
COPY dir:d20aeb749bf0b3fe533952f7903b6aa08724fe8bf03e369130d4e2a6ff71bd3f in /opt/java/openjdk 
# Sat, 02 Dec 2023 07:39:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f00e23cf063836a6c39fe0baef42f7ade86d7a096548dcccb4620aa0e1a2a6a NEO4J_TARBALL=neo4j-community-4.4.28-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 07:39:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 07:39:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 07:39:09 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 07:39:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 07:39:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:39:38 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 07:39:38 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 07:39:38 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 07:39:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:39:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e28bbb7ed8d446eab9126cf70b8a8696a1b2c97ace981f72b9e7fa4a8fa7e1`  
		Last Modified: Sat, 02 Dec 2023 07:43:21 GMT  
		Size: 145.3 MB (145266435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0609e7d73a5c1db314d18988189cf0542c93b2b5b3fad6064837df9fcc70f00a`  
		Last Modified: Sat, 02 Dec 2023 07:43:09 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbd2488daaa37df4a60545b9d2c8f0eaffb97cd04e4409a0e0bd232cb1546fe`  
		Last Modified: Sat, 02 Dec 2023 07:43:09 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20b7755b77acacf6b35dc48bbffc1537c8ca86e3a1f1d1825a8c7caacb23045`  
		Last Modified: Sat, 02 Dec 2023 07:43:15 GMT  
		Size: 120.7 MB (120654077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.28` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:d5a6c165f8c5441441634400b01c301d1e8c2747577f32e7fa29e3f3e4fa942c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292699562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32c762fcddaa1dd67bdd1ccf8f300900298434a55c572fc796856acfa2ba55c3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:45:58 GMT
COPY dir:201fdbb3aef6b177b9038d3dd5bbe865568281c78c7bc0c153b57943d571a0b6 in /opt/java/openjdk 
# Sat, 02 Dec 2023 11:55:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f00e23cf063836a6c39fe0baef42f7ade86d7a096548dcccb4620aa0e1a2a6a NEO4J_TARBALL=neo4j-community-4.4.28-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 11:55:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 11:55:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 11:55:09 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 11:55:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 11:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 11:55:36 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 11:55:36 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 11:55:36 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 11:55:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 11:55:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c9736680f80d26b6300f944e7ba80ac7f1a756c950bdf599346e7954ad2dff`  
		Last Modified: Sat, 02 Dec 2023 09:04:30 GMT  
		Size: 142.0 MB (142001789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0052c0ee1539da703ca76e0b52e164012b1a23b80865d07784a2dbf00164ea`  
		Last Modified: Sat, 02 Dec 2023 11:58:41 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53da938b15194a167297081c5683008de76f1c926337793487f93995a74ccf11`  
		Last Modified: Sat, 02 Dec 2023 11:58:41 GMT  
		Size: 9.4 KB (9418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e244f831fb37ad9fd4cf1c9aeddf80c67dc937ea40b5935a244e7757ec8b98`  
		Last Modified: Sat, 02 Dec 2023 11:58:46 GMT  
		Size: 120.6 MB (120620349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.28-community`

```console
$ docker pull neo4j@sha256:58821a9b6f2be798782ea9b92affbac926647688ab9a1d727bada80132de93a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.28-community` - linux; amd64

```console
$ docker pull neo4j@sha256:0cc2304afc87557e0adac8154f9f7dd97db179fa4de2f9606c4fa1100e6bea4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297351612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92605d7d706ad3b955b9f6cc5eb676a69edc9c265430a967de9acad2100c1965`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:39:06 GMT
COPY dir:d20aeb749bf0b3fe533952f7903b6aa08724fe8bf03e369130d4e2a6ff71bd3f in /opt/java/openjdk 
# Sat, 02 Dec 2023 07:39:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f00e23cf063836a6c39fe0baef42f7ade86d7a096548dcccb4620aa0e1a2a6a NEO4J_TARBALL=neo4j-community-4.4.28-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 07:39:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 07:39:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 07:39:09 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 07:39:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 07:39:38 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:39:38 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 07:39:38 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 07:39:38 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 07:39:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:39:39 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e28bbb7ed8d446eab9126cf70b8a8696a1b2c97ace981f72b9e7fa4a8fa7e1`  
		Last Modified: Sat, 02 Dec 2023 07:43:21 GMT  
		Size: 145.3 MB (145266435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0609e7d73a5c1db314d18988189cf0542c93b2b5b3fad6064837df9fcc70f00a`  
		Last Modified: Sat, 02 Dec 2023 07:43:09 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbd2488daaa37df4a60545b9d2c8f0eaffb97cd04e4409a0e0bd232cb1546fe`  
		Last Modified: Sat, 02 Dec 2023 07:43:09 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20b7755b77acacf6b35dc48bbffc1537c8ca86e3a1f1d1825a8c7caacb23045`  
		Last Modified: Sat, 02 Dec 2023 07:43:15 GMT  
		Size: 120.7 MB (120654077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.28-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:d5a6c165f8c5441441634400b01c301d1e8c2747577f32e7fa29e3f3e4fa942c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292699562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32c762fcddaa1dd67bdd1ccf8f300900298434a55c572fc796856acfa2ba55c3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:45:58 GMT
COPY dir:201fdbb3aef6b177b9038d3dd5bbe865568281c78c7bc0c153b57943d571a0b6 in /opt/java/openjdk 
# Sat, 02 Dec 2023 11:55:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=5f00e23cf063836a6c39fe0baef42f7ade86d7a096548dcccb4620aa0e1a2a6a NEO4J_TARBALL=neo4j-community-4.4.28-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 11:55:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 11:55:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 11:55:09 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 11:55:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 11:55:36 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 11:55:36 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 11:55:36 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 11:55:36 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 11:55:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 11:55:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c9736680f80d26b6300f944e7ba80ac7f1a756c950bdf599346e7954ad2dff`  
		Last Modified: Sat, 02 Dec 2023 09:04:30 GMT  
		Size: 142.0 MB (142001789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0052c0ee1539da703ca76e0b52e164012b1a23b80865d07784a2dbf00164ea`  
		Last Modified: Sat, 02 Dec 2023 11:58:41 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53da938b15194a167297081c5683008de76f1c926337793487f93995a74ccf11`  
		Last Modified: Sat, 02 Dec 2023 11:58:41 GMT  
		Size: 9.4 KB (9418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e244f831fb37ad9fd4cf1c9aeddf80c67dc937ea40b5935a244e7757ec8b98`  
		Last Modified: Sat, 02 Dec 2023 11:58:46 GMT  
		Size: 120.6 MB (120620349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.28-enterprise`

```console
$ docker pull neo4j@sha256:22a8909b929765b92558c40f6ea7717e9145017d54984e790a5231769587d50b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.28-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:95047e3c76d3481d3728bca1f30fe4221fb36da69d13c40f15997aa1fff968bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.9 MB (401907379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0849facd0a7645b7f70420e538ba34451812115a7be15a83369dc49779a0e728`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:39:06 GMT
COPY dir:d20aeb749bf0b3fe533952f7903b6aa08724fe8bf03e369130d4e2a6ff71bd3f in /opt/java/openjdk 
# Sat, 02 Dec 2023 07:39:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=57dab47060e05c353c0c6741d9bbd0b8bc05677e5c5e16592ebdaf1ec90b1678 NEO4J_TARBALL=neo4j-enterprise-4.4.28-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 07:39:44 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 07:39:45 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 07:39:45 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 07:40:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 07:40:21 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:40:21 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 07:40:21 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 07:40:21 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 07:40:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 07:40:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e28bbb7ed8d446eab9126cf70b8a8696a1b2c97ace981f72b9e7fa4a8fa7e1`  
		Last Modified: Sat, 02 Dec 2023 07:43:21 GMT  
		Size: 145.3 MB (145266435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defc888d987870a51f472b728fd09b7235ee48e4bd61871c14aae8eee642bbce`  
		Last Modified: Sat, 02 Dec 2023 07:43:33 GMT  
		Size: 3.9 KB (3858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df57ee89926a2202b735f6116042a537af3272578bdbabdfb1f22b291e372546`  
		Last Modified: Sat, 02 Dec 2023 07:43:33 GMT  
		Size: 9.4 KB (9415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4778b5c7eefb485b3983316f5612bc946ca41ade136936eb81e1c8fa08182d2c`  
		Last Modified: Sat, 02 Dec 2023 07:43:42 GMT  
		Size: 225.2 MB (225209847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.28-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:02e9296a7db24d8e30960f52cd134b2a25e289e6f738a0e9d3beca22c6917f25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.3 MB (397252348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42df89dcc0eb7a9e9748bb59ef476c82cd6eb8b19c918e10269900711da9c1a`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:45:58 GMT
COPY dir:201fdbb3aef6b177b9038d3dd5bbe865568281c78c7bc0c153b57943d571a0b6 in /opt/java/openjdk 
# Sat, 02 Dec 2023 11:55:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=57dab47060e05c353c0c6741d9bbd0b8bc05677e5c5e16592ebdaf1ec90b1678 NEO4J_TARBALL=neo4j-enterprise-4.4.28-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Dec 2023 11:55:42 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
# Sat, 02 Dec 2023 11:55:42 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Dec 2023 11:55:43 GMT
COPY multi:c12cca2f0caa27234ee009a6f13af4571110b68335ab209e0f1d1267b8204be3 in /startup/ 
# Sat, 02 Dec 2023 11:56:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.28-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Sat, 02 Dec 2023 11:56:08 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 11:56:08 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Dec 2023 11:56:08 GMT
VOLUME [/data /logs]
# Sat, 02 Dec 2023 11:56:08 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Dec 2023 11:56:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Dec 2023 11:56:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c9736680f80d26b6300f944e7ba80ac7f1a756c950bdf599346e7954ad2dff`  
		Last Modified: Sat, 02 Dec 2023 09:04:30 GMT  
		Size: 142.0 MB (142001789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf5642a1b8a5b80fbfdde4a35694e65df68820097bab5700262a1654ef1248e`  
		Last Modified: Sat, 02 Dec 2023 11:58:58 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f250da6740af78797be267bd6077033ffdbd37599bf9e285705ed2a633d1072c`  
		Last Modified: Sat, 02 Dec 2023 11:58:59 GMT  
		Size: 9.4 KB (9419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77b2f4763eceb909f9aeb3cb0733d1818c64fe5bf1802e1564c617e0d9678cf`  
		Last Modified: Sat, 02 Dec 2023 11:59:07 GMT  
		Size: 225.2 MB (225173133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-bullseye`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community-bullseye`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community-ubi8`

```console
$ docker pull neo4j@sha256:66ee178804b2cef4d96970102f1e888757d8f057a4693948ca94de78db54a549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:3691352f8f19990f7ee48760f4fe11c6c2bfc113b823e97159429bcf195f15c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419558005b5f432dbde0de3e3ea83f3097a49580470564a0e5e673922f3dd018`
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
# Fri, 15 Dec 2023 20:27:50 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:27:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:27:51 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:27:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 20:27:55 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:27:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:27:55 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:27:55 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:27:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:27:55 GMT
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
	-	`sha256:cf59deb2402f310709eba8cf138253ce5d5c2a56e8fe4766dd0fecd80b88d1f4`  
		Last Modified: Fri, 15 Dec 2023 20:30:06 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45ed7e108e2499b7058c383574889cd1a388c1f21990044a84f49e7de6c2d78`  
		Last Modified: Fri, 15 Dec 2023 20:30:12 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8d044f777243781a40289d57084f76df08b3d10ae10e54ea6ff988bf731afdf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301032001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e6f328c8da8a6d3ecbba9457379a04ddf326b4f60964f9064fe4233b9b0d87`
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
# Fri, 15 Dec 2023 19:56:47 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:56:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:56:47 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:56:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 19:56:51 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:56:51 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:56:51 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:56:51 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:56:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:56:51 GMT
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
	-	`sha256:678aadd0357c08f88064688bc130b5741e8e090c574435c5ba1241414a92687d`  
		Last Modified: Fri, 15 Dec 2023 19:58:56 GMT  
		Size: 9.5 KB (9492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e32f6d606e84f5f5c58783fe8e34b659be9375e00ab66af55b522748efba70`  
		Last Modified: Fri, 15 Dec 2023 19:59:00 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:146f4274ff235006af008f3d00087b23a8e31b8cb4da2e593c3c65e88b91d7e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:fa010d9206174022a5a4635c942146b6a08663de8b951bae737d2ab41b78e0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.7 MB (565743748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f9b34b44d79ed4a296b4c3d72b36fbe199fd1545c0aba1388096e1e9f8ee72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:25:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:25:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:25:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:25:11 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:44 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:44 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:44 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:44 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:44 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae39b7af5987a41cdb35983b56add04547233dc7edcbf58a6a9172431a06d5`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 3.9 KB (3872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28dd1cc0bf3eeebfa503dc778864c0c921dc5c412f4bc5a2ec2aea83d1b500d`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331217693aad4ce280b9b77f716fb8df9c088600723dff20b1aa0cbddc8dedd`  
		Last Modified: Fri, 15 Dec 2023 20:29:44 GMT  
		Size: 389.4 MB (389438662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:38e26208bdaf43907adf3b729c8ad9d7359a25d779fbcc771eae69a3ce54bf9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563162628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d011222cf93171c66aa6789fcdcded634920296bb7de05368e156ab333e8c643`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:54:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:54:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:54:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:54:18 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:48 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:48 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfda03cc0832011a22b20addea2402464befa486f7f25ccce0fbac8fc1a5d5e8`  
		Last Modified: Fri, 15 Dec 2023 19:58:22 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d952aa4ac391ad27a65ecc9fd7b1d9037b26d856a359961575e8ee3acf304b3`  
		Last Modified: Fri, 15 Dec 2023 19:58:21 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbe77bbe7384be2f06a8114b7dffd3ada2dddc79443b666f1694301b2cdf296`  
		Last Modified: Fri, 15 Dec 2023 19:58:35 GMT  
		Size: 389.4 MB (389403382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:146f4274ff235006af008f3d00087b23a8e31b8cb4da2e593c3c65e88b91d7e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:fa010d9206174022a5a4635c942146b6a08663de8b951bae737d2ab41b78e0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.7 MB (565743748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f9b34b44d79ed4a296b4c3d72b36fbe199fd1545c0aba1388096e1e9f8ee72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:25:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:25:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:25:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:25:11 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:44 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:44 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:44 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:44 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:44 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae39b7af5987a41cdb35983b56add04547233dc7edcbf58a6a9172431a06d5`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 3.9 KB (3872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28dd1cc0bf3eeebfa503dc778864c0c921dc5c412f4bc5a2ec2aea83d1b500d`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331217693aad4ce280b9b77f716fb8df9c088600723dff20b1aa0cbddc8dedd`  
		Last Modified: Fri, 15 Dec 2023 20:29:44 GMT  
		Size: 389.4 MB (389438662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:38e26208bdaf43907adf3b729c8ad9d7359a25d779fbcc771eae69a3ce54bf9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563162628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d011222cf93171c66aa6789fcdcded634920296bb7de05368e156ab333e8c643`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:54:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:54:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:54:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:54:18 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:48 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:48 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfda03cc0832011a22b20addea2402464befa486f7f25ccce0fbac8fc1a5d5e8`  
		Last Modified: Fri, 15 Dec 2023 19:58:22 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d952aa4ac391ad27a65ecc9fd7b1d9037b26d856a359961575e8ee3acf304b3`  
		Last Modified: Fri, 15 Dec 2023 19:58:21 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbe77bbe7384be2f06a8114b7dffd3ada2dddc79443b666f1694301b2cdf296`  
		Last Modified: Fri, 15 Dec 2023 19:58:35 GMT  
		Size: 389.4 MB (389403382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:6d684e23849b05bed6e9d589f60036368c33d70465352612d4f8b676153c730f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise-ubi8` - linux; amd64

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

### `neo4j:5-enterprise-ubi8` - linux; arm64 variant v8

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

## `neo4j:5-ubi8`

```console
$ docker pull neo4j@sha256:66ee178804b2cef4d96970102f1e888757d8f057a4693948ca94de78db54a549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:3691352f8f19990f7ee48760f4fe11c6c2bfc113b823e97159429bcf195f15c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419558005b5f432dbde0de3e3ea83f3097a49580470564a0e5e673922f3dd018`
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
# Fri, 15 Dec 2023 20:27:50 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:27:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:27:51 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:27:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 20:27:55 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:27:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:27:55 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:27:55 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:27:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:27:55 GMT
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
	-	`sha256:cf59deb2402f310709eba8cf138253ce5d5c2a56e8fe4766dd0fecd80b88d1f4`  
		Last Modified: Fri, 15 Dec 2023 20:30:06 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45ed7e108e2499b7058c383574889cd1a388c1f21990044a84f49e7de6c2d78`  
		Last Modified: Fri, 15 Dec 2023 20:30:12 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8d044f777243781a40289d57084f76df08b3d10ae10e54ea6ff988bf731afdf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301032001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e6f328c8da8a6d3ecbba9457379a04ddf326b4f60964f9064fe4233b9b0d87`
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
# Fri, 15 Dec 2023 19:56:47 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:56:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:56:47 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:56:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 19:56:51 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:56:51 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:56:51 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:56:51 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:56:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:56:51 GMT
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
	-	`sha256:678aadd0357c08f88064688bc130b5741e8e090c574435c5ba1241414a92687d`  
		Last Modified: Fri, 15 Dec 2023 19:58:56 GMT  
		Size: 9.5 KB (9492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e32f6d606e84f5f5c58783fe8e34b659be9375e00ab66af55b522748efba70`  
		Last Modified: Fri, 15 Dec 2023 19:59:00 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15-bullseye`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15-community`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15-community` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15-community-bullseye`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15-community-ubi8`

```console
$ docker pull neo4j@sha256:66ee178804b2cef4d96970102f1e888757d8f057a4693948ca94de78db54a549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:3691352f8f19990f7ee48760f4fe11c6c2bfc113b823e97159429bcf195f15c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419558005b5f432dbde0de3e3ea83f3097a49580470564a0e5e673922f3dd018`
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
# Fri, 15 Dec 2023 20:27:50 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:27:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:27:51 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:27:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 20:27:55 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:27:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:27:55 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:27:55 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:27:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:27:55 GMT
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
	-	`sha256:cf59deb2402f310709eba8cf138253ce5d5c2a56e8fe4766dd0fecd80b88d1f4`  
		Last Modified: Fri, 15 Dec 2023 20:30:06 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45ed7e108e2499b7058c383574889cd1a388c1f21990044a84f49e7de6c2d78`  
		Last Modified: Fri, 15 Dec 2023 20:30:12 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8d044f777243781a40289d57084f76df08b3d10ae10e54ea6ff988bf731afdf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301032001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e6f328c8da8a6d3ecbba9457379a04ddf326b4f60964f9064fe4233b9b0d87`
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
# Fri, 15 Dec 2023 19:56:47 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:56:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:56:47 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:56:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 19:56:51 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:56:51 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:56:51 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:56:51 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:56:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:56:51 GMT
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
	-	`sha256:678aadd0357c08f88064688bc130b5741e8e090c574435c5ba1241414a92687d`  
		Last Modified: Fri, 15 Dec 2023 19:58:56 GMT  
		Size: 9.5 KB (9492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e32f6d606e84f5f5c58783fe8e34b659be9375e00ab66af55b522748efba70`  
		Last Modified: Fri, 15 Dec 2023 19:59:00 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15-enterprise`

```console
$ docker pull neo4j@sha256:146f4274ff235006af008f3d00087b23a8e31b8cb4da2e593c3c65e88b91d7e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:fa010d9206174022a5a4635c942146b6a08663de8b951bae737d2ab41b78e0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.7 MB (565743748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f9b34b44d79ed4a296b4c3d72b36fbe199fd1545c0aba1388096e1e9f8ee72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:25:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:25:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:25:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:25:11 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:44 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:44 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:44 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:44 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:44 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae39b7af5987a41cdb35983b56add04547233dc7edcbf58a6a9172431a06d5`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 3.9 KB (3872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28dd1cc0bf3eeebfa503dc778864c0c921dc5c412f4bc5a2ec2aea83d1b500d`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331217693aad4ce280b9b77f716fb8df9c088600723dff20b1aa0cbddc8dedd`  
		Last Modified: Fri, 15 Dec 2023 20:29:44 GMT  
		Size: 389.4 MB (389438662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:38e26208bdaf43907adf3b729c8ad9d7359a25d779fbcc771eae69a3ce54bf9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563162628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d011222cf93171c66aa6789fcdcded634920296bb7de05368e156ab333e8c643`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:54:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:54:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:54:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:54:18 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:48 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:48 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfda03cc0832011a22b20addea2402464befa486f7f25ccce0fbac8fc1a5d5e8`  
		Last Modified: Fri, 15 Dec 2023 19:58:22 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d952aa4ac391ad27a65ecc9fd7b1d9037b26d856a359961575e8ee3acf304b3`  
		Last Modified: Fri, 15 Dec 2023 19:58:21 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbe77bbe7384be2f06a8114b7dffd3ada2dddc79443b666f1694301b2cdf296`  
		Last Modified: Fri, 15 Dec 2023 19:58:35 GMT  
		Size: 389.4 MB (389403382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:146f4274ff235006af008f3d00087b23a8e31b8cb4da2e593c3c65e88b91d7e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:fa010d9206174022a5a4635c942146b6a08663de8b951bae737d2ab41b78e0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.7 MB (565743748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f9b34b44d79ed4a296b4c3d72b36fbe199fd1545c0aba1388096e1e9f8ee72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:25:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:25:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:25:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:25:11 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:44 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:44 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:44 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:44 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:44 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae39b7af5987a41cdb35983b56add04547233dc7edcbf58a6a9172431a06d5`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 3.9 KB (3872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28dd1cc0bf3eeebfa503dc778864c0c921dc5c412f4bc5a2ec2aea83d1b500d`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331217693aad4ce280b9b77f716fb8df9c088600723dff20b1aa0cbddc8dedd`  
		Last Modified: Fri, 15 Dec 2023 20:29:44 GMT  
		Size: 389.4 MB (389438662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:38e26208bdaf43907adf3b729c8ad9d7359a25d779fbcc771eae69a3ce54bf9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563162628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d011222cf93171c66aa6789fcdcded634920296bb7de05368e156ab333e8c643`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:54:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:54:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:54:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:54:18 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:48 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:48 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfda03cc0832011a22b20addea2402464befa486f7f25ccce0fbac8fc1a5d5e8`  
		Last Modified: Fri, 15 Dec 2023 19:58:22 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d952aa4ac391ad27a65ecc9fd7b1d9037b26d856a359961575e8ee3acf304b3`  
		Last Modified: Fri, 15 Dec 2023 19:58:21 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbe77bbe7384be2f06a8114b7dffd3ada2dddc79443b666f1694301b2cdf296`  
		Last Modified: Fri, 15 Dec 2023 19:58:35 GMT  
		Size: 389.4 MB (389403382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:6d684e23849b05bed6e9d589f60036368c33d70465352612d4f8b676153c730f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15-enterprise-ubi8` - linux; amd64

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

### `neo4j:5.15-enterprise-ubi8` - linux; arm64 variant v8

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

## `neo4j:5.15-ubi8`

```console
$ docker pull neo4j@sha256:66ee178804b2cef4d96970102f1e888757d8f057a4693948ca94de78db54a549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:3691352f8f19990f7ee48760f4fe11c6c2bfc113b823e97159429bcf195f15c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419558005b5f432dbde0de3e3ea83f3097a49580470564a0e5e673922f3dd018`
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
# Fri, 15 Dec 2023 20:27:50 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:27:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:27:51 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:27:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 20:27:55 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:27:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:27:55 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:27:55 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:27:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:27:55 GMT
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
	-	`sha256:cf59deb2402f310709eba8cf138253ce5d5c2a56e8fe4766dd0fecd80b88d1f4`  
		Last Modified: Fri, 15 Dec 2023 20:30:06 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45ed7e108e2499b7058c383574889cd1a388c1f21990044a84f49e7de6c2d78`  
		Last Modified: Fri, 15 Dec 2023 20:30:12 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8d044f777243781a40289d57084f76df08b3d10ae10e54ea6ff988bf731afdf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301032001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e6f328c8da8a6d3ecbba9457379a04ddf326b4f60964f9064fe4233b9b0d87`
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
# Fri, 15 Dec 2023 19:56:47 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:56:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:56:47 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:56:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 19:56:51 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:56:51 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:56:51 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:56:51 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:56:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:56:51 GMT
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
	-	`sha256:678aadd0357c08f88064688bc130b5741e8e090c574435c5ba1241414a92687d`  
		Last Modified: Fri, 15 Dec 2023 19:58:56 GMT  
		Size: 9.5 KB (9492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e32f6d606e84f5f5c58783fe8e34b659be9375e00ab66af55b522748efba70`  
		Last Modified: Fri, 15 Dec 2023 19:59:00 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15.0`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15.0` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15.0-bullseye`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15.0-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15.0-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15.0-community`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15.0-community-bullseye`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15.0-community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15.0-community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15.0-community-ubi8`

```console
$ docker pull neo4j@sha256:66ee178804b2cef4d96970102f1e888757d8f057a4693948ca94de78db54a549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15.0-community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:3691352f8f19990f7ee48760f4fe11c6c2bfc113b823e97159429bcf195f15c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419558005b5f432dbde0de3e3ea83f3097a49580470564a0e5e673922f3dd018`
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
# Fri, 15 Dec 2023 20:27:50 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:27:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:27:51 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:27:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 20:27:55 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:27:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:27:55 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:27:55 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:27:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:27:55 GMT
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
	-	`sha256:cf59deb2402f310709eba8cf138253ce5d5c2a56e8fe4766dd0fecd80b88d1f4`  
		Last Modified: Fri, 15 Dec 2023 20:30:06 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45ed7e108e2499b7058c383574889cd1a388c1f21990044a84f49e7de6c2d78`  
		Last Modified: Fri, 15 Dec 2023 20:30:12 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15.0-community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8d044f777243781a40289d57084f76df08b3d10ae10e54ea6ff988bf731afdf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301032001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e6f328c8da8a6d3ecbba9457379a04ddf326b4f60964f9064fe4233b9b0d87`
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
# Fri, 15 Dec 2023 19:56:47 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:56:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:56:47 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:56:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 19:56:51 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:56:51 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:56:51 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:56:51 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:56:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:56:51 GMT
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
	-	`sha256:678aadd0357c08f88064688bc130b5741e8e090c574435c5ba1241414a92687d`  
		Last Modified: Fri, 15 Dec 2023 19:58:56 GMT  
		Size: 9.5 KB (9492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e32f6d606e84f5f5c58783fe8e34b659be9375e00ab66af55b522748efba70`  
		Last Modified: Fri, 15 Dec 2023 19:59:00 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15.0-enterprise`

```console
$ docker pull neo4j@sha256:146f4274ff235006af008f3d00087b23a8e31b8cb4da2e593c3c65e88b91d7e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:fa010d9206174022a5a4635c942146b6a08663de8b951bae737d2ab41b78e0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.7 MB (565743748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f9b34b44d79ed4a296b4c3d72b36fbe199fd1545c0aba1388096e1e9f8ee72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:25:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:25:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:25:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:25:11 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:44 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:44 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:44 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:44 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:44 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae39b7af5987a41cdb35983b56add04547233dc7edcbf58a6a9172431a06d5`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 3.9 KB (3872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28dd1cc0bf3eeebfa503dc778864c0c921dc5c412f4bc5a2ec2aea83d1b500d`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331217693aad4ce280b9b77f716fb8df9c088600723dff20b1aa0cbddc8dedd`  
		Last Modified: Fri, 15 Dec 2023 20:29:44 GMT  
		Size: 389.4 MB (389438662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:38e26208bdaf43907adf3b729c8ad9d7359a25d779fbcc771eae69a3ce54bf9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563162628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d011222cf93171c66aa6789fcdcded634920296bb7de05368e156ab333e8c643`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:54:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:54:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:54:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:54:18 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:48 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:48 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfda03cc0832011a22b20addea2402464befa486f7f25ccce0fbac8fc1a5d5e8`  
		Last Modified: Fri, 15 Dec 2023 19:58:22 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d952aa4ac391ad27a65ecc9fd7b1d9037b26d856a359961575e8ee3acf304b3`  
		Last Modified: Fri, 15 Dec 2023 19:58:21 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbe77bbe7384be2f06a8114b7dffd3ada2dddc79443b666f1694301b2cdf296`  
		Last Modified: Fri, 15 Dec 2023 19:58:35 GMT  
		Size: 389.4 MB (389403382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15.0-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:146f4274ff235006af008f3d00087b23a8e31b8cb4da2e593c3c65e88b91d7e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15.0-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:fa010d9206174022a5a4635c942146b6a08663de8b951bae737d2ab41b78e0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.7 MB (565743748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f9b34b44d79ed4a296b4c3d72b36fbe199fd1545c0aba1388096e1e9f8ee72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:25:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:25:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:25:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:25:11 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:44 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:44 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:44 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:44 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:44 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae39b7af5987a41cdb35983b56add04547233dc7edcbf58a6a9172431a06d5`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 3.9 KB (3872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28dd1cc0bf3eeebfa503dc778864c0c921dc5c412f4bc5a2ec2aea83d1b500d`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331217693aad4ce280b9b77f716fb8df9c088600723dff20b1aa0cbddc8dedd`  
		Last Modified: Fri, 15 Dec 2023 20:29:44 GMT  
		Size: 389.4 MB (389438662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15.0-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:38e26208bdaf43907adf3b729c8ad9d7359a25d779fbcc771eae69a3ce54bf9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563162628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d011222cf93171c66aa6789fcdcded634920296bb7de05368e156ab333e8c643`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:54:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:54:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:54:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:54:18 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:48 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:48 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfda03cc0832011a22b20addea2402464befa486f7f25ccce0fbac8fc1a5d5e8`  
		Last Modified: Fri, 15 Dec 2023 19:58:22 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d952aa4ac391ad27a65ecc9fd7b1d9037b26d856a359961575e8ee3acf304b3`  
		Last Modified: Fri, 15 Dec 2023 19:58:21 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbe77bbe7384be2f06a8114b7dffd3ada2dddc79443b666f1694301b2cdf296`  
		Last Modified: Fri, 15 Dec 2023 19:58:35 GMT  
		Size: 389.4 MB (389403382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.15.0-enterprise-ubi8`

```console
$ docker pull neo4j@sha256:6d684e23849b05bed6e9d589f60036368c33d70465352612d4f8b676153c730f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15.0-enterprise-ubi8` - linux; amd64

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

### `neo4j:5.15.0-enterprise-ubi8` - linux; arm64 variant v8

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

## `neo4j:5.15.0-ubi8`

```console
$ docker pull neo4j@sha256:66ee178804b2cef4d96970102f1e888757d8f057a4693948ca94de78db54a549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.15.0-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:3691352f8f19990f7ee48760f4fe11c6c2bfc113b823e97159429bcf195f15c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419558005b5f432dbde0de3e3ea83f3097a49580470564a0e5e673922f3dd018`
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
# Fri, 15 Dec 2023 20:27:50 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:27:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:27:51 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:27:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 20:27:55 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:27:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:27:55 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:27:55 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:27:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:27:55 GMT
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
	-	`sha256:cf59deb2402f310709eba8cf138253ce5d5c2a56e8fe4766dd0fecd80b88d1f4`  
		Last Modified: Fri, 15 Dec 2023 20:30:06 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45ed7e108e2499b7058c383574889cd1a388c1f21990044a84f49e7de6c2d78`  
		Last Modified: Fri, 15 Dec 2023 20:30:12 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.15.0-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8d044f777243781a40289d57084f76df08b3d10ae10e54ea6ff988bf731afdf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301032001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e6f328c8da8a6d3ecbba9457379a04ddf326b4f60964f9064fe4233b9b0d87`
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
# Fri, 15 Dec 2023 19:56:47 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:56:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:56:47 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:56:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 19:56:51 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:56:51 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:56:51 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:56:51 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:56:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:56:51 GMT
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
	-	`sha256:678aadd0357c08f88064688bc130b5741e8e090c574435c5ba1241414a92687d`  
		Last Modified: Fri, 15 Dec 2023 19:58:56 GMT  
		Size: 9.5 KB (9492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e32f6d606e84f5f5c58783fe8e34b659be9375e00ab66af55b522748efba70`  
		Last Modified: Fri, 15 Dec 2023 19:59:00 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:bullseye`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community-bullseye`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community-ubi8`

```console
$ docker pull neo4j@sha256:66ee178804b2cef4d96970102f1e888757d8f057a4693948ca94de78db54a549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community-ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:3691352f8f19990f7ee48760f4fe11c6c2bfc113b823e97159429bcf195f15c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419558005b5f432dbde0de3e3ea83f3097a49580470564a0e5e673922f3dd018`
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
# Fri, 15 Dec 2023 20:27:50 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:27:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:27:51 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:27:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 20:27:55 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:27:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:27:55 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:27:55 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:27:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:27:55 GMT
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
	-	`sha256:cf59deb2402f310709eba8cf138253ce5d5c2a56e8fe4766dd0fecd80b88d1f4`  
		Last Modified: Fri, 15 Dec 2023 20:30:06 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45ed7e108e2499b7058c383574889cd1a388c1f21990044a84f49e7de6c2d78`  
		Last Modified: Fri, 15 Dec 2023 20:30:12 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community-ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8d044f777243781a40289d57084f76df08b3d10ae10e54ea6ff988bf731afdf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301032001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e6f328c8da8a6d3ecbba9457379a04ddf326b4f60964f9064fe4233b9b0d87`
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
# Fri, 15 Dec 2023 19:56:47 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:56:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:56:47 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:56:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 19:56:51 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:56:51 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:56:51 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:56:51 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:56:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:56:51 GMT
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
	-	`sha256:678aadd0357c08f88064688bc130b5741e8e090c574435c5ba1241414a92687d`  
		Last Modified: Fri, 15 Dec 2023 19:58:56 GMT  
		Size: 9.5 KB (9492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e32f6d606e84f5f5c58783fe8e34b659be9375e00ab66af55b522748efba70`  
		Last Modified: Fri, 15 Dec 2023 19:59:00 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:146f4274ff235006af008f3d00087b23a8e31b8cb4da2e593c3c65e88b91d7e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:fa010d9206174022a5a4635c942146b6a08663de8b951bae737d2ab41b78e0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.7 MB (565743748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f9b34b44d79ed4a296b4c3d72b36fbe199fd1545c0aba1388096e1e9f8ee72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:25:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:25:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:25:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:25:11 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:44 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:44 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:44 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:44 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:44 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae39b7af5987a41cdb35983b56add04547233dc7edcbf58a6a9172431a06d5`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 3.9 KB (3872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28dd1cc0bf3eeebfa503dc778864c0c921dc5c412f4bc5a2ec2aea83d1b500d`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331217693aad4ce280b9b77f716fb8df9c088600723dff20b1aa0cbddc8dedd`  
		Last Modified: Fri, 15 Dec 2023 20:29:44 GMT  
		Size: 389.4 MB (389438662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:38e26208bdaf43907adf3b729c8ad9d7359a25d779fbcc771eae69a3ce54bf9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563162628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d011222cf93171c66aa6789fcdcded634920296bb7de05368e156ab333e8c643`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:54:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:54:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:54:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:54:18 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:48 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:48 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfda03cc0832011a22b20addea2402464befa486f7f25ccce0fbac8fc1a5d5e8`  
		Last Modified: Fri, 15 Dec 2023 19:58:22 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d952aa4ac391ad27a65ecc9fd7b1d9037b26d856a359961575e8ee3acf304b3`  
		Last Modified: Fri, 15 Dec 2023 19:58:21 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbe77bbe7384be2f06a8114b7dffd3ada2dddc79443b666f1694301b2cdf296`  
		Last Modified: Fri, 15 Dec 2023 19:58:35 GMT  
		Size: 389.4 MB (389403382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise-bullseye`

```console
$ docker pull neo4j@sha256:146f4274ff235006af008f3d00087b23a8e31b8cb4da2e593c3c65e88b91d7e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:fa010d9206174022a5a4635c942146b6a08663de8b951bae737d2ab41b78e0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **565.7 MB (565743748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f9b34b44d79ed4a296b4c3d72b36fbe199fd1545c0aba1388096e1e9f8ee72`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:25:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:25:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:25:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:25:11 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:43 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:44 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:44 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:44 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:44 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:44 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:44 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aae39b7af5987a41cdb35983b56add04547233dc7edcbf58a6a9172431a06d5`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 3.9 KB (3872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28dd1cc0bf3eeebfa503dc778864c0c921dc5c412f4bc5a2ec2aea83d1b500d`  
		Last Modified: Fri, 15 Dec 2023 20:29:29 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331217693aad4ce280b9b77f716fb8df9c088600723dff20b1aa0cbddc8dedd`  
		Last Modified: Fri, 15 Dec 2023 20:29:44 GMT  
		Size: 389.4 MB (389438662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:38e26208bdaf43907adf3b729c8ad9d7359a25d779fbcc771eae69a3ce54bf9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.2 MB (563162628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d011222cf93171c66aa6789fcdcded634920296bb7de05368e156ab333e8c643`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:54:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=7571340603eca6b15923ba213f90d6460e9622657db955488207c0437fb414fb NEO4J_TARBALL=neo4j-enterprise-5.15.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:54:17 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:54:17 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:54:18 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:48 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:48 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfda03cc0832011a22b20addea2402464befa486f7f25ccce0fbac8fc1a5d5e8`  
		Last Modified: Fri, 15 Dec 2023 19:58:22 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d952aa4ac391ad27a65ecc9fd7b1d9037b26d856a359961575e8ee3acf304b3`  
		Last Modified: Fri, 15 Dec 2023 19:58:21 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbe77bbe7384be2f06a8114b7dffd3ada2dddc79443b666f1694301b2cdf296`  
		Last Modified: Fri, 15 Dec 2023 19:58:35 GMT  
		Size: 389.4 MB (389403382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:9c564b96267ab1b2c64944808d3b4cb054c6b7be684cd98027804effefe6db8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:789a89f1bed2ce8615883a948e4a9eb4e774dd74256f237fb73e5f555e1ee4c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291851029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dfb69e69728e4da94093c47befed672cce9d9c83148c387ceede5a1e45f0a22`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:09:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 07:35:48 GMT
COPY dir:e13dbcd57950f4d4d23f4aba8428b6fbbf838d8f4801d32a25e344d37d33c37e in /opt/java/openjdk 
# Fri, 15 Dec 2023 20:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:24:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:24:30 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 20:24:30 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:25:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 20:25:02 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:25:02 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:25:02 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:25:02 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:25:02 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:25:03 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4929994d0853caabbfd68ce7ab07e3af7c0e483db2f66881247df513f25c95`  
		Last Modified: Sat, 02 Dec 2023 07:40:56 GMT  
		Size: 144.9 MB (144873901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d6899848fc5eaac913b6751e14a1eaf620d140842ebb2517980cc9c3c9efc9`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6539ea3d558ea7232af6399fcfbbf7ca3c20cf3741399229d8c2b7b87898ef`  
		Last Modified: Fri, 15 Dec 2023 20:28:46 GMT  
		Size: 9.5 KB (9489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83735c89ef28eba22026769152b573ee0c1d914ca3b03fe508d327603b18e78e`  
		Last Modified: Fri, 15 Dec 2023 20:28:52 GMT  
		Size: 115.5 MB (115545956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f28741ec0e2bc6b4beffbf32026b11311b0c8cfbd24069893bf16ab741c88fa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289274766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b49430bb9c8b01aa5087b38d91c3060bfd7be63cb69ebd4dfa7e33975acaa00`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:22:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Dec 2023 08:54:33 GMT
COPY dir:b97789a1c2e6d715436236e063679209ed5b51287e172faadc90d7cbd7bc1135 in /opt/java/openjdk 
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:53:43 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:53:44 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 15 Dec 2023 19:53:44 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:54:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN apt update     && apt-get install -y curl gcc git jq make procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && git clone https://github.com/ncopa/su-exec.git     && cd su-exec     && git checkout 4c3bb42b093f14da70d8ab924b487ccfbb1397af     && echo d6c40440609a23483f12eb6295b5191e94baf08298a856bab6e15b10c3b82891 su-exec.c | sha256sum -c     && echo 2a87af245eb125aca9305a0b1025525ac80825590800f047419dc57bba36b334 Makefile | sha256sum -c     && make     && mv /su-exec/su-exec /usr/bin/su-exec     && apt-get -y purge --auto-remove curl gcc git make     && rm -rf /var/lib/apt/lists/* /su-exec
# Fri, 15 Dec 2023 19:54:12 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:54:12 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:54:12 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:54:12 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:54:12 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:54:12 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d93fb72555944d51d7e18e85dbba1405725af6fa11dc155f20ab3dc455df52`  
		Last Modified: Sat, 02 Dec 2023 09:08:50 GMT  
		Size: 143.7 MB (143681749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231bc995d177519536f3394d00334e961ba4ce52b39a4de4e5655ac3265e9f4`  
		Last Modified: Fri, 15 Dec 2023 19:57:41 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdfd6cc00534f53f3ba3907fc83af82d3a122113ac12e9bfc194a82cd46fa9`  
		Last Modified: Fri, 15 Dec 2023 19:57:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5a282811d905ae461208da4adbc648e78d0515e819bb2ae9d88c5c7534f8d9`  
		Last Modified: Fri, 15 Dec 2023 19:57:46 GMT  
		Size: 115.5 MB (115515518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:ubi8`

```console
$ docker pull neo4j@sha256:66ee178804b2cef4d96970102f1e888757d8f057a4693948ca94de78db54a549
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:ubi8` - linux; amd64

```console
$ docker pull neo4j@sha256:3691352f8f19990f7ee48760f4fe11c6c2bfc113b823e97159429bcf195f15c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304128237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419558005b5f432dbde0de3e3ea83f3097a49580470564a0e5e673922f3dd018`
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
# Fri, 15 Dec 2023 20:27:50 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 20:27:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 20:27:51 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 20:27:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 20:27:55 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 20:27:55 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 20:27:55 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 20:27:55 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 20:27:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 20:27:55 GMT
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
	-	`sha256:cf59deb2402f310709eba8cf138253ce5d5c2a56e8fe4766dd0fecd80b88d1f4`  
		Last Modified: Fri, 15 Dec 2023 20:30:06 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45ed7e108e2499b7058c383574889cd1a388c1f21990044a84f49e7de6c2d78`  
		Last Modified: Fri, 15 Dec 2023 20:30:12 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:ubi8` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8d044f777243781a40289d57084f76df08b3d10ae10e54ea6ff988bf731afdf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301032001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e6f328c8da8a6d3ecbba9457379a04ddf326b4f60964f9064fe4233b9b0d87`
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
# Fri, 15 Dec 2023 19:56:47 GMT
ENV PATH=/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0090ee5fd8ca5718ced107d5e7a7803919f55b970c3e7acad83bf88292a2361f NEO4J_TARBALL=neo4j-community-5.15.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 15 Dec 2023 19:56:47 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
# Fri, 15 Dec 2023 19:56:47 GMT
COPY multi:8fee13a85b98996afa1dd437b17591f4356f4c453ab9a107827f32427bb071da in /startup/ 
# Fri, 15 Dec 2023 19:56:50 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.15.0-unix.tar.gz
RUN set -eux;     groupadd --gid 7474 --system neo4j && useradd --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --gid neo4j neo4j;     curl --fail --silent --show-error --location --remote-name ${NEO4J_URI};     echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet;     tar --extract --file ${NEO4J_TARBALL} --directory /var/lib;     mv /var/lib/neo4j-* "${NEO4J_HOME}";     rm ${NEO4J_TARBALL};     mv "${NEO4J_HOME}"/data /data;     mv "${NEO4J_HOME}"/logs /logs;     chown -R neo4j:neo4j /data;     chmod -R 777 /data;     chown -R neo4j:neo4j /logs;     chmod -R 777 /logs;     chown -R neo4j:neo4j "${NEO4J_HOME}";     chmod -R 777 "${NEO4J_HOME}";     ln -s /data "${NEO4J_HOME}"/data;     ln -s /logs "${NEO4J_HOME}"/logs;     mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report
# Fri, 15 Dec 2023 19:56:51 GMT
ENV PATH=/var/lib/neo4j/bin:/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:56:51 GMT
WORKDIR /var/lib/neo4j
# Fri, 15 Dec 2023 19:56:51 GMT
VOLUME [/data /logs]
# Fri, 15 Dec 2023 19:56:51 GMT
EXPOSE 7473 7474 7687
# Fri, 15 Dec 2023 19:56:51 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 15 Dec 2023 19:56:51 GMT
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
	-	`sha256:678aadd0357c08f88064688bc130b5741e8e090c574435c5ba1241414a92687d`  
		Last Modified: Fri, 15 Dec 2023 19:58:56 GMT  
		Size: 9.5 KB (9492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e32f6d606e84f5f5c58783fe8e34b659be9375e00ab66af55b522748efba70`  
		Last Modified: Fri, 15 Dec 2023 19:59:00 GMT  
		Size: 112.6 MB (112618886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
