## `chronograf:latest`

```console
$ docker pull chronograf@sha256:140637b8e1580537e9994f1106e9357d338fb90a618af5e40b7d790f9c1a6f16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `chronograf:latest` - linux; amd64

```console
$ docker pull chronograf@sha256:0b09bb3ab83804f13964ec13973c6752745c6e7374e2f108b199a7cab9dafa8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82809853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9c4ef1906cc7a549cd792acc68c61601d5c2684f197a29ad60901bd13f791b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:13 GMT
ADD file:cb5fcc80c057b356a31492a20c6e3a75b70ed70a663506c8e97ad730ae32a02d in / 
# Thu, 07 Sep 2023 00:21:13 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 15:16:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 15:17:08 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 07 Sep 2023 15:17:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 15:17:15 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 07 Sep 2023 15:17:15 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 07 Sep 2023 15:17:15 GMT
EXPOSE 8888
# Thu, 07 Sep 2023 15:17:15 GMT
VOLUME [/var/lib/chronograf]
# Thu, 07 Sep 2023 15:17:15 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 07 Sep 2023 15:17:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 15:17:15 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:7d97e254a0461b0a30b3f443f1daa0d620a3cc6ff4e2714cc1cfd96ace5b7a7e`  
		Last Modified: Thu, 07 Sep 2023 00:26:03 GMT  
		Size: 31.4 MB (31417503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f551166512b9726b9b273f852ee365881f71796018c2b70c3342431c6233715a`  
		Last Modified: Thu, 07 Sep 2023 15:17:49 GMT  
		Size: 5.2 MB (5226401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c87ef7c1b350dc0a74cb92bfa144648128f3ad59e777eeaf58e62c9033b91ba`  
		Last Modified: Thu, 07 Sep 2023 15:18:22 GMT  
		Size: 46.1 MB (46141560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a452f99e1afb0aa9f72f9f8a5b30cf21d66ebed4c9781ec482706291453ec4`  
		Last Modified: Thu, 07 Sep 2023 15:18:16 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db9016fb2274a5a4a434850f603ec956b29e97830ce190d789b12c9a886e73e`  
		Last Modified: Thu, 07 Sep 2023 15:18:16 GMT  
		Size: 11.9 KB (11904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396b9545b2ad3b2f4e98bc5f16760ab4337545437cdb228dd62b0a53f19647dc`  
		Last Modified: Thu, 07 Sep 2023 15:18:16 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm variant v7

```console
$ docker pull chronograf@sha256:879c2dcedde6dbc3f7ffdefe5dc4499f93b769172d2c9a7f7059f777f28dc29b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74945438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adbbfd75c83cd2870d449d6763fa33731c00e6d63279b848f0c7f8cac9521844`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:09 GMT
ADD file:d714939aacc810de397a02461ce4b9dd85e92783aff066bd3da685e3d2d97439 in / 
# Thu, 07 Sep 2023 00:58:10 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:53:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 01:54:17 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 07 Sep 2023 01:54:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:54:28 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 07 Sep 2023 01:54:28 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 07 Sep 2023 01:54:28 GMT
EXPOSE 8888
# Thu, 07 Sep 2023 01:54:28 GMT
VOLUME [/var/lib/chronograf]
# Thu, 07 Sep 2023 01:54:29 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 07 Sep 2023 01:54:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 01:54:29 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:323242406c24248128abc25e113055d272350b4ac4ecd985dbabfb7061c48d49`  
		Last Modified: Thu, 07 Sep 2023 01:03:12 GMT  
		Size: 26.6 MB (26578710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97c2b71d52540a29adf80cc6b59cbf80b92dc95748101dde3c9199ff19b0918`  
		Last Modified: Thu, 07 Sep 2023 01:54:59 GMT  
		Size: 4.5 MB (4491966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fd8ade4fd5a0228bfb06318218f24ea1c3ec842ed84637056a04502347653b`  
		Last Modified: Thu, 07 Sep 2023 01:55:30 GMT  
		Size: 43.9 MB (43850372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9797c093114c1e733b705d751b1de7c57de5c5cda7e88fb7486d3b392ab0ec`  
		Last Modified: Thu, 07 Sep 2023 01:55:23 GMT  
		Size: 12.2 KB (12245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dce1708038b03b04ebcd54580d9f51a3b33020a201c42671cf01235dbde4e3`  
		Last Modified: Thu, 07 Sep 2023 01:55:23 GMT  
		Size: 11.9 KB (11905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e3e2689179a0af25e4288df97127c30b602245316689af6b632404d2b827ab`  
		Last Modified: Thu, 07 Sep 2023 01:55:24 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `chronograf:latest` - linux; arm64 variant v8

```console
$ docker pull chronograf@sha256:bf698fb783f1c4428a87de66e886658ee267a4c2eade14d5e0716ded1cc3b37b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79151446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6a9c75f6b7d45127c8d11aca9d170bfc16853f0014e17a67ad4bc619601908`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["chronograf"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:59:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apt-get update && apt-get install -y gnupg ca-certificates dirmngr --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 07 Sep 2023 01:59:35 GMT
ENV CHRONOGRAF_VERSION=1.10.1
# Thu, 07 Sep 2023 01:59:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     set -x &&     apt-get update && apt-get install -y ca-certificates curl --no-install-recommends &&     rm -rf /var/lib/apt/lists/* &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc" &&     curl -SLO "https://dl.influxdata.com/chronograf/releases/chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb" &&     gpg --batch --verify chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb.asc chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     dpkg -i chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb &&     rm -f chronograf_${CHRONOGRAF_VERSION}_${ARCH}.deb* &&     apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:59:47 GMT
COPY file:6403df1bf15a98453f66ca6b38ee538c184409065ea1d3c321788dec9eaa5c77 in /usr/share/chronograf/LICENSE 
# Thu, 07 Sep 2023 01:59:47 GMT
COPY file:6a5854b87d89e3055231dd56f8f199c325f44eeed8faed4cf32833126a5b9cd9 in /usr/share/chronograf/agpl-3.0.md 
# Thu, 07 Sep 2023 01:59:47 GMT
EXPOSE 8888
# Thu, 07 Sep 2023 01:59:47 GMT
VOLUME [/var/lib/chronograf]
# Thu, 07 Sep 2023 01:59:47 GMT
COPY file:7ce45912f7e80a04754c20ff31c757dd5de5eb9a5845af3b183b4a5227dd1c1e in /entrypoint.sh 
# Thu, 07 Sep 2023 01:59:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 07 Sep 2023 01:59:47 GMT
CMD ["chronograf"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c7773eabba056f94a266442f4d1121f905c1f4e838e60933e6b13d719c9660`  
		Last Modified: Thu, 07 Sep 2023 02:00:15 GMT  
		Size: 5.2 MB (5209305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb629f3a3f4b9bdd9de75e6c74a535c5cd97c1ea47dd26f3d3585b591d659e1d`  
		Last Modified: Thu, 07 Sep 2023 02:00:42 GMT  
		Size: 43.9 MB (43854844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b64f7f062d350e173ee9962e37dcbbe69887efa8969964e61315b63a788d849`  
		Last Modified: Thu, 07 Sep 2023 02:00:38 GMT  
		Size: 12.2 KB (12248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b9c9f97f10efe247e1be05cc88418f286ffb252493611736705898b3ea73d1`  
		Last Modified: Thu, 07 Sep 2023 02:00:38 GMT  
		Size: 11.9 KB (11907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1ac651f5f7c32999a87addacd34e8ec07e0eebdc00c09f15a55537935bf979`  
		Last Modified: Thu, 07 Sep 2023 02:00:38 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
