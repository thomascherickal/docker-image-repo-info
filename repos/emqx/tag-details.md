<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `emqx`

-	[`emqx:4`](#emqx4)
-	[`emqx:4.3`](#emqx43)
-	[`emqx:4.3.22`](#emqx4322)
-	[`emqx:4.4`](#emqx44)
-	[`emqx:4.4.14`](#emqx4414)
-	[`emqx:5`](#emqx5)
-	[`emqx:5.0`](#emqx50)
-	[`emqx:5.0.16`](#emqx5016)
-	[`emqx:latest`](#emqxlatest)

## `emqx:4`

```console
$ docker pull emqx@sha256:b885c2942827f2de9875c0ffc0b2d96a70534378514676dcb8a89e1834282836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4` - linux; amd64

```console
$ docker pull emqx@sha256:b9e00a0594bfa618da93b3732f15cdd44607d352cd709b3c80cf12d2023f7a4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81178265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc81f95bd1c990a7ce0c3b72644b7020eec4d16ba23b26334f5f8c97a718096f`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 10:08:30 GMT
ENV EMQX_VERSION=4.4.14
# Thu, 09 Feb 2023 10:08:30 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 09 Feb 2023 10:08:35 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 10:08:36 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:36 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 10:08:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e287081db8a87dd0c4bc906aab9ec66ae29d474ecf5b1b9f74d58f29508246f8`  
		Last Modified: Thu, 09 Feb 2023 10:09:28 GMT  
		Size: 2.6 MB (2569458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1d7eea27095717fd0ec4493a63bbb2948479760c1416348aa1416f56de3f7a`  
		Last Modified: Thu, 09 Feb 2023 10:09:28 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c491150cca28c041b02397fcfda72fb6d175fc40fe55324b1fb2cba83afe3c1f`  
		Last Modified: Thu, 09 Feb 2023 10:09:33 GMT  
		Size: 47.2 MB (47191775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa34193ac495277a6ffd8f1f99e2f483c4b00e87fe42ca586078917aa82b7ea`  
		Last Modified: Thu, 09 Feb 2023 10:09:28 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:f1c083942ac25a82b0ca92172d0e9db7076dd1bced0b6f50a2db2d0491830bf2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72602820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffd65711efce49b512b5b9d20be35d2b3dc47c5bcc3b90ee0ec319a3bb9ae08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:40:49 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:40:49 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 09:40:49 GMT
ENV EMQX_VERSION=4.4.14
# Thu, 09 Feb 2023 09:40:49 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 09 Feb 2023 09:40:53 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 09:40:53 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:40:53 GMT
USER emqx
# Thu, 09 Feb 2023 09:40:54 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:40:54 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 09:40:54 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 09 Feb 2023 09:40:54 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:40:54 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3867239bfba19f43467d153fbc9ce80013ca9aa3afe6cd6462125843d3ba288`  
		Last Modified: Thu, 09 Feb 2023 09:41:34 GMT  
		Size: 2.6 MB (2559196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2694a14cbe1093cc3cb46d69b34ecb35e4bc2cc2e4769a6e0d55abb8a1b0c443`  
		Last Modified: Thu, 09 Feb 2023 09:41:33 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7263c6478ce08f0dcf66f54563da9696efd93a3e38f3908582560db5d87b033`  
		Last Modified: Thu, 09 Feb 2023 09:41:37 GMT  
		Size: 40.0 MB (39975888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bbc98ec1b1da7658b5747405e08ef124bae7393b92bd3505dd33dcfec2b42b`  
		Last Modified: Thu, 09 Feb 2023 09:41:33 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3`

```console
$ docker pull emqx@sha256:7f9a2002156db03d5529ee8da2d8e4ee4f3c8f6d9ddcb5e50c63af8fbaf86c42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3` - linux; amd64

```console
$ docker pull emqx@sha256:ebc0587bb666ab2bd3b3c947bea4c3c55a03b52617019e006fe09227a7f5207c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68297278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e1c4cc15d83e4d1fe010ab0ed0998d075bc0df629b82441d78603d3ce1d9d7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 10:08:13 GMT
ENV EMQX_VERSION=4.3.22
# Thu, 09 Feb 2023 10:08:18 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 10:08:19 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:19 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:19 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:19 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 10:08:19 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:19 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fb7ffe7ac41fa03959ff1a7c7100f9b6cd5697f8b33be38282fd44ce420b93`  
		Last Modified: Thu, 09 Feb 2023 10:09:16 GMT  
		Size: 4.6 MB (4612872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4af828b19ca7fea5bf51f0987fe907d8a1ae8ea965a06cd574ad99b5c8193a`  
		Last Modified: Thu, 09 Feb 2023 10:09:15 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d877c601c16dabeda04346f0cb89d32f400aa925fbe2a0036d96dc5431f4ce`  
		Last Modified: Thu, 09 Feb 2023 10:09:19 GMT  
		Size: 36.5 MB (36538721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfc7e26d4c2ba3ba7464b7544ce75dcdddce24326262db675877eb859d82990`  
		Last Modified: Thu, 09 Feb 2023 10:09:15 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:dd50337913b99be60dc739a033deb1ce3576074fa5d42187b64464bc42243b88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66636558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9382f01e19164573b838c50ca0bb90af1e944de91f30fe089b8aaab0d00c8ca3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:40:36 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:40:37 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 09:40:37 GMT
ENV EMQX_VERSION=4.3.22
# Thu, 09 Feb 2023 09:40:41 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 09:40:41 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:40:41 GMT
USER emqx
# Thu, 09 Feb 2023 09:40:41 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:40:41 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 09:40:42 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Thu, 09 Feb 2023 09:40:42 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:40:42 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3761492c946737d92142b86f8a712e511128b1fb16b77e415ca93c7b3e477b21`  
		Last Modified: Thu, 09 Feb 2023 09:41:22 GMT  
		Size: 4.5 MB (4490722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e966573db76618e6ceb16ab2e4d9aa5b6eeb54918e5ecb75bdad9e268b0d073b`  
		Last Modified: Thu, 09 Feb 2023 09:41:21 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f7c97a2ea55acf09f523ca259acc2189881dd9f78a21bb6bb373497de81e38`  
		Last Modified: Thu, 09 Feb 2023 09:41:25 GMT  
		Size: 36.2 MB (36217852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2123dd835039f7389696ddc988db4349a8b21a4751edae93de50d3eb63a3745f`  
		Last Modified: Thu, 09 Feb 2023 09:41:21 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.3.22`

```console
$ docker pull emqx@sha256:7f9a2002156db03d5529ee8da2d8e4ee4f3c8f6d9ddcb5e50c63af8fbaf86c42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.3.22` - linux; amd64

```console
$ docker pull emqx@sha256:ebc0587bb666ab2bd3b3c947bea4c3c55a03b52617019e006fe09227a7f5207c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68297278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e1c4cc15d83e4d1fe010ab0ed0998d075bc0df629b82441d78603d3ce1d9d7`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:13 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:13 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 10:08:13 GMT
ENV EMQX_VERSION=4.3.22
# Thu, 09 Feb 2023 10:08:18 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 10:08:19 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:19 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:19 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:19 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 10:08:19 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:19 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:19 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fb7ffe7ac41fa03959ff1a7c7100f9b6cd5697f8b33be38282fd44ce420b93`  
		Last Modified: Thu, 09 Feb 2023 10:09:16 GMT  
		Size: 4.6 MB (4612872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4af828b19ca7fea5bf51f0987fe907d8a1ae8ea965a06cd574ad99b5c8193a`  
		Last Modified: Thu, 09 Feb 2023 10:09:15 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d877c601c16dabeda04346f0cb89d32f400aa925fbe2a0036d96dc5431f4ce`  
		Last Modified: Thu, 09 Feb 2023 10:09:19 GMT  
		Size: 36.5 MB (36538721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfc7e26d4c2ba3ba7464b7544ce75dcdddce24326262db675877eb859d82990`  
		Last Modified: Thu, 09 Feb 2023 10:09:15 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.3.22` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:dd50337913b99be60dc739a033deb1ce3576074fa5d42187b64464bc42243b88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66636558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9382f01e19164573b838c50ca0bb90af1e944de91f30fe089b8aaab0d00c8ca3`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:40:36 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:40:37 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 09:40:37 GMT
ENV EMQX_VERSION=4.3.22
# Thu, 09 Feb 2023 09:40:41 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="e5f6874eb29f83cce9c84afae95cc05de11ed8aa47f046783afa1c75e812a4b7"; fi;     if [ ${arch} = "arm64" ]; then sha256="85bf586fdf1c11f4057f6137faa4390100a3f3eb0e285e8a68e63c7d15bea09b"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${ID}${VERSION_ID}-${EMQX_VERSION}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 09:40:41 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:40:41 GMT
USER emqx
# Thu, 09 Feb 2023 09:40:41 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:40:41 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 09:40:42 GMT
COPY file:715d536465bb73dc7e7d11b7af4806884602823836c36e9ec561de98ccbf3424 in /usr/bin/ 
# Thu, 09 Feb 2023 09:40:42 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:40:42 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3761492c946737d92142b86f8a712e511128b1fb16b77e415ca93c7b3e477b21`  
		Last Modified: Thu, 09 Feb 2023 09:41:22 GMT  
		Size: 4.5 MB (4490722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e966573db76618e6ceb16ab2e4d9aa5b6eeb54918e5ecb75bdad9e268b0d073b`  
		Last Modified: Thu, 09 Feb 2023 09:41:21 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f7c97a2ea55acf09f523ca259acc2189881dd9f78a21bb6bb373497de81e38`  
		Last Modified: Thu, 09 Feb 2023 09:41:25 GMT  
		Size: 36.2 MB (36217852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2123dd835039f7389696ddc988db4349a8b21a4751edae93de50d3eb63a3745f`  
		Last Modified: Thu, 09 Feb 2023 09:41:21 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4`

```console
$ docker pull emqx@sha256:b885c2942827f2de9875c0ffc0b2d96a70534378514676dcb8a89e1834282836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4` - linux; amd64

```console
$ docker pull emqx@sha256:b9e00a0594bfa618da93b3732f15cdd44607d352cd709b3c80cf12d2023f7a4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81178265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc81f95bd1c990a7ce0c3b72644b7020eec4d16ba23b26334f5f8c97a718096f`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 10:08:30 GMT
ENV EMQX_VERSION=4.4.14
# Thu, 09 Feb 2023 10:08:30 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 09 Feb 2023 10:08:35 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 10:08:36 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:36 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 10:08:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e287081db8a87dd0c4bc906aab9ec66ae29d474ecf5b1b9f74d58f29508246f8`  
		Last Modified: Thu, 09 Feb 2023 10:09:28 GMT  
		Size: 2.6 MB (2569458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1d7eea27095717fd0ec4493a63bbb2948479760c1416348aa1416f56de3f7a`  
		Last Modified: Thu, 09 Feb 2023 10:09:28 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c491150cca28c041b02397fcfda72fb6d175fc40fe55324b1fb2cba83afe3c1f`  
		Last Modified: Thu, 09 Feb 2023 10:09:33 GMT  
		Size: 47.2 MB (47191775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa34193ac495277a6ffd8f1f99e2f483c4b00e87fe42ca586078917aa82b7ea`  
		Last Modified: Thu, 09 Feb 2023 10:09:28 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:f1c083942ac25a82b0ca92172d0e9db7076dd1bced0b6f50a2db2d0491830bf2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72602820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffd65711efce49b512b5b9d20be35d2b3dc47c5bcc3b90ee0ec319a3bb9ae08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:40:49 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:40:49 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 09:40:49 GMT
ENV EMQX_VERSION=4.4.14
# Thu, 09 Feb 2023 09:40:49 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 09 Feb 2023 09:40:53 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 09:40:53 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:40:53 GMT
USER emqx
# Thu, 09 Feb 2023 09:40:54 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:40:54 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 09:40:54 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 09 Feb 2023 09:40:54 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:40:54 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3867239bfba19f43467d153fbc9ce80013ca9aa3afe6cd6462125843d3ba288`  
		Last Modified: Thu, 09 Feb 2023 09:41:34 GMT  
		Size: 2.6 MB (2559196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2694a14cbe1093cc3cb46d69b34ecb35e4bc2cc2e4769a6e0d55abb8a1b0c443`  
		Last Modified: Thu, 09 Feb 2023 09:41:33 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7263c6478ce08f0dcf66f54563da9696efd93a3e38f3908582560db5d87b033`  
		Last Modified: Thu, 09 Feb 2023 09:41:37 GMT  
		Size: 40.0 MB (39975888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bbc98ec1b1da7658b5747405e08ef124bae7393b92bd3505dd33dcfec2b42b`  
		Last Modified: Thu, 09 Feb 2023 09:41:33 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:4.4.14`

```console
$ docker pull emqx@sha256:b885c2942827f2de9875c0ffc0b2d96a70534378514676dcb8a89e1834282836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:4.4.14` - linux; amd64

```console
$ docker pull emqx@sha256:b9e00a0594bfa618da93b3732f15cdd44607d352cd709b3c80cf12d2023f7a4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81178265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc81f95bd1c990a7ce0c3b72644b7020eec4d16ba23b26334f5f8c97a718096f`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:29 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:30 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 10:08:30 GMT
ENV EMQX_VERSION=4.4.14
# Thu, 09 Feb 2023 10:08:30 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 09 Feb 2023 10:08:35 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 10:08:36 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:36 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:36 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:36 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 10:08:36 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:36 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:36 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e287081db8a87dd0c4bc906aab9ec66ae29d474ecf5b1b9f74d58f29508246f8`  
		Last Modified: Thu, 09 Feb 2023 10:09:28 GMT  
		Size: 2.6 MB (2569458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1d7eea27095717fd0ec4493a63bbb2948479760c1416348aa1416f56de3f7a`  
		Last Modified: Thu, 09 Feb 2023 10:09:28 GMT  
		Size: 4.1 KB (4112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c491150cca28c041b02397fcfda72fb6d175fc40fe55324b1fb2cba83afe3c1f`  
		Last Modified: Thu, 09 Feb 2023 10:09:33 GMT  
		Size: 47.2 MB (47191775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa34193ac495277a6ffd8f1f99e2f483c4b00e87fe42ca586078917aa82b7ea`  
		Last Modified: Thu, 09 Feb 2023 10:09:28 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:4.4.14` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:f1c083942ac25a82b0ca92172d0e9db7076dd1bced0b6f50a2db2d0491830bf2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72602820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffd65711efce49b512b5b9d20be35d2b3dc47c5bcc3b90ee0ec319a3bb9ae08`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:40:49 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl unzip ca-certificates;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:40:49 GMT
RUN set -eu;     groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx
# Thu, 09 Feb 2023 09:40:49 GMT
ENV EMQX_VERSION=4.4.14
# Thu, 09 Feb 2023 09:40:49 GMT
ENV OTP=otp24.3.4.2-1
# Thu, 09 Feb 2023 09:40:53 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="b70590c16effa60759f6ab08a4a0e666ad4487cf0eb88263ab992e44b440b815"; fi;     if [ ${arch} = "arm64" ]; then sha256="98b78798577ddb7685c42dc41b7a758aacfe27924c8be4510e2057527a142ba0"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${OTP}-${ID}${VERSION_ID}-${arch}.zip";     curl -f -O -L https://www.emqx.com/en/downloads/broker/${EMQX_VERSION}/${pkg};     echo "$sha256 *$pkg" | sha256sum -c || exit 1;     unzip -q -d /opt $pkg;     chgrp -Rf emqx /opt/emqx;     chmod -Rf g+w /opt/emqx;     chown -Rf emqx /opt/emqx;     ln -s /opt/emqx/bin/* /usr/local/bin/;     rm -rf $pkg
# Thu, 09 Feb 2023 09:40:53 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:40:53 GMT
USER emqx
# Thu, 09 Feb 2023 09:40:54 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:40:54 GMT
EXPOSE 11883 18083 1883 4369 4370 5369 6369 6370 8081 8083 8084 8883
# Thu, 09 Feb 2023 09:40:54 GMT
COPY file:6dd7e4492be7572c69a0409bd663714c620b2048d81308e1877901073db7f426 in /usr/bin/ 
# Thu, 09 Feb 2023 09:40:54 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:40:54 GMT
CMD ["emqx" "foreground"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3867239bfba19f43467d153fbc9ce80013ca9aa3afe6cd6462125843d3ba288`  
		Last Modified: Thu, 09 Feb 2023 09:41:34 GMT  
		Size: 2.6 MB (2559196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2694a14cbe1093cc3cb46d69b34ecb35e4bc2cc2e4769a6e0d55abb8a1b0c443`  
		Last Modified: Thu, 09 Feb 2023 09:41:33 GMT  
		Size: 4.1 KB (4117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7263c6478ce08f0dcf66f54563da9696efd93a3e38f3908582560db5d87b033`  
		Last Modified: Thu, 09 Feb 2023 09:41:37 GMT  
		Size: 40.0 MB (39975888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bbc98ec1b1da7658b5747405e08ef124bae7393b92bd3505dd33dcfec2b42b`  
		Last Modified: Thu, 09 Feb 2023 09:41:33 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5`

```console
$ docker pull emqx@sha256:601c82ac0495ad758003d337c90c4f2cf408c4e85c995e611344b081c09c02c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5` - linux; amd64

```console
$ docker pull emqx@sha256:7d87307488a966746ab49e68e98eb65517db733af54cf209a6d927cb7648d941
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100346619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56505e666d708b81be558f0c7e2ed02b77138943b147fa9eb226ce895ec0151`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:46 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 10:08:46 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 10:08:46 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 10:08:46 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 10:08:46 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 10:08:58 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 10:08:58 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:58 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:59 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:59 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 10:08:59 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:59 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:59 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc09b4c23409fc6e30f1f0933f0f2c6bd9d7a6566ed0054cb6583015adff6a07`  
		Last Modified: Thu, 09 Feb 2023 10:09:44 GMT  
		Size: 3.0 MB (2987646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5690e645d1f946b924e8d76142ecfdece6e52665554c1a7e613091d6885878`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8d953ea948855c1f2fb3f57b7d7c23e9736c453bad99369844efe4dc499ffd`  
		Last Modified: Thu, 09 Feb 2023 10:09:51 GMT  
		Size: 65.9 MB (65942145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5687a1533ec033755e06b7c820a08146f8677a51fee7416c28de93a5f31ae6d5`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:34ca0ce3077d1e2d1d46e231a442ea68b8f8b695a08f3278c39538fe54ea25c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91443872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dbae1937e6637a793bdc65e2d083cd920472c28c6e242b811a8921b05d6d108`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:41:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:41:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 09:41:01 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 09:41:01 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 09:41:01 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 09:41:01 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 09:41:06 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 09:41:07 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:41:07 GMT
USER emqx
# Thu, 09 Feb 2023 09:41:07 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:41:07 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 09:41:07 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 09:41:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:41:07 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5394f2f4b016df4b79fc515dbf7cd492b3dbe93b959baf39817d26676ae083`  
		Last Modified: Thu, 09 Feb 2023 09:41:48 GMT  
		Size: 3.0 MB (3002749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def267c4d834a0cd84dd88a877e1c746c0a38d9d4b39043b22f599b1a6b9e6b9`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f45e39fe16597c4cd113c4c6390cec4adadb72279e5937cfd5ebf925d3f50d`  
		Last Modified: Thu, 09 Feb 2023 09:41:55 GMT  
		Size: 58.4 MB (58373594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0b8c7e3854a4c45110a7bac48de29bb922a8660f7d4ed1855ce44364cdff81`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0`

```console
$ docker pull emqx@sha256:601c82ac0495ad758003d337c90c4f2cf408c4e85c995e611344b081c09c02c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0` - linux; amd64

```console
$ docker pull emqx@sha256:7d87307488a966746ab49e68e98eb65517db733af54cf209a6d927cb7648d941
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100346619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56505e666d708b81be558f0c7e2ed02b77138943b147fa9eb226ce895ec0151`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:46 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 10:08:46 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 10:08:46 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 10:08:46 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 10:08:46 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 10:08:58 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 10:08:58 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:58 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:59 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:59 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 10:08:59 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:59 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:59 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc09b4c23409fc6e30f1f0933f0f2c6bd9d7a6566ed0054cb6583015adff6a07`  
		Last Modified: Thu, 09 Feb 2023 10:09:44 GMT  
		Size: 3.0 MB (2987646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5690e645d1f946b924e8d76142ecfdece6e52665554c1a7e613091d6885878`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8d953ea948855c1f2fb3f57b7d7c23e9736c453bad99369844efe4dc499ffd`  
		Last Modified: Thu, 09 Feb 2023 10:09:51 GMT  
		Size: 65.9 MB (65942145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5687a1533ec033755e06b7c820a08146f8677a51fee7416c28de93a5f31ae6d5`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:34ca0ce3077d1e2d1d46e231a442ea68b8f8b695a08f3278c39538fe54ea25c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91443872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dbae1937e6637a793bdc65e2d083cd920472c28c6e242b811a8921b05d6d108`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:41:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:41:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 09:41:01 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 09:41:01 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 09:41:01 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 09:41:01 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 09:41:06 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 09:41:07 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:41:07 GMT
USER emqx
# Thu, 09 Feb 2023 09:41:07 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:41:07 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 09:41:07 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 09:41:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:41:07 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5394f2f4b016df4b79fc515dbf7cd492b3dbe93b959baf39817d26676ae083`  
		Last Modified: Thu, 09 Feb 2023 09:41:48 GMT  
		Size: 3.0 MB (3002749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def267c4d834a0cd84dd88a877e1c746c0a38d9d4b39043b22f599b1a6b9e6b9`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f45e39fe16597c4cd113c4c6390cec4adadb72279e5937cfd5ebf925d3f50d`  
		Last Modified: Thu, 09 Feb 2023 09:41:55 GMT  
		Size: 58.4 MB (58373594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0b8c7e3854a4c45110a7bac48de29bb922a8660f7d4ed1855ce44364cdff81`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:5.0.16`

```console
$ docker pull emqx@sha256:601c82ac0495ad758003d337c90c4f2cf408c4e85c995e611344b081c09c02c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:5.0.16` - linux; amd64

```console
$ docker pull emqx@sha256:7d87307488a966746ab49e68e98eb65517db733af54cf209a6d927cb7648d941
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100346619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56505e666d708b81be558f0c7e2ed02b77138943b147fa9eb226ce895ec0151`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:46 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 10:08:46 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 10:08:46 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 10:08:46 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 10:08:46 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 10:08:58 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 10:08:58 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:58 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:59 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:59 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 10:08:59 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:59 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:59 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc09b4c23409fc6e30f1f0933f0f2c6bd9d7a6566ed0054cb6583015adff6a07`  
		Last Modified: Thu, 09 Feb 2023 10:09:44 GMT  
		Size: 3.0 MB (2987646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5690e645d1f946b924e8d76142ecfdece6e52665554c1a7e613091d6885878`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8d953ea948855c1f2fb3f57b7d7c23e9736c453bad99369844efe4dc499ffd`  
		Last Modified: Thu, 09 Feb 2023 10:09:51 GMT  
		Size: 65.9 MB (65942145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5687a1533ec033755e06b7c820a08146f8677a51fee7416c28de93a5f31ae6d5`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:5.0.16` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:34ca0ce3077d1e2d1d46e231a442ea68b8f8b695a08f3278c39538fe54ea25c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91443872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dbae1937e6637a793bdc65e2d083cd920472c28c6e242b811a8921b05d6d108`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:41:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:41:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 09:41:01 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 09:41:01 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 09:41:01 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 09:41:01 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 09:41:06 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 09:41:07 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:41:07 GMT
USER emqx
# Thu, 09 Feb 2023 09:41:07 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:41:07 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 09:41:07 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 09:41:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:41:07 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5394f2f4b016df4b79fc515dbf7cd492b3dbe93b959baf39817d26676ae083`  
		Last Modified: Thu, 09 Feb 2023 09:41:48 GMT  
		Size: 3.0 MB (3002749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def267c4d834a0cd84dd88a877e1c746c0a38d9d4b39043b22f599b1a6b9e6b9`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f45e39fe16597c4cd113c4c6390cec4adadb72279e5937cfd5ebf925d3f50d`  
		Last Modified: Thu, 09 Feb 2023 09:41:55 GMT  
		Size: 58.4 MB (58373594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0b8c7e3854a4c45110a7bac48de29bb922a8660f7d4ed1855ce44364cdff81`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `emqx:latest`

```console
$ docker pull emqx@sha256:601c82ac0495ad758003d337c90c4f2cf408c4e85c995e611344b081c09c02c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `emqx:latest` - linux; amd64

```console
$ docker pull emqx@sha256:7d87307488a966746ab49e68e98eb65517db733af54cf209a6d927cb7648d941
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100346619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56505e666d708b81be558f0c7e2ed02b77138943b147fa9eb226ce895ec0151`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:08:45 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:08:46 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 10:08:46 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 10:08:46 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 10:08:46 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 10:08:46 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 10:08:58 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 10:08:58 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 10:08:58 GMT
USER emqx
# Thu, 09 Feb 2023 10:08:59 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 10:08:59 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 10:08:59 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 10:08:59 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:08:59 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc09b4c23409fc6e30f1f0933f0f2c6bd9d7a6566ed0054cb6583015adff6a07`  
		Last Modified: Thu, 09 Feb 2023 10:09:44 GMT  
		Size: 3.0 MB (2987646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5690e645d1f946b924e8d76142ecfdece6e52665554c1a7e613091d6885878`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 4.1 KB (4113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8d953ea948855c1f2fb3f57b7d7c23e9736c453bad99369844efe4dc499ffd`  
		Last Modified: Thu, 09 Feb 2023 10:09:51 GMT  
		Size: 65.9 MB (65942145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5687a1533ec033755e06b7c820a08146f8677a51fee7416c28de93a5f31ae6d5`  
		Last Modified: Thu, 09 Feb 2023 10:09:43 GMT  
		Size: 905.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `emqx:latest` - linux; arm64 variant v8

```console
$ docker pull emqx@sha256:34ca0ce3077d1e2d1d46e231a442ea68b8f8b695a08f3278c39538fe54ea25c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91443872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dbae1937e6637a793bdc65e2d083cd920472c28c6e242b811a8921b05d6d108`
-	Entrypoint: `["\/usr\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/emqx\/bin\/emqx","foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:41:00 GMT
RUN set -eu;     apt-get update;     apt-get install -y --no-install-recommends curl ca-certificates procps;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:41:01 GMT
RUN groupadd -r -g 1000 emqx;     useradd -r -m -u 1000 -g emqx emqx;
# Thu, 09 Feb 2023 09:41:01 GMT
ENV EMQX_VERSION=5.0.16
# Thu, 09 Feb 2023 09:41:01 GMT
ENV AMD64_SHA256=ee95db4baeaa51ff19bb37104013d0a954be64478d02015466a2dfc8d825d19c
# Thu, 09 Feb 2023 09:41:01 GMT
ENV ARM64_SHA256=8bf96461796da3bb0640c0f7456e3bc36b68ddd1ab9c5dae950553645d4859a6
# Thu, 09 Feb 2023 09:41:01 GMT
ENV LC_ALL=C.UTF-8 LANG=C.UTF-8
# Thu, 09 Feb 2023 09:41:06 GMT
RUN set -eu;     arch=$(dpkg --print-architecture);     if [ ${arch} = "amd64" ]; then sha256="$AMD64_SHA256"; fi;     if [ ${arch} = "arm64" ]; then sha256="$ARM64_SHA256"; fi;     ID="$(sed -n '/^ID=/p' /etc/os-release | sed -r 's/ID=(.*)/\1/g' | sed 's/\"//g')";     VERSION_ID="$(sed -n '/^VERSION_ID=/p' /etc/os-release | sed -r 's/VERSION_ID=(.*)/\1/g' | sed 's/\"//g')";     pkg="emqx-${EMQX_VERSION}-${ID}${VERSION_ID}-${arch}.tar.gz";     curl -f -O -L https://www.emqx.com/en/downloads/broker/v${EMQX_VERSION}/${pkg} &&     echo "$sha256 *$pkg" | sha256sum -c &&     mkdir /opt/emqx &&     tar zxf $pkg -C /opt/emqx &&     chgrp -Rf emqx /opt/emqx &&     chmod -Rf g+w /opt/emqx &&     chown -Rf emqx /opt/emqx &&     ln -s /opt/emqx/bin/* /usr/local/bin/ &&     rm -f $pkg
# Thu, 09 Feb 2023 09:41:07 GMT
WORKDIR /opt/emqx
# Thu, 09 Feb 2023 09:41:07 GMT
USER emqx
# Thu, 09 Feb 2023 09:41:07 GMT
VOLUME [/opt/emqx/log /opt/emqx/data]
# Thu, 09 Feb 2023 09:41:07 GMT
EXPOSE 11883 18083 1883 4370 5369 8083 8084 8883
# Thu, 09 Feb 2023 09:41:07 GMT
COPY file:a75ee173244a77553082438ca14f9a3c739eae012d396b2119540782b95f16bb in /usr/bin/ 
# Thu, 09 Feb 2023 09:41:07 GMT
ENTRYPOINT ["/usr/bin/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:41:07 GMT
CMD ["/opt/emqx/bin/emqx" "foreground"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5394f2f4b016df4b79fc515dbf7cd492b3dbe93b959baf39817d26676ae083`  
		Last Modified: Thu, 09 Feb 2023 09:41:48 GMT  
		Size: 3.0 MB (3002749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def267c4d834a0cd84dd88a877e1c746c0a38d9d4b39043b22f599b1a6b9e6b9`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 4.1 KB (4116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f45e39fe16597c4cd113c4c6390cec4adadb72279e5937cfd5ebf925d3f50d`  
		Last Modified: Thu, 09 Feb 2023 09:41:55 GMT  
		Size: 58.4 MB (58373594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0b8c7e3854a4c45110a7bac48de29bb922a8660f7d4ed1855ce44364cdff81`  
		Last Modified: Thu, 09 Feb 2023 09:41:47 GMT  
		Size: 904.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
