## `openjdk:latest`

```console
$ docker pull openjdk@sha256:10de8787bed66b22d8700d2f5f7c9affd9726176b433296cadedba1e0c948405
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `openjdk:latest` - linux; amd64

```console
$ docker pull openjdk@sha256:7928e7eb217232e0ed0a248746a8ebcaba4ca7fdc0f3105789ff2584aa67322a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.6 MB (242597178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744cf265878b854fbae9a17dddb120eac0f5d0edde8606ff3855a3fb348595cf`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 13 Oct 2021 18:29:51 GMT
ADD file:3223e5829b65b376c23e1faa6f519d37b0166b38063f91b793a8ed710a39fe33 in / 
# Wed, 13 Oct 2021 18:29:51 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 18:47:48 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 13 Oct 2021 18:49:05 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 13 Oct 2021 18:49:05 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 18:49:05 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 18:49:06 GMT
ENV JAVA_VERSION=17
# Wed, 13 Oct 2021 18:49:17 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 13 Oct 2021 18:49:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:58c4eaffce77ac1fb013bf82c91927c631802ad54465ebc9b687b5dc8ee73c02`  
		Last Modified: Wed, 13 Oct 2021 18:31:20 GMT  
		Size: 42.0 MB (41961111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a22c806ee8aa2b360bd5818a4f78bc3da280abb86f3db09805b1daddd78324`  
		Last Modified: Wed, 13 Oct 2021 18:56:49 GMT  
		Size: 13.5 MB (13489427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a88e5590ad1b849be4e189b4ba765d5c709a6f42b53dfaaebbe4449ef517d35`  
		Last Modified: Wed, 13 Oct 2021 18:58:43 GMT  
		Size: 187.1 MB (187146640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:latest` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9dd57f3b4c120603c7462281be8ced6403b0693aea165768b3577f8eadc65ea2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.1 MB (242106295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29cbaf3d347f2cee42ae47e0abf9da35cd90ba38a492b7b11ee6dca131180ebc`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Sep 2021 09:28:21 GMT
ADD file:19a29c4f8accf14e581617044399a0a04fbdf31b2a3dd531b59c72d011deea65 in / 
# Wed, 29 Sep 2021 09:28:21 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 05:58:48 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 13 Oct 2021 06:02:23 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 13 Oct 2021 06:02:24 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:02:25 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 06:02:26 GMT
ENV JAVA_VERSION=17
# Wed, 13 Oct 2021 06:02:42 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-x64_bin.tar.gz'; 			downloadSha256='aef49cc7aa606de2044302e757fa94c8e144818e93487081c4fd319ca858134b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_linux-aarch64_bin.tar.gz'; 			downloadSha256='b8108a6b6c2579bd585281937cf09d401a5a971c59b9624e18abcf596b9caa22'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 13 Oct 2021 06:02:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fbe1b66208e55e97b0e90b882e6fdeed78abb9318897a2d87343840b78e723ef`  
		Last Modified: Wed, 29 Sep 2021 09:29:46 GMT  
		Size: 41.9 MB (41883345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076e889c44db9131098a7368fb924c97ba81cb10aee46f9c273b2076baab08f5`  
		Last Modified: Wed, 13 Oct 2021 06:23:16 GMT  
		Size: 14.3 MB (14270423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c050a6f9ac24ea50977cfba1f7edf04636795bd49aeade27fcf241d7ac14fdac`  
		Last Modified: Wed, 13 Oct 2021 06:28:06 GMT  
		Size: 186.0 MB (185952527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:latest` - windows version 10.0.17763.2183; amd64

```console
$ docker pull openjdk@sha256:90c830daa657bc3eb55a8b4fec9f682206cb7e798a565f66ae62c640b699bfc5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2869804672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4552a811b57fc5c25ef2721b80f0470eb951562d48413cc44202a74b9a882a5e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 00:31:34 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 15 Sep 2021 00:39:14 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 15 Sep 2021 00:40:03 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 15 Sep 2021 00:40:04 GMT
ENV JAVA_VERSION=17
# Wed, 15 Sep 2021 00:40:04 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_windows-x64_bin.zip
# Wed, 15 Sep 2021 00:40:05 GMT
ENV JAVA_SHA256=e88b0df00021c9d266bb435c9a95fdc67d1948cce4518daf85c234907bd393c5
# Wed, 15 Sep 2021 00:41:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Sep 2021 00:41:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d714779fd458636d1b2289ae98777c0c8707a28708bffccab0b1314b59d77c`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 356.1 KB (356133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb8edc5219b9dc30560f6beba3551f189a29cee0da7e1addc07adc947a05653`  
		Last Modified: Wed, 15 Sep 2021 01:14:27 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4899e7ca7fa7a47de0bc8dec992cc3e10d1ecdbeadbfd643a80737a8df09c178`  
		Last Modified: Wed, 15 Sep 2021 01:14:27 GMT  
		Size: 315.5 KB (315467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac695f0ea6843cc67b0ae97e75703b4bba561d0b6d31da9c46d2be7f966ad6c5`  
		Last Modified: Wed, 15 Sep 2021 01:14:25 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b2c66025026cb674eddd9dba8aa820db1401ffd8dab3065b426e4c92731406`  
		Last Modified: Wed, 15 Sep 2021 01:14:25 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4e41e57d815a6e08537c6c34f81b101ad45c70880dd592bba4a7b31666efa0`  
		Last Modified: Wed, 15 Sep 2021 01:14:25 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75877a72b7bf20f952dfdd355ae222415cd299b67173aa0d708cdba353ff6a97`  
		Last Modified: Wed, 15 Sep 2021 01:14:41 GMT  
		Size: 182.4 MB (182427194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cee5586b0a3b62cef9698a5657f0f7a2c177c9d053b5ab6ec31ab78267f3fdf`  
		Last Modified: Wed, 15 Sep 2021 01:14:25 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:latest` - windows version 10.0.14393.4651; amd64

```console
$ docker pull openjdk@sha256:60b1660d9acaede1693f48b5c80920f021679ab4927c098c36b34b663ac784ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6454423203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab98f1cade5b484f2471f879397990d7885bc01c2ed0f6f742299a882e8cace`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 00:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 00:35:51 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 15 Sep 2021 00:41:25 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 15 Sep 2021 00:42:18 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 15 Sep 2021 00:42:19 GMT
ENV JAVA_VERSION=17
# Wed, 15 Sep 2021 00:42:20 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_windows-x64_bin.zip
# Wed, 15 Sep 2021 00:42:21 GMT
ENV JAVA_SHA256=e88b0df00021c9d266bb435c9a95fdc67d1948cce4518daf85c234907bd393c5
# Wed, 15 Sep 2021 00:43:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Sep 2021 00:43:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8721f004192f15fe71b8626ef3f3e34cbf2cfe1d15a63b6b544ab946162ef707`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b794d0a07a41196dae8678e4ecbb9a5766d6db31f9729bfe3f1d83963af3e0`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 339.2 KB (339172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96d7d774769f6a1e49099ad3d81f4f5beac1f7aa9603957c90af07798c7a10c`  
		Last Modified: Wed, 15 Sep 2021 01:15:00 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0c0dc76a862d394d0fdaa158d75d7f21857b64669444a47327b160126051d9`  
		Last Modified: Wed, 15 Sep 2021 01:15:00 GMT  
		Size: 328.2 KB (328214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a33a97494fe71397e66f4ab8c33f4010545e97df2d1a3dc90dc0784ba5d481`  
		Last Modified: Wed, 15 Sep 2021 01:14:57 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b94b5bea64b0f3fffc79fd41ec9498569eea626d0565ded17dd51675d66fe0`  
		Last Modified: Wed, 15 Sep 2021 01:14:57 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d249d0550e435c9dc61c730d5a932d6b55f872842ccb2258f65e49e9db8d942`  
		Last Modified: Wed, 15 Sep 2021 01:14:57 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca822a83ed50e2f1bd84bba5684d22f208893b91b7f436bcce80017f092ede1`  
		Last Modified: Wed, 15 Sep 2021 01:18:16 GMT  
		Size: 182.4 MB (182419810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e4d4e15b17d8e4fbec840c1a3a64de9238139ac8d6a11472c65e2bfbcbdadd`  
		Last Modified: Wed, 15 Sep 2021 01:14:57 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
