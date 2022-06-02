## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:31887bb4e30f516dcdae6ee406b07a6ef306f1ec3a0bf0b0e780c77f20e662ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `golang:1-nanoserver` - windows version 10.0.20348.707; amd64

```console
$ docker pull golang@sha256:b684c168e34d7ce145c037c33df22a37473b3881aefa4a175124554fc04f16ca
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.1 MB (267074095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:207f51284cb81cb18eea22f1da4c8a087bc792d6544c82395c66174a95357104`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 05 May 2022 02:37:33 GMT
RUN Apply image 10.0.20348.707
# Tue, 10 May 2022 22:28:05 GMT
SHELL [cmd /S /C]
# Tue, 10 May 2022 22:28:06 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:28:07 GMT
USER ContainerAdministrator
# Tue, 10 May 2022 22:28:55 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Tue, 10 May 2022 22:28:56 GMT
USER ContainerUser
# Wed, 01 Jun 2022 23:23:35 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:26:07 GMT
COPY dir:f2d0f4a9267a591c33858aceb464994502f206b1bde0c83972e6f9e2e21fe641 in C:\Program Files\Go 
# Wed, 01 Jun 2022 23:27:02 GMT
RUN go version
# Wed, 01 Jun 2022 23:27:03 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:2c74f0842c5a8e9b80b9e2cf64e1ab10a6fa67951f28cff5fee060b88128564c`  
		Size: 117.7 MB (117687017 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:617bb7e935bb4ca0ff934490b4a9f19a0bdedc2df4476ebd2784b3e63f7ec0eb`  
		Last Modified: Tue, 10 May 2022 22:56:44 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d185904f43d3a2981edaed48af0694ad47290902c2db8fc338def1f6d21a700`  
		Last Modified: Tue, 10 May 2022 22:56:44 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bd0b6a3dc76d11dbe60ada4f477170f4156f5e8d0a1e13555d3b4c266f9258`  
		Last Modified: Tue, 10 May 2022 22:56:44 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a892e1a707cb554fd1d08cd68714e3e78217f10d1c9d93a6120ea840590f89ff`  
		Last Modified: Tue, 10 May 2022 22:56:44 GMT  
		Size: 98.4 KB (98390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0fb4392e920dc3d82438940caa8c09546cce8a9d054013225a0c792a6d5bb`  
		Last Modified: Tue, 10 May 2022 22:56:41 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c5e95eaf94ab482d5a138134240d245396ce4e13fc520952eb8035b1262dd3`  
		Last Modified: Wed, 01 Jun 2022 23:47:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa81377334b1eb4d021b3445b6a94d0c990f1bd82911bcf3f0dc363abb36593`  
		Last Modified: Wed, 01 Jun 2022 23:50:22 GMT  
		Size: 149.2 MB (149220429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24b4397bc000ea93a4a3363e7215d508cc74eb6de25f3650716578b3c66fa0a`  
		Last Modified: Wed, 01 Jun 2022 23:47:39 GMT  
		Size: 61.2 KB (61158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab35b2881ddb50a3e6e945752ff0374395101e643eac16295cf27470c0b8728`  
		Last Modified: Wed, 01 Jun 2022 23:47:38 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull golang@sha256:f64249ad11676adb90219c218fbb2275dce4639d8ef30a045ada17e969270edc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.5 MB (252482207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:586ec6ebaccb5e4bc013cb181fd68fbf6889baadef6864d0165928ea11ce1457`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Tue, 10 May 2022 22:32:24 GMT
SHELL [cmd /S /C]
# Tue, 10 May 2022 22:32:24 GMT
ENV GOPATH=C:\go
# Tue, 10 May 2022 22:32:25 GMT
USER ContainerAdministrator
# Tue, 10 May 2022 22:32:50 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Tue, 10 May 2022 22:32:51 GMT
USER ContainerUser
# Wed, 01 Jun 2022 23:27:19 GMT
ENV GOLANG_VERSION=1.18.3
# Wed, 01 Jun 2022 23:29:51 GMT
COPY dir:f2d0f4a9267a591c33858aceb464994502f206b1bde0c83972e6f9e2e21fe641 in C:\Program Files\Go 
# Wed, 01 Jun 2022 23:30:35 GMT
RUN go version
# Wed, 01 Jun 2022 23:30:36 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d7d4dec608f59eb9166ff96f59e4f4fcbda08a55e78d630ba39e558b23b3e475`  
		Last Modified: Tue, 10 May 2022 22:59:35 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4735e17fcd180a1d905a22c771ac994a1a249e57bfdde77ef41ccf51a0e29a3`  
		Last Modified: Tue, 10 May 2022 22:59:35 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833e97847abafba5e024c2c960a8b406785b7f11a1a3dd574f40993a068c19e4`  
		Last Modified: Tue, 10 May 2022 22:59:35 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd374e2694dcb43adcc3181c4f72a6fd7b1432b49478e67616949e2efe9aafd`  
		Last Modified: Tue, 10 May 2022 22:59:35 GMT  
		Size: 68.8 KB (68805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d279dc1f42008981f8d43d3f502139a3b21c0f5ca5d86ac0b9862c424b4477e`  
		Last Modified: Tue, 10 May 2022 22:59:33 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544088d8ac402da890dab3a50f88ce8b0a328aa42759853cf624e81a5b5646e2`  
		Last Modified: Wed, 01 Jun 2022 23:50:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37f6550d5326b4b8a6a4a872523bcde4352329a121d68322d9223e78872eab9`  
		Last Modified: Wed, 01 Jun 2022 23:53:20 GMT  
		Size: 149.2 MB (149200327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c95efe5638c689acdc995c4001a617628f0f5e3879b5bc6c0146e8595afa3c`  
		Last Modified: Wed, 01 Jun 2022 23:50:37 GMT  
		Size: 72.1 KB (72067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f64c487fbd419b6c977df6cbbc92087927217a8803e8535130b1745df3f0d1`  
		Last Modified: Wed, 01 Jun 2022 23:50:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
