## `openjdk:18-ea-jdk`

```console
$ docker pull openjdk@sha256:dcd91a7a7fd14eca70dc8bad4461f6b2b36ee8c48f7fc9c474af69eb3e069953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.469; amd64
	-	windows version 10.0.17763.2452; amd64

### `openjdk:18-ea-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:2177a66e659cec329fb6c080d619be602d2fe611ebc2dd90cd0d52e5e1ba0b83
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244268893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:268c6d351886650a12fd91e52d24abb1dd8be248c79f849d4ed3de9e39bcee6d`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Dec 2021 02:20:57 GMT
ADD file:15b307e0b1aafead42c103e34d3e51a271acea1ab0b68961e239f11af3b0d179 in / 
# Thu, 23 Dec 2021 02:20:57 GMT
CMD ["/bin/bash"]
# Thu, 23 Dec 2021 02:37:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Dec 2021 02:38:28 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 23 Dec 2021 02:38:28 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Dec 2021 02:38:28 GMT
ENV LANG=C.UTF-8
# Wed, 19 Jan 2022 20:40:03 GMT
ENV JAVA_VERSION=18-ea+31
# Wed, 19 Jan 2022 20:40:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/31/GPL/openjdk-18-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='d57d6a205ea5a0b891490b6d9e45315f719ba92123775c4e0e3e76464504f7fa'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/31/GPL/openjdk-18-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='668f2637087591644db894f1f03c5782bb491fd4452b0c736ab7f6e70f1eb036'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 19 Jan 2022 20:40:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:155aced2666332ddff5a741b0236f360820e7aa3fc3dde2224fc17a91fc48db6`  
		Last Modified: Thu, 23 Dec 2021 02:21:56 GMT  
		Size: 42.1 MB (42105152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5901c58ecb29b61159b5e3a63dfbb0fb520b2de1d33c9fb038d9b697e3fcd4`  
		Last Modified: Thu, 23 Dec 2021 02:45:32 GMT  
		Size: 13.5 MB (13520734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af336d5002bb19cc46c68ced8428827aaf14d98731d36578cb1192441b42b33d`  
		Last Modified: Wed, 19 Jan 2022 20:54:27 GMT  
		Size: 188.6 MB (188643007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:236e1cb2ebfa8b84907f34438704576589886bce1f558e503d90742d6808ebdf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243908575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b53ed16274114733c1cbffbc43b6b08ff1b18593b744f18469a723ab0982227`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Dec 2021 02:40:45 GMT
ADD file:140d632303428d802f77f473aef33fa52daacdfc76b23edde4344be661c1d4b0 in / 
# Thu, 23 Dec 2021 02:40:46 GMT
CMD ["/bin/bash"]
# Thu, 23 Dec 2021 02:58:38 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Dec 2021 02:58:39 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 23 Dec 2021 02:58:40 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Dec 2021 02:58:41 GMT
ENV LANG=C.UTF-8
# Wed, 19 Jan 2022 20:54:52 GMT
ENV JAVA_VERSION=18-ea+31
# Wed, 19 Jan 2022 20:55:05 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/31/GPL/openjdk-18-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='d57d6a205ea5a0b891490b6d9e45315f719ba92123775c4e0e3e76464504f7fa'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/31/GPL/openjdk-18-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='668f2637087591644db894f1f03c5782bb491fd4452b0c736ab7f6e70f1eb036'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 19 Jan 2022 20:55:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:53f096d4aa0757c30613f325df1e03a90db9d9879ea251b394e3ab0a068b5610`  
		Last Modified: Thu, 23 Dec 2021 02:41:44 GMT  
		Size: 42.0 MB (42018351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921862a08fd8bc652539d62804daf06ab6464bd5b42061f5bedbdfa73bd62136`  
		Last Modified: Thu, 23 Dec 2021 03:11:46 GMT  
		Size: 14.3 MB (14303905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d9b64a5eed824a919c702bb101eb405f01c287cd9413d19c7984bbd3494cdd`  
		Last Modified: Wed, 19 Jan 2022 21:14:55 GMT  
		Size: 187.6 MB (187586319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk` - windows version 10.0.20348.469; amd64

```console
$ docker pull openjdk@sha256:6231989d45d3b49fd49958304814931339c1ee06d12f958812e8dccb13749830
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2393425065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d809def908e7294a0b4beb71087082972562af39806f6ff78ba56e66da3bad84`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 06 Jan 2022 03:56:33 GMT
RUN Install update ltsc2022-amd64
# Tue, 11 Jan 2022 18:59:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 05:09:49 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Jan 2022 05:21:09 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 12 Jan 2022 05:21:31 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 12 Jan 2022 05:21:32 GMT
ENV JAVA_VERSION=18-ea+30
# Wed, 12 Jan 2022 05:21:33 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_windows-x64_bin.zip
# Wed, 12 Jan 2022 05:21:35 GMT
ENV JAVA_SHA256=57e77e09ea1801bd17d69a31b973074ea5bfeafdc150ca0376b7df8f593629f3
# Wed, 12 Jan 2022 05:22:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 12 Jan 2022 05:22:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b593686e27e7562a5b0696823307ffa822214cee8bd2eec1075eadad4cb9712`  
		Size: 956.0 MB (956001983 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:99e0b71ede60d3b2c5b9053bf27e47c0875590991eede49813d849cc660c7551`  
		Last Modified: Tue, 11 Jan 2022 19:32:06 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42ce1d7b7857ac1eb8d4fbf9579f07cf6a89ed47f3a0979451365d92324f699`  
		Last Modified: Wed, 12 Jan 2022 22:55:59 GMT  
		Size: 644.8 KB (644784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcdfa2da65ea1a1d06b424da27e67263157b1e5a0cb8cf1a5ea3abede1a4007`  
		Last Modified: Wed, 12 Jan 2022 23:02:11 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781d4d837417b9f24bd4783e24e7885836d5bbbccd2a465481dfb85aef6cac6c`  
		Last Modified: Wed, 12 Jan 2022 23:02:12 GMT  
		Size: 551.5 KB (551542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748080050c60eaa9f3140b41c6bd630a27a6b7124a6400786af351d904f8524e`  
		Last Modified: Wed, 12 Jan 2022 23:02:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845352c55222ce1d4da98d5d9aeb4560b39fe26e780810f207c7beae16ecb07c`  
		Last Modified: Wed, 12 Jan 2022 23:02:09 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9938c512137d258605deda56fa17013707713090d27391d3bc66c164ca795c22`  
		Last Modified: Wed, 12 Jan 2022 23:02:08 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1293b9a0c00deefb06ed91cb7ad6c727249dbc78c16f51df2c7580d2819632d`  
		Last Modified: Wed, 12 Jan 2022 23:02:29 GMT  
		Size: 184.5 MB (184519311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d43a192a8ed40a247395cff1cf54d39d29f6e3b244d86952cf5dd894e4235d`  
		Last Modified: Wed, 12 Jan 2022 23:02:09 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk` - windows version 10.0.17763.2452; amd64

```console
$ docker pull openjdk@sha256:13b85a8e5214fba258ffb63543befa3c485a88219fe0ae07bbc7ebbfcf16a9b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2897158462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a13b4ec2f4384760d59d1a5f7b823e7b740d2ada76db8b6b73dd66bd14d3810`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 05:12:35 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Jan 2022 05:22:51 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 12 Jan 2022 05:24:10 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 12 Jan 2022 05:24:11 GMT
ENV JAVA_VERSION=18-ea+30
# Wed, 12 Jan 2022 05:24:12 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/30/GPL/openjdk-18-ea+30_windows-x64_bin.zip
# Wed, 12 Jan 2022 05:24:13 GMT
ENV JAVA_SHA256=57e77e09ea1801bd17d69a31b973074ea5bfeafdc150ca0376b7df8f593629f3
# Wed, 12 Jan 2022 05:25:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 12 Jan 2022 05:25:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3a70d5fd54e2005efbf590b48700ed40509210354a0d8f3f18c3b444a5325896`  
		Last Modified: Wed, 12 Jan 2022 06:20:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74f00c66c11971de2e35204e3f42aca9ac77b3dba4dcd545130bea41c91fd27`  
		Last Modified: Wed, 12 Jan 2022 22:56:55 GMT  
		Size: 346.0 KB (345951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5ef5c6a221a0976ffb06a622ddbeb928e23f646d54ec24e713534a432fd788`  
		Last Modified: Wed, 12 Jan 2022 23:03:02 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1738ecfeffa0ad0e4c36d0a2110a8003421d56cec36f4a31c700953c0bc6bc7`  
		Last Modified: Wed, 12 Jan 2022 23:03:03 GMT  
		Size: 303.1 KB (303067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c62b5744eaef65206df9ca7a42d3d440570ad8131b93cfced7004be36c59db`  
		Last Modified: Wed, 12 Jan 2022 23:02:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ad761c2b0483cac1059235b6181bf1a7d964bf07e9036022ed45e984fc662`  
		Last Modified: Wed, 12 Jan 2022 23:02:59 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa30ea07b77bbedcdbcf9626bdedb35d681aac64bfcbc773a6304c0c899f20a`  
		Last Modified: Wed, 12 Jan 2022 23:03:00 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc41987746763078deae6d29239f68758b8e9aef2094c3f8a1dd12c751f4dd3`  
		Last Modified: Wed, 12 Jan 2022 23:03:24 GMT  
		Size: 184.3 MB (184270030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff25853a3e9481526295980e759afc1c7ee7b40da144fe3ba4fb3edc1bdd41fc`  
		Last Modified: Wed, 12 Jan 2022 23:02:59 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
