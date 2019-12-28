## `mono:slim`

```console
$ docker pull mono@sha256:e137fc49776b95ce1c44047ea9deaa69244ce56f0b833f9fda25e2b4af4ab49d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:slim` - linux; amd64

```console
$ docker pull mono@sha256:3fbc1438cf4ad5f9927ff4c8fd1bde9f827ac55f8065814f00fe4ef8e5b0ba40
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85742837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6194e440ff3046e473b21a8f2e394eb21ce932bec1df73a0dc7b98b2d06990e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:11:17 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:11:31 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:12:14 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d110a8d8d6a5fa5a2ed11b6480fdb8ddd3752cc065f9bb4601207fe6c2a5ccaa`  
		Last Modified: Tue, 10 Dec 2019 22:24:24 GMT  
		Size: 244.5 KB (244460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df5758d8b4d450d2162c07e6a21fcfd0720544194e831610eb80d1780f188bc`  
		Last Modified: Tue, 10 Dec 2019 22:24:39 GMT  
		Size: 63.0 MB (62973805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:263841647b1413f97ede49244a3250c2bd9224534cfda1f58a4cef015523f95e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46863874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24cceab2b02f7699b97ad45390d24175d4f6cbc35951f14304e31bb40284717`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:53:16 GMT
ADD file:7d6af454b55cb354e31c096e935358dd5914688ded04ebc76243a4ff598c4495 in / 
# Sat, 28 Dec 2019 04:53:18 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:28:31 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:28:56 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:29:51 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af28f499fd964f4506ea46c2ac342bc52328a8c30cd633661b69f383a5144e9b`  
		Last Modified: Sat, 28 Dec 2019 05:00:23 GMT  
		Size: 21.2 MB (21202822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f759ae685ca874cea702ae1f63627810d814a2cae6a44c704003176e0c8b37c`  
		Last Modified: Sat, 28 Dec 2019 07:44:23 GMT  
		Size: 244.6 KB (244552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720fbe46ab0c5e8c2e3e9ed44413d9fde2ad1d45d9161dd0c6a021855acc1b78`  
		Last Modified: Sat, 28 Dec 2019 07:44:33 GMT  
		Size: 25.4 MB (25416500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:70f8a6f90eedb2b040cdfe84d228b3b26f0549a32b275183a056543a822ebc44
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44204341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0d6480804e64f949cbbdd9cc9ba45c6e077cd0266e5641b4822ce6ac3e6663`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:37:00 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 07:37:19 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 07:38:02 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ea3a0398ee0834c6b8b5a98490a2451261135d85bbd06845c7077aff2a4667`  
		Last Modified: Sat, 28 Dec 2019 07:50:49 GMT  
		Size: 244.5 KB (244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f543438b2494429fd7ef0a5cbe2145241dfa4aa2f1008038a251526056612dc`  
		Last Modified: Sat, 28 Dec 2019 07:50:58 GMT  
		Size: 24.6 MB (24648229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:c71f8c65cdbb3beccdfee0f7c89b9759cdd7559800c2d53820b2dc232ead5311
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50063944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c674cf5e286615ef8d8b03cbda9840dbfdfd5f9e5f8da1cc02ef19acda0215b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:32:06 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:32:29 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:33:16 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a200380ef45d7e798a6c00bf777add415c1dcd43827dfd4245e9a70a44551c16`  
		Last Modified: Tue, 10 Dec 2019 22:37:08 GMT  
		Size: 244.4 KB (244414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d827d45253e033764c27bafc3cf0f6f6a7c489c4cbfc72204de1e80d360e4ad`  
		Last Modified: Tue, 10 Dec 2019 22:37:19 GMT  
		Size: 29.4 MB (29433771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; 386

```console
$ docker pull mono@sha256:20815f6f85d3625af3bab809cbd0189f28793864ae7eece04b7b0b16287d55f8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.1 MB (90146351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51cf847eb7ced4d53e982f60c5343ba2adc72eb520774f12209b44d8ee8ddeaf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Tue, 10 Dec 2019 22:40:38 GMT
ENV MONO_VERSION=6.6.0.161
# Tue, 10 Dec 2019 22:40:51 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 10 Dec 2019 22:41:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd443cfef677c492dd94fe413c0d2136b767456782251d33c6f1317711c7ebb`  
		Last Modified: Tue, 10 Dec 2019 22:44:33 GMT  
		Size: 244.5 KB (244499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd896b7ec3d7536139b522b4d9ce45dfd161f148c667dbc616035478ae145c7`  
		Last Modified: Tue, 10 Dec 2019 22:44:49 GMT  
		Size: 66.7 MB (66749782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:slim` - linux; ppc64le

```console
$ docker pull mono@sha256:a7840aa6d9953b14f7d37472ed11dc4785cff7c5edbf16718bfc36a6d9cf58b6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48874163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea84dffac95f8be085f5eeb79990afa1341135da9867d71688f2d9a3b61bfbf`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:00:10 GMT
ENV MONO_VERSION=6.6.0.161
# Sat, 28 Dec 2019 06:01:14 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Sat, 28 Dec 2019 06:02:17 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-stretch/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367bf0f7a48952d80f9489622c9b118004dd0fd4763a1fd6153d9b12a571b1ee`  
		Last Modified: Sat, 28 Dec 2019 06:22:04 GMT  
		Size: 244.5 KB (244543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf3902985b2f759ba0edff57a78d4eb7e81f59e8327b7d243b8f3b4b8ca7c79`  
		Last Modified: Sat, 28 Dec 2019 06:22:14 GMT  
		Size: 25.8 MB (25828829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
