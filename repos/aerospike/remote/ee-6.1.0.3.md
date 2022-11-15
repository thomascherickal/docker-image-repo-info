## `aerospike:ee-6.1.0.3`

```console
$ docker pull aerospike@sha256:523dc1dcff24d7bb152f421332d076d734c6f082433a87ac22fce292d13a7378
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-6.1.0.3` - linux; amd64

```console
$ docker pull aerospike@sha256:25e24b06ff8613ae850fbdfedb63439be8e4e874d767540c91c96674c70d2ffd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68170281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55b5e226143c09a6d3c341403ef803948ef4ff22a1d70ec2360e6e4d3c3ae0ae`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`
-	`SHELL`: `["\/bin\/bash","-o","pipefail","-c"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:19:20 GMT
ENV AEROSPIKE_VERSION=6.1.0.3
# Tue, 15 Nov 2022 10:19:20 GMT
ENV AEROSPIKE_SHA256=de62082abe7c5fb040fc5eaaed22274142d96cbcd7dfce7530a52d65bce8b277
# Tue, 15 Nov 2022 10:19:20 GMT
ENV AS_TINI_SHA256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940
# Tue, 15 Nov 2022 10:19:20 GMT
SHELL [/bin/bash -o pipefail -c]
# Tue, 15 Nov 2022 10:19:39 GMT
RUN export DEBIAN_FRONTEND=noninteractive   && apt-get update -y   && apt-get install -y --no-install-recommends     apt-utils     2>&1 | grep -v "delaying package configuration"   && apt-get install -y --no-install-recommends     binutils     ca-certificates     gettext-base     wget     xz-utils   && apt-get install -y --no-install-recommends     libcurl4     libldap-2.4.2   && wget https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static --progress=bar:force:noscroll -O /usr/bin/as-tini-static 2>&1   && echo "$AS_TINI_SHA256 /usr/bin/as-tini-static" | sha256sum -c -   && chmod +x /usr/bin/as-tini-static   && wget "https://artifacts.aerospike.com/aerospike-server-enterprise/${AEROSPIKE_VERSION}/aerospike-server-enterprise-${AEROSPIKE_VERSION}-debian11.tgz" --progress=bar:force:noscroll -O aerospike-server.tgz 2>&1   && echo "$AEROSPIKE_SHA256 aerospike-server.tgz" | sha256sum -c -   && mkdir -p aerospike/pkg   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && ar --output aerospike/pkg -x aerospike/aerospike-tools-*.deb   && tar xf aerospike/pkg/data.tar.xz -C aerospike/pkg/   && rm -rf aerospike-server.tgz /var/lib/apt/lists/*   && dpkg -r apt-utils binutils ca-certificates wget xz-utils   && dpkg --purge apt-utils binutils ca-certificates wget xz-utils 2>&1   && apt-get purge -y   && apt-get autoremove -y   && find aerospike/pkg/opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv aerospike/pkg/etc/aerospike/astools.conf /etc/aerospike   && if [ -d 'aerospike/pkg/opt/aerospike/bin/asadm' ]; then     mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/;     ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f /usr/lib/asadm/asinfo ]; then       ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;     fi   fi   && rm -rf /opt/aerospike/bin   && rm -rf aerospike
# Tue, 15 Nov 2022 10:19:39 GMT
COPY file:f56e2e33c0b4bb66affff75053eaed44661e723b8b33d3ef3c10e305b506c350 in /etc/aerospike/aerospike.template.conf 
# Tue, 15 Nov 2022 10:19:39 GMT
COPY file:954d06187376ade36d0a4daf43c9abe4806362f2f33f0bd9dbaef5a67c967bd3 in /entrypoint.sh 
# Tue, 15 Nov 2022 10:19:40 GMT
EXPOSE 3000 3001 3002
# Tue, 15 Nov 2022 10:19:40 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Tue, 15 Nov 2022 10:19:40 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e1e89544533e5cfeb8f506da9718a7f3164db7e8fa9ade0e6c455eb0fcc0c7`  
		Last Modified: Tue, 15 Nov 2022 10:20:16 GMT  
		Size: 36.8 MB (36755787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2839584911aa742e46d286753860796167851817604fc0680b9a6d5455eb7524`  
		Last Modified: Tue, 15 Nov 2022 10:20:10 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94e4b1f03eb0b5084caa3447334a1377edad2dea563a2cf860032e5ca13f2c9`  
		Last Modified: Tue, 15 Nov 2022 10:20:10 GMT  
		Size: 820.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
