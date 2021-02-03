## `mono:6-slim`

```console
$ docker pull mono@sha256:28d3578057e16483bef3cb7d9b30c54fa672b8ced049268ad11d96652864336a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mono:6-slim` - linux; amd64

```console
$ docker pull mono@sha256:8769207b9677e6f3f0e95b6423c76cdfd5e450f6b32c051db7b91db5577d7e21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94443211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:348b7e1144c12af5295b3c38dd57ef1b5c6e171ee9409efbbe2bacd0c680eae5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:51 GMT
ADD file:422aca8901ae3d869a815051cea7f1e4c0204fad16884e7cd01da57d142f2e3a in / 
# Tue, 12 Jan 2021 00:32:51 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 09:40:56 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 09:41:03 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 09:41:33 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a076a628af6f7dcabc536bee373c0d9b48d9f0516788e64080c4e841746e6ce6`  
		Last Modified: Tue, 12 Jan 2021 00:39:13 GMT  
		Size: 27.1 MB (27108069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe02677df6f8831edfcea8a4558dcbb344dda0a234033ce403a445f71bb95e04`  
		Last Modified: Tue, 12 Jan 2021 09:56:50 GMT  
		Size: 255.9 KB (255924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f0c1d36d945478bb94f4061ab9e9570a42d064b1bac55d482cc3d9eefdc1b`  
		Last Modified: Tue, 12 Jan 2021 09:57:04 GMT  
		Size: 67.1 MB (67079218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v5

```console
$ docker pull mono@sha256:fbdc9066c014b9853957843c45f789b61596294919443a607a8ccf5749442c7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51607237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d35599162358d092829e97e4858f0a1073436f41099f7a5b983df6c1b4956954`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:51:34 GMT
ADD file:57136a762436a5d41e60c61db0d89baea17a289845ea55565e45cc79a9e81e23 in / 
# Tue, 12 Jan 2021 00:51:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:58:10 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 01:58:32 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 01:59:18 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:2e2535e18472e7491a1d935b1f44ac842e4cc5c4d3de40cecb77b56b44515910`  
		Last Modified: Tue, 12 Jan 2021 01:00:19 GMT  
		Size: 24.9 MB (24851909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781b0df29588b1d712497221b09542f9b882364892a46ecf5521b50115ffe045`  
		Last Modified: Tue, 12 Jan 2021 02:07:54 GMT  
		Size: 255.9 KB (255947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccd7e036e1bf04d2229ab088bc370548d6b63d0540abdfa03ab614ff643669e`  
		Last Modified: Tue, 12 Jan 2021 02:08:01 GMT  
		Size: 26.5 MB (26499381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm variant v7

```console
$ docker pull mono@sha256:5feb406d1ce80dd86fc2db709ca76f30c7120ee7a40a712fd7e32899e4bdffb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48669353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15fcf95ecaebe203ce057c5d16cbfff554c6d24084bef88355b180812987040`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:01:09 GMT
ADD file:1db27e410cc7caf4a97a7313c57260fd01aa134b84306914ef0948dcca27372d in / 
# Tue, 12 Jan 2021 00:01:12 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:53:47 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:54:04 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:54:42 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:be493c6a598447fe5f46a390f3bee10f2d2ba2215d39829fe84eb40a7add18fc`  
		Last Modified: Tue, 12 Jan 2021 00:11:14 GMT  
		Size: 22.7 MB (22715905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c33bdc53ec4d57ecf8d4565fca28d67f043f4855d49b01e900e8ef3c8bb9d6`  
		Last Modified: Tue, 12 Jan 2021 04:03:03 GMT  
		Size: 255.9 KB (255942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9304eb6e55e2cd3920831bd0dec33588ea625b97a60aa2b06301f9351de819`  
		Last Modified: Tue, 12 Jan 2021 04:03:11 GMT  
		Size: 25.7 MB (25697506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; arm64 variant v8

```console
$ docker pull mono@sha256:90a25ba70e6af84267801fd4cbeb308a72f614df951c6c33e9782e140e373538
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57840965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b69b6854e1856fe6d38217029a566ca928db10d685c520adb43f1ecd510f16d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:41:13 GMT
ADD file:0252dccbbfb76766e0e189783d38f6a6afd13f44daa7c5370ffd094adea0f583 in / 
# Tue, 12 Jan 2021 00:41:21 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 05:07:35 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 05:07:52 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 05:08:28 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:f8be76fcf2062bd14a3a78f858da701db8bcd907a2d0f33716d89d9329df2b1f`  
		Last Modified: Tue, 12 Jan 2021 00:51:54 GMT  
		Size: 25.9 MB (25864492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c624bef28ff9228422eef122ec713693eb2e8d2ed78aa41f319bd0678a607c`  
		Last Modified: Tue, 12 Jan 2021 05:15:20 GMT  
		Size: 255.9 KB (255923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec950da6523b4cb54939edc61c6460d64327528adc05f607fbf005ff508a88`  
		Last Modified: Tue, 12 Jan 2021 05:15:34 GMT  
		Size: 31.7 MB (31720550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; 386

```console
$ docker pull mono@sha256:521020ecd687652f6d5c2e2de3a818db2510b049378854f835bfc7caa058746e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99129650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a612a9ed794b39d2f1751626f377d4fe36630334994f4e592e859b2370d5d37`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:39:36 GMT
ADD file:601e9b729a871ae893eafa56eeac5d5d2c93a1bd60786560aae25b3644295a23 in / 
# Tue, 12 Jan 2021 00:39:36 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:55:14 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:55:23 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:56:00 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:a5116b3c01b9daadc6c4605561821b0e7f908a2d339a79315de7651174cd76d7`  
		Last Modified: Tue, 12 Jan 2021 00:46:26 GMT  
		Size: 27.8 MB (27767991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae7e24292b47c5c54d019f27f833b4d1fd06c6c1760426a915f4626d13ebb5`  
		Last Modified: Tue, 12 Jan 2021 04:01:42 GMT  
		Size: 255.9 KB (255867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723f6fae6c251aafe4f2903014f5ca67d695cd2f74f87cc46b0b9b5e50650a9f`  
		Last Modified: Tue, 12 Jan 2021 04:02:03 GMT  
		Size: 71.1 MB (71105792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mono:6-slim` - linux; ppc64le

```console
$ docker pull mono@sha256:fe8b241787171b74a2fd43cd5f13bd303c637bf330e80f289245b9c27b8eb306
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60100071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638800145fd3d9c6b9e6088d6dd2118832963e6457e99a6a04bfd75078bebd50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:25:06 GMT
ADD file:9d7252c169da9a089a0caa2f26cea24678267c15c0e129e7320d4defe0d4637b in / 
# Tue, 12 Jan 2021 00:25:16 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:34:09 GMT
ENV MONO_VERSION=6.12.0.107
# Tue, 12 Jan 2021 03:35:26 GMT
RUN apt-get update   && apt-get install -y --no-install-recommends gnupg dirmngr   && rm -rf /var/lib/apt/lists/*   && export GNUPGHOME="$(mktemp -d)"   && gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF   && gpg --batch --export --armor 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF > /etc/apt/trusted.gpg.d/mono.gpg.asc   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && apt-key list | grep Xamarin   && apt-get purge -y --auto-remove gnupg dirmngr
# Tue, 12 Jan 2021 03:37:38 GMT
RUN echo "deb http://download.mono-project.com/repo/debian stable-buster/snapshots/$MONO_VERSION main" > /etc/apt/sources.list.d/mono-official-stable.list   && apt-get update   && apt-get install -y mono-runtime   && rm -rf /var/lib/apt/lists/* /tmp/*
```

-	Layers:
	-	`sha256:cb701c1e59a3b25dcb09b089f31d61af3065659cd29a7c748f66f3e3c8a96d58`  
		Last Modified: Tue, 12 Jan 2021 00:34:11 GMT  
		Size: 30.5 MB (30532837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77824b16d99ee079aa03b8aabec031637265f7380c082326eaf48d078a93e7`  
		Last Modified: Tue, 12 Jan 2021 04:01:02 GMT  
		Size: 256.1 KB (256146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8e3bf2452dcba3a8621830f987ddbcc051bd5b6d5817e6d595c1cd93497f67`  
		Last Modified: Tue, 12 Jan 2021 04:01:08 GMT  
		Size: 29.3 MB (29311088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
