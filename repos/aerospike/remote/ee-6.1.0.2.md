## `aerospike:ee-6.1.0.2`

```console
$ docker pull aerospike@sha256:ac60e71c51325a6ddd10b8338cb3e43aa03a9316bf1a26a33b72e42f6baf7ba9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ee-6.1.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:fb29d4885122cd54ea2f90b20adc40327448cafd46a75f7f144d3f1e127d1c37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 MB (123854182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d87f02a44b63d04f7e91c5ad7070d8e39af470fbf5eb052535b62daaa01b03`
-	Entrypoint: `["\/usr\/bin\/as-tini-static","-r","SIGUSR1","-t","SIGTERM","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:49:45 GMT
ENV AEROSPIKE_VERSION=6.1.0.2
# Wed, 05 Oct 2022 00:49:45 GMT
ENV AEROSPIKE_SHA256=efd49204813876c5b3b3064b875efccfd49fa2a7e4840161e411988fc87f012f
# Wed, 05 Oct 2022 00:49:45 GMT
ENV AS_TINI_SHA256=d1f6826dd70cdd88dde3d5a20d8ed248883a3bc2caba3071c8a3a9b0e0de5940
# Wed, 05 Oct 2022 00:50:21 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps wget python python3 python3-distutils lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget https://github.com/aerospike/tini/releases/download/1.0.1/as-tini-static -O /usr/bin/as-tini-static   && echo "$AS_TINI_SHA256 /usr/bin/as-tini-static" | sha256sum -c -   && chmod +x /usr/bin/as-tini-static   && wget "https://download.aerospike.com/artifacts/aerospike-server-enterprise/${AEROSPIKE_VERSION}/aerospike-server-enterprise-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && if [ -d '/opt/aerospike/bin/asadm' ];   then   mv /opt/aerospike/bin/asadm /usr/lib/;   ln -s /usr/lib/asadm/asadm /usr/bin/asadm;     if [ -f /usr/lib/asadm/asinfo ];     then     ln -s /usr/lib/asadm/asinfo /usr/bin/asinfo;     fi   fi   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 05 Oct 2022 00:50:22 GMT
COPY file:f56e2e33c0b4bb66affff75053eaed44661e723b8b33d3ef3c10e305b506c350 in /etc/aerospike/aerospike.template.conf 
# Wed, 05 Oct 2022 00:50:22 GMT
COPY file:697e2123680798e87da7a3f98d1d70e76ffec66f0e1aafa90ff25047a11cca52 in /entrypoint.sh 
# Wed, 05 Oct 2022 00:50:22 GMT
EXPOSE 3000 3001 3002
# Wed, 05 Oct 2022 00:50:22 GMT
ENTRYPOINT ["/usr/bin/as-tini-static" "-r" "SIGUSR1" "-t" "SIGTERM" "--" "/entrypoint.sh"]
# Wed, 05 Oct 2022 00:50:22 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8966432d370bf892046da7b626992459e19204e0df468e7cf820a71c07fbac`  
		Last Modified: Wed, 05 Oct 2022 00:51:15 GMT  
		Size: 96.7 MB (96714253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b142a52a4fccd383af862e878aa43c129fae2b5fc25e1e990b9d87e36a8f47`  
		Last Modified: Wed, 05 Oct 2022 00:51:01 GMT  
		Size: 1.0 KB (1046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa683204949ffbf7ea950843fa29f80385d6fca10326d615160c766d1f36ae8`  
		Last Modified: Wed, 05 Oct 2022 00:51:01 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
