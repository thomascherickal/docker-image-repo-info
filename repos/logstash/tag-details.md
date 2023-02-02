<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.8`](#logstash7178)
-	[`logstash:8.6.1`](#logstash861)

## `logstash:7.17.8`

```console
$ docker pull logstash@sha256:17a4f64e9cf592090d27ae04f82d29cf6cd8d0193aee4ddbc98d3d48785aba7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.8` - linux; amd64

```console
$ docker pull logstash@sha256:bfd7e943403fcb9bbb9f5d9935438a0645bea281e265fa17d2aaaa8c36a32f40
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **439.3 MB (439327352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:450ca8ef458a01eb35cefe29b987ce2bf3cceaa59bdd0680e27f61473b5c6b08`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 16:27:53 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Wed, 30 Nov 2022 16:27:54 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Wed, 30 Nov 2022 16:28:18 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.8-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.8 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Wed, 30 Nov 2022 16:28:21 GMT
WORKDIR /usr/share/logstash
# Wed, 30 Nov 2022 16:28:21 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 30 Nov 2022 16:28:22 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Nov 2022 16:28:22 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Wed, 30 Nov 2022 16:28:22 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Wed, 30 Nov 2022 16:28:22 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Wed, 30 Nov 2022 16:28:22 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Wed, 30 Nov 2022 16:28:22 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Wed, 30 Nov 2022 16:28:23 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 30 Nov 2022 16:28:23 GMT
ADD file:fd9d0a7164e8960b5937497c683f797308c938637accbdddf5785afd2b9bf57b in /usr/local/bin/ 
# Wed, 30 Nov 2022 16:28:23 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Wed, 30 Nov 2022 16:28:23 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Wed, 30 Nov 2022 16:28:23 GMT
USER 1000
# Wed, 30 Nov 2022 16:28:23 GMT
EXPOSE 5044 9600
# Wed, 30 Nov 2022 16:28:24 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.8 org.opencontainers.image.version=7.17.8 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-11-30T16:12:02+00:00 org.opencontainers.image.created=2022-11-30T16:12:02+00:00
# Wed, 30 Nov 2022 16:28:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f823d6208889ffeec2b453ff808f856aca37c98b869052134d61fab9e4c2a83f`  
		Last Modified: Thu, 08 Dec 2022 19:23:16 GMT  
		Size: 41.9 MB (41886332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc931784f49d637e75f3beab5792d3585024b55a98554c0df3af71cbf325dee`  
		Last Modified: Thu, 08 Dec 2022 19:23:11 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce68bbfd60ce0775b48aecf3826d2fa600983b6345c628351578584c01847202`  
		Last Modified: Thu, 08 Dec 2022 19:23:41 GMT  
		Size: 367.1 MB (367086253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837cfbff93fc00a712459958a6578e9be57f1b62b7a3ff27aa03c640d08747d0`  
		Last Modified: Thu, 08 Dec 2022 19:23:11 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ec5d04021fe93edb4271dcb5228c5c9ab51ab2a4f0bb91b0f9f9cffda889cc`  
		Last Modified: Thu, 08 Dec 2022 19:23:11 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed76ef861142c461be3fd9fc0ceef0d7e55926d3714c716a0ebe3d9a1f28c02`  
		Last Modified: Thu, 08 Dec 2022 19:23:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d8b7581e187ca8338f6115c685f4332777ec16c63ef4bef968ef90163261e1`  
		Last Modified: Thu, 08 Dec 2022 19:23:09 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af975d8f765d1402150b7301caee24ee8ddba96bdc4f761896462669f2878cc`  
		Last Modified: Thu, 08 Dec 2022 19:23:09 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2cb522f5402e501bbd9c459965e9db6d08c8c4a21a01d14d9388e21f9bc19b`  
		Last Modified: Thu, 08 Dec 2022 19:23:09 GMT  
		Size: 1.8 MB (1769836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f480fcc2337e9cfb076499d9bf3f68bdb6e99cd32c12dd92130b8be83c1a90e`  
		Last Modified: Thu, 08 Dec 2022 19:23:09 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f480fcc2337e9cfb076499d9bf3f68bdb6e99cd32c12dd92130b8be83c1a90e`  
		Last Modified: Thu, 08 Dec 2022 19:23:09 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.8` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:4323ea4b30e049dc661914a40dedec354fe7633ea5001fffcc00137bac2d0a14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.4 MB (428371129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27945e0b56b6a3545e7d303700a54fcecc7c243de1342a8781f9b829356e5a2f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 30 Nov 2022 16:26:55 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Wed, 30 Nov 2022 16:26:56 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Wed, 30 Nov 2022 16:27:14 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.8-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.8 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Wed, 30 Nov 2022 16:27:18 GMT
WORKDIR /usr/share/logstash
# Wed, 30 Nov 2022 16:27:18 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 30 Nov 2022 16:27:18 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Nov 2022 16:27:19 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Wed, 30 Nov 2022 16:27:19 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Wed, 30 Nov 2022 16:27:19 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Wed, 30 Nov 2022 16:27:19 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Wed, 30 Nov 2022 16:27:19 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Wed, 30 Nov 2022 16:27:19 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 30 Nov 2022 16:27:19 GMT
ADD file:23f506765f8d4b5886b9950ca845119ace9048b115940f036dd7345be6c4568b in /usr/local/bin/ 
# Wed, 30 Nov 2022 16:27:20 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Wed, 30 Nov 2022 16:27:20 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Wed, 30 Nov 2022 16:27:20 GMT
USER 1000
# Wed, 30 Nov 2022 16:27:20 GMT
EXPOSE 5044 9600
# Wed, 30 Nov 2022 16:27:20 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.8 org.opencontainers.image.version=7.17.8 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-11-30T16:13:53+00:00 org.opencontainers.image.created=2022-11-30T16:13:53+00:00
# Wed, 30 Nov 2022 16:27:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970fbd9e1b2059419309efd1cb8d93c574c9739161b8c4a1968daa470764eb3`  
		Last Modified: Thu, 08 Dec 2022 18:42:22 GMT  
		Size: 35.7 MB (35674529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a958d563f0cf47b4b0e259ce086b856a03e8f7f7a2129cfcb12d60d32ad72b4`  
		Last Modified: Thu, 08 Dec 2022 18:42:18 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416eb8b4e716336d88e9381943bba7a44800aa38d1fc1b4246688b20a129866a`  
		Last Modified: Thu, 08 Dec 2022 18:42:44 GMT  
		Size: 363.8 MB (363843751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13361744da54fd558e3c5c87a8797099bceda33a7a171e5bdbe7d58835457cca`  
		Last Modified: Thu, 08 Dec 2022 18:42:18 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdd9fd0789aca318368669002f393ddae5c8e255c32597ac04410c5c35ffdbb`  
		Last Modified: Thu, 08 Dec 2022 18:42:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96f667f10d4ec73b30cfbc3238e215cba2ff172173c5e6a01f867bf42ed1076`  
		Last Modified: Thu, 08 Dec 2022 18:42:16 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79548d93521ac7515eba3399f8b931b790d595670f3b05b47adb3494dd460da4`  
		Last Modified: Thu, 08 Dec 2022 18:42:16 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9509c3215982bc7ce20b3c294169ff34deb99b714974896e34a12939c5a5649f`  
		Last Modified: Thu, 08 Dec 2022 18:42:16 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8b20dee9e55523efc693085f7b65b9af0103b5bf58807beab089d7498c7a98`  
		Last Modified: Thu, 08 Dec 2022 18:42:16 GMT  
		Size: 1.6 MB (1649735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7637ec0a45845b9ad28908406f8e6e84b70116026791dce7d6a7769cf272f5aa`  
		Last Modified: Thu, 08 Dec 2022 18:42:16 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7637ec0a45845b9ad28908406f8e6e84b70116026791dce7d6a7769cf272f5aa`  
		Last Modified: Thu, 08 Dec 2022 18:42:16 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.6.1`

```console
$ docker pull logstash@sha256:e835cb319261fb9cdc102dfacaf7fdcdc357bd6b0f7b01f62e181a89c2443351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.6.1` - linux; amd64

```console
$ docker pull logstash@sha256:731c186d7ee6de7251a1a949b52c1488f1be7380c8a096a91e6c16c350b29c95
```

-	Docker Version: 20.10.22
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.9 MB (413854823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:675f42f60a0032db04ce1dfafacf698063e67dc5c06962862c5228a753fd628e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 10:58:38 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Tue, 24 Jan 2023 10:58:38 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Tue, 24 Jan 2023 10:59:00 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.6.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.6.1 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash
# Tue, 24 Jan 2023 10:59:03 GMT
WORKDIR /usr/share/logstash
# Tue, 24 Jan 2023 10:59:03 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 10:59:03 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 10:59:03 GMT
COPY file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Tue, 24 Jan 2023 10:59:03 GMT
COPY file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Tue, 24 Jan 2023 10:59:03 GMT
COPY file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Tue, 24 Jan 2023 10:59:03 GMT
COPY file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Tue, 24 Jan 2023 10:59:04 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Tue, 24 Jan 2023 10:59:04 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 24 Jan 2023 10:59:04 GMT
COPY file:65009cd6aa01133f279899826ce268f3a2f9e28442f3960b3ca7e7baeff08a84 in /usr/local/bin/ 
# Tue, 24 Jan 2023 10:59:04 GMT
COPY file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Tue, 24 Jan 2023 10:59:04 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Tue, 24 Jan 2023 10:59:05 GMT
USER 1000
# Tue, 24 Jan 2023 10:59:05 GMT
EXPOSE 5044 9600
# Tue, 24 Jan 2023 10:59:05 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.6.1 org.opencontainers.image.version=8.6.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-01-24T10:41:55+00:00 org.opencontainers.image.created=2023-01-24T10:41:55+00:00
# Tue, 24 Jan 2023 10:59:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b05278d4acde07e42cc4ad0dcd27b4035f9a7211b4004181bbe847f38fa818c`  
		Last Modified: Thu, 02 Feb 2023 01:14:29 GMT  
		Size: 41.4 MB (41363076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13694366de2a9c5b4e2bc7f18516d66c0d87d4e75bceb1bea08d1deaca1c1028`  
		Last Modified: Thu, 02 Feb 2023 01:14:24 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9633f1996718f65004b52540e5138fb01395697f93f544dd96755a075b461e`  
		Last Modified: Thu, 02 Feb 2023 01:14:50 GMT  
		Size: 342.1 MB (342137649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7214e727529d7d1c189c343bd2b94f1ce757df98de843ababbbae46dca66095`  
		Last Modified: Thu, 02 Feb 2023 01:14:24 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fbd7408eb857d3689c6b6109039d8f7dff5b8402d9ebec161e672c02f36217`  
		Last Modified: Thu, 02 Feb 2023 01:14:24 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67237f4b5fbe29b46827a768ebd4bdbad0dae77af5ab1adadddc970e674f139`  
		Last Modified: Thu, 02 Feb 2023 01:14:22 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36809248986ae4ff19e5d07d219dfcb377f6716271fbe32e5363abc5e81772a1`  
		Last Modified: Thu, 02 Feb 2023 01:14:22 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0823a8ad372b0eb8c2d41cb05c0a33f1c5b2ac704d834bf90f4229527f665ab`  
		Last Modified: Thu, 02 Feb 2023 01:14:22 GMT  
		Size: 2.7 KB (2696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4eee64495c95ccb8099d8454f2e3bed4225a4c35875fe2bf1c22972e8660f56`  
		Last Modified: Thu, 02 Feb 2023 01:14:22 GMT  
		Size: 1.8 MB (1770284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c9b95bd862318a5908081a934d8c48b7c359ca9e44266dd596815dfc16a72`  
		Last Modified: Thu, 02 Feb 2023 01:14:22 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c9b95bd862318a5908081a934d8c48b7c359ca9e44266dd596815dfc16a72`  
		Last Modified: Thu, 02 Feb 2023 01:14:22 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.6.1` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:fa71aaf9db0dec256499fb89d2e111bf67dfc3628f4e88ad1d8308bd322bd252
```

-	Docker Version: 20.10.22
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.5 MB (404488641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e3c0cdcc57a3700d9ca740a40388cc1128294c070a691202add838878d97ca0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 10:58:58 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Tue, 24 Jan 2023 10:58:59 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Tue, 24 Jan 2023 10:59:17 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.6.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.6.1 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash
# Tue, 24 Jan 2023 10:59:20 GMT
WORKDIR /usr/share/logstash
# Tue, 24 Jan 2023 10:59:20 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 10:59:20 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 10:59:21 GMT
COPY file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Tue, 24 Jan 2023 10:59:21 GMT
COPY file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Tue, 24 Jan 2023 10:59:21 GMT
COPY file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Tue, 24 Jan 2023 10:59:21 GMT
COPY file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Tue, 24 Jan 2023 10:59:21 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Tue, 24 Jan 2023 10:59:21 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 24 Jan 2023 10:59:21 GMT
COPY file:eb399118a6d96199662b2ad412aae33884620905c254dc04609d5c06a2fe27c0 in /usr/local/bin/ 
# Tue, 24 Jan 2023 10:59:22 GMT
COPY file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Tue, 24 Jan 2023 10:59:22 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Tue, 24 Jan 2023 10:59:22 GMT
USER 1000
# Tue, 24 Jan 2023 10:59:22 GMT
EXPOSE 5044 9600
# Tue, 24 Jan 2023 10:59:22 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.6.1 org.opencontainers.image.version=8.6.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-01-24T10:44:10+00:00 org.opencontainers.image.created=2023-01-24T10:44:10+00:00
# Tue, 24 Jan 2023 10:59:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cd0e6a56ffbe3e7c7061506d542d65017564a2cc7c738588a3d650086acf8f`  
		Last Modified: Wed, 01 Feb 2023 22:18:16 GMT  
		Size: 34.7 MB (34727989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e384894b2cc92d77285650046f9b2a7b42d9221a3b432c9c9b3bacf0e6750`  
		Last Modified: Wed, 01 Feb 2023 22:18:12 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459841013beeb9cddb80bc25b618f41bf1ec065934e599f87aa324101f6c087c`  
		Last Modified: Wed, 01 Feb 2023 22:18:34 GMT  
		Size: 340.9 MB (340911796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e478dbd9141067159cd9d852a51ed6c9208d739cc86600364fc4458ff1f0fde2`  
		Last Modified: Wed, 01 Feb 2023 22:18:12 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d399a516dd45a4af54fe043c2503b93376a7feeace6023e51fcac88684b70555`  
		Last Modified: Wed, 01 Feb 2023 22:18:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9e0057d340aa0a6523fb04aca174d5fb8e37d5a53a75ac5ccc73ecaa4640be`  
		Last Modified: Wed, 01 Feb 2023 22:18:10 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5150c96e62f9850defe11f2b374b4bb981578ba04e4be6f7946ae463f237a864`  
		Last Modified: Wed, 01 Feb 2023 22:18:10 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d7cbab05efc906e2fbecc1389cd7c215d18417a9e80f2a62a97c29752076f3`  
		Last Modified: Wed, 01 Feb 2023 22:18:10 GMT  
		Size: 2.7 KB (2699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9b378ff3a62ef8e6c71c1a0ef9d7ffd7ad0cbc3521311045a31cc03d2d89fc`  
		Last Modified: Wed, 01 Feb 2023 22:18:11 GMT  
		Size: 1.6 MB (1648732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adde5766a07a86f7ab6406213ff6e9779d457dc2b2a9d2a6e41d603348dc8ab3`  
		Last Modified: Wed, 01 Feb 2023 22:18:10 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adde5766a07a86f7ab6406213ff6e9779d457dc2b2a9d2a6e41d603348dc8ab3`  
		Last Modified: Wed, 01 Feb 2023 22:18:10 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
