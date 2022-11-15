## `aerospike:ce-6.1.0.3`

```console
$ docker pull aerospike@sha256:c3d1d22c757f548a32a9f04ee13d3d7498600ff94644f5d458c35856ccb77f1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-6.1.0.3` - linux; amd64

```console
$ docker pull aerospike@sha256:df2121ec6655002ac3484fe97f53cf55a73d3a121327bc63a3d98de8a4dca05f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65133642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c45eb5e42680bd1532b7fea89e8b194f33040192e704570f7a3cf01f878323b7`
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
# Tue, 15 Nov 2022 10:19:44 GMT
ENV AEROSPIKE_SHA256=e4f9c152209547517951b78e42ca0251bd237fe1eba65b7bef81fea94ab653c9
# Tue, 15 Nov 2022 10:19:44 GMT
ENV AS_TINI_SHA256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940
# Tue, 15 Nov 2022 10:19:44 GMT
SHELL [/bin/bash -o pipefail -c]
# Tue, 15 Nov 2022 10:19:59 GMT
RUN export DEBIAN_FRONTEND=noninteractive   && apt-get update -y   && apt-get install -y --no-install-recommends     apt-utils     2>&1 | grep -v "delaying package configuration"   && apt-get install -y --no-install-recommends     binutils     ca-certificates     gettext-base     wget     xz-utils   && wget https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static --progress=bar:force:noscroll -O /usr/bin/as-tini-static 2>&1   && echo "$AS_TINI_SHA256 /usr/bin/as-tini-static" | sha256sum -c -   && chmod +x /usr/bin/as-tini-static   && wget "https://artifacts.aerospike.com/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian11.tgz" --progress=bar:force:noscroll -O aerospike-server.tgz 2>&1   && echo "$AEROSPIKE_SHA256 aerospike-server.tgz" | sha256sum -c -   && mkdir -p aerospike/pkg   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && ar --output aerospike/pkg -x aerospike/aerospike-tools-*.deb   && tar xf aerospike/pkg/data.tar.xz -C aerospike/pkg/   && rm -rf aerospike-server.tgz /var/lib/apt/lists/*   && dpkg -r apt-utils binutils ca-certificates wget xz-utils   && dpkg --purge apt-utils binutils ca-certificates wget xz-utils 2>&1   && apt-get purge -y   && apt-get autoremove -y   && find aerospike/pkg/opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv aerospike/pkg/etc/aerospike/astools.conf /etc/aerospike   && if [ -d 'aerospike/pkg/opt/aerospike/bin/asadm' ]; then     mv aerospike/pkg/opt/aerospike/bin/asadm /usr/lib/;     ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f /usr/lib/asadm/asinfo ]; then       ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;     fi   fi   && rm -rf /opt/aerospike/bin   && rm -rf aerospike
# Tue, 15 Nov 2022 10:19:59 GMT
COPY file:f497c4c6974a190f79a562efd9c9c0d6b753efe43e62c3fcc2536f74ad08238d in /etc/aerospike/aerospike.template.conf 
# Tue, 15 Nov 2022 10:19:59 GMT
COPY file:e3973656bf47d8e3796d7b5dc7200e68dcaedc877c80f4ebeed9484f3aa315d9 in /entrypoint.sh 
# Tue, 15 Nov 2022 10:19:59 GMT
EXPOSE 3000 3001 3002
# Tue, 15 Nov 2022 10:19:59 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Tue, 15 Nov 2022 10:19:59 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8d1d2a501616a287ba777d2a88b9bae058cc0313cea2128f542806c1b14cb0`  
		Last Modified: Tue, 15 Nov 2022 10:20:27 GMT  
		Size: 33.7 MB (33719208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c144dac2e99a78c46966b1ba61225b35a843573713b97934dae6451adc6534`  
		Last Modified: Tue, 15 Nov 2022 10:20:22 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c7177a97a5a1653802950306c62dbfbbf577e51d75a58977bdeeb70165583`  
		Last Modified: Tue, 15 Nov 2022 10:20:22 GMT  
		Size: 788.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
