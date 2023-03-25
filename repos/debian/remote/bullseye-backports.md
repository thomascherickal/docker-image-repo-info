## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:4dfa866b116f63cc865b2fa4d0905e4d812929af08680c77d4c2cf4de4fe35cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:c617037db0604e4bb27a3c2460738a22cef87ac023933d8f3278b9326bcc750a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55045834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791bc0a8e3c24bd14a971fdc8cf6f5d1b6ab04f0db6b6d446326269b4967d97d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:30:18 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27aa661c306ebe830169d2ff7c65c5b82d14523dc4a114a5df1b1a6279c39fa9`  
		Last Modified: Thu, 23 Mar 2023 01:34:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:5e2fc48e4bc30f6107c72618457618da37c6dd5ca98ef19fb2254a93ab9c8e98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52549780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2f49c82de2b1caa290083ec6019e958d398a23760aba723efcebd8c01b29281`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:37 GMT
ADD file:8419f4bee11379b8aa511da1fe7cdcd6b2cb8c252bc90f76dec672a5b802ea27 in / 
# Thu, 23 Mar 2023 00:48:37 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:48:39 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9a8ea6c28ff9e1b5a437e1e5b168873207139672ec8d755939cad00b23349e22`  
		Last Modified: Thu, 23 Mar 2023 02:21:35 GMT  
		Size: 52.5 MB (52549555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69816ee3daa48201de0a8386cf1501eddf766583836a74d035bd2969bb679ba`  
		Last Modified: Thu, 23 Mar 2023 02:21:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:81f8ffbb7b0cdad7393ba9034a4bcf0afe362c95fd9e59827e452059096cfda2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50212012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d855c1bf72d5407c55ac50abbbdb5be4f3a68e2c5156a771b82ae995fa84ed3b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 22:30:10 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a3f412c70268c2c555a6d2e8699c260c77d3e9aa9ed8332b44121e627f5964`  
		Last Modified: Fri, 24 Mar 2023 23:28:31 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:c8660693dab64baea85b7f953e93c0480f16100ff1ddd7bf40dac2eb3b60b1d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53703325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9177fc6915502ac07e2d3e9950cb3024bae81549d9a4ddd17fb42b1eb09fcac6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:45:05 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4321f724ec4103a60b8da16d123240593e023dd1ca36e9790676e6575ad7ea`  
		Last Modified: Thu, 23 Mar 2023 00:48:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:9b61749c8b1ee17a4ee71e23e0b31539f16653343af9a2756bcf86b45690d559
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56028136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab32b4bdda8b36bc50d177f322c9fd3ce2a5f84fad78c04322bbc3ffda489c6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:08 GMT
ADD file:f331251c4c21fceff56d13f76442a6334dc355c29ec7450768c1c86a3db1adab in / 
# Thu, 23 Mar 2023 00:39:09 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:39:11 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c1bb878cff31d37952c5c73ed15c167f599bb7f97b3eeaa1a17352b2473b3394`  
		Last Modified: Thu, 23 Mar 2023 00:42:44 GMT  
		Size: 56.0 MB (56027911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad54a68987940f3f6609b73654acb8468ef9df8b07dbbd85d0100cfe346cf541`  
		Last Modified: Thu, 23 Mar 2023 00:42:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:2f87205e795a268513c1dc1f5487529c930ba030f985335109e34ce78b16db29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53264946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:196afe73fd70e3f9fff74553731261e9d69067de1a51695135308b6c1107a52b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 05:17:36 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4d51d8cd24e32a9331fc46320d0c1730eddd4b9931ec847c0df151c1dd92c9`  
		Last Modified: Thu, 23 Mar 2023 05:25:27 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:6d015466ceb0799b2bb14760783d808c98f5ecddebaa95e20d408ae759016860
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58921252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c02aabbc9ab2cd0465456427d1f10978744f08f9a6d0760a73a7174b5926070c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 01:19:33 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064e253a5420b378dea517838ecc1b7cc8ddd83bf06f54587cce6c3f8ffad439`  
		Last Modified: Thu, 23 Mar 2023 01:24:07 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:7cf3dc57904e3fa0b24d08b0eb40fa2152455047e05a0bb1396e2aebd21e2cf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53277724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb5241975235e7e2510d9d313561de376291e77431ff7b0cdc738c419c18759`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Mar 2023 00:43:50 GMT
ADD file:1111f9325245c8edccf2d9480c39cf2368f783ad86c2700d452be4e8cbebef8a in / 
# Thu, 23 Mar 2023 00:43:54 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 00:43:58 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:00dac46cbc44f444bd1dffe5b00a1b239054295b96f7984793273e9d12e75591`  
		Last Modified: Thu, 23 Mar 2023 00:47:04 GMT  
		Size: 53.3 MB (53277499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9886548eea58359865cffbc1b4ae32b94bf69c94ef046624bc9eb749b10d97a8`  
		Last Modified: Thu, 23 Mar 2023 00:47:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
