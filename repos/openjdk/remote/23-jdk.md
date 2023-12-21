## `openjdk:23-jdk`

```console
$ docker pull openjdk@sha256:f1e1752195f7ba8b3758935f35b0ae79232cfcc35179b7fc887505ee69037538
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 6
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `openjdk:23-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:8a7f3e3844a8ba626b8dccf59523d473b20d74b73efa6f24f7470010f0815995
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.3 MB (269273420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6166d381a157fd324a7624df49ee8a25713b9a617d25dd2a650af235012f336b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Dec 2023 19:53:43 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Fri, 15 Dec 2023 19:53:43 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 19:53:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Fri, 15 Dec 2023 19:53:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-23
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/usr/java/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:53:43 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 19:53:43 GMT
ENV JAVA_VERSION=23-ea+2
# Fri, 15 Dec 2023 19:53:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='c10168b0639ae5a316fb20444202e82fabe5908be7241f1cd42e34ed9d1eca76'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='84b416aba4f3578138dd0d27f570dbaee9123528c4d45d13a338278c3d7136c1'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 15 Dec 2023 19:53:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d986f6e16b814d17738e29faaa870ea909cb21aef547eab206d33b92ad75acd7`  
		Last Modified: Thu, 21 Dec 2023 00:40:48 GMT  
		Size: 15.0 MB (14995426 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09263cab735c482e50f635c1f064f9ad065e933972c8062f592c04766e2dff65`  
		Last Modified: Thu, 21 Dec 2023 00:40:51 GMT  
		Size: 203.0 MB (202954526 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk` - unknown; unknown

```console
$ docker pull openjdk@sha256:18848b24256c23151237e501293d0a35bc85115e0fdf0cbc05fd2c8d83721ad8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1935697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9fa10100444cc58d1de0579d5c1944b39a90a546a851b10601819a75125040`

```dockerfile
```

-	Layers:
	-	`sha256:0dc8980fd21b51deecf08bd367871858eb93cb4d2401450acf5f50e947c6b560`  
		Last Modified: Thu, 21 Dec 2023 00:40:47 GMT  
		Size: 1.9 MB (1915833 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e0f917f7c25e0733d0704015e10e671ca541884e6d4d0ade5be72ef9e9231d6`  
		Last Modified: Thu, 21 Dec 2023 00:40:47 GMT  
		Size: 19.9 KB (19864 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:23-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b42e80447636e70920beec9554225c24d3b0820f421a1ce25ba6ecf388088dcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.6 MB (266620858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f95035d7fedf3933f2eab3b584243db03aae2c77b9c80ef373d1cbeb03104f4a`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 19:53:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Fri, 15 Dec 2023 19:53:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-23
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/usr/java/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:53:43 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 19:53:43 GMT
ENV JAVA_VERSION=23-ea+2
# Fri, 15 Dec 2023 19:53:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='c10168b0639ae5a316fb20444202e82fabe5908be7241f1cd42e34ed9d1eca76'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='84b416aba4f3578138dd0d27f570dbaee9123528c4d45d13a338278c3d7136c1'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 15 Dec 2023 19:53:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61733c769b5e0a95819f0df3a4ff8980287c816c785b828bfb4321091a36b7f5`  
		Last Modified: Fri, 15 Dec 2023 23:19:58 GMT  
		Size: 15.7 MB (15686550 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d72ccedffc6e6f877ccd22b7130dfd06f27fbee00b306cc91f823faff20d32ac`  
		Last Modified: Sat, 16 Dec 2023 09:26:47 GMT  
		Size: 200.9 MB (200861763 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk` - unknown; unknown

```console
$ docker pull openjdk@sha256:f904f1841ac7ad9a2040e096dd4e9e4e71b3f685b4f63e05ab304d5a437f534e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1934128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8ac3121f8685045a56d745d9080b2d61281a3936955b195cd95db0b9699bea`

```dockerfile
```

-	Layers:
	-	`sha256:4474043a7ba0333b72aed93140e7498e24d62ee0c9d7dd6b6b4bb0bafa61808e`  
		Last Modified: Sat, 16 Dec 2023 09:26:42 GMT  
		Size: 1.9 MB (1914393 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c29f44cd24ff101b1336e6763083ec631f5962c610204fad4f4e0fd82de3b812`  
		Last Modified: Sat, 16 Dec 2023 09:26:42 GMT  
		Size: 19.7 KB (19735 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:23-jdk` - windows version 10.0.20348.2159; amd64

```console
$ docker pull openjdk@sha256:cc9172491beac13eb4275403b43a29226baf2e04b0f915bedc05f33b8a7f8dce
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087924389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b275be1da9c7fb81c007cb077f2ed7805f807cabbe24aea7c92426664d7bf71`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Sat, 16 Dec 2023 01:59:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 16 Dec 2023 01:59:52 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Sat, 16 Dec 2023 01:59:53 GMT
ENV JAVA_HOME=C:\openjdk-23
# Sat, 16 Dec 2023 01:59:58 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 16 Dec 2023 01:59:58 GMT
ENV JAVA_VERSION=23-ea+2
# Sat, 16 Dec 2023 01:59:59 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_windows-x64_bin.zip
# Sat, 16 Dec 2023 01:59:59 GMT
ENV JAVA_SHA256=bf19a08c126e820eb3d622dbae9c2928853561d1227235461046491413e7f649
# Sat, 16 Dec 2023 02:00:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 16 Dec 2023 02:00:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a57533c2f32e73f891b22198eae723bac07ef0570921b494b990c11761f93a`  
		Last Modified: Sat, 16 Dec 2023 02:00:23 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accd4967041574377fb4f17559cf90326c4252e8526d540618e92ac5325e9aea`  
		Last Modified: Sat, 16 Dec 2023 02:00:23 GMT  
		Size: 504.2 KB (504162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5270214a52d02d50e92f16dfe70d7026188a8afdba2130cdb579298e188785d4`  
		Last Modified: Sat, 16 Dec 2023 02:00:23 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48618d537d5897dcc778c79e2ccdfa8042f8d63b71c7996975e6419b606d7e6c`  
		Last Modified: Sat, 16 Dec 2023 02:00:23 GMT  
		Size: 356.5 KB (356469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3af01f397493be121d4ed699a047d792fc604e9781296a9b8e24cfabea39d0`  
		Last Modified: Sat, 16 Dec 2023 02:00:21 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220508affe45d964e1688c3a0843914e1a35210910c7b14db8f5217729fa8cee`  
		Last Modified: Sat, 16 Dec 2023 02:00:21 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddcbb29cb6931e7489904834088934dd9bde873eb9dc4f82c748f20c217e276`  
		Last Modified: Sat, 16 Dec 2023 02:00:21 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f6ef7fdf32e8aba8d909df998e343857240c8c3f0b0035fd6fe9408d7fa536`  
		Last Modified: Sat, 16 Dec 2023 02:00:34 GMT  
		Size: 197.8 MB (197782361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20e6f93b138852565325f429cf5b42b601912d46993138e143f00957ce23494`  
		Last Modified: Sat, 16 Dec 2023 02:00:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:23-jdk` - windows version 10.0.17763.5206; amd64

```console
$ docker pull openjdk@sha256:ee58dd7d58ba8d68c0a2a625f6aa17bdfc2497bb4a02a02d436a553e4327872f
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258273118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70df19c343af79b0daecbfaee1b34fe538e5b52f8bc5b35543aa4b52cc41394e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Sat, 16 Dec 2023 01:58:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 16 Dec 2023 01:59:01 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Sat, 16 Dec 2023 01:59:02 GMT
ENV JAVA_HOME=C:\openjdk-23
# Sat, 16 Dec 2023 01:59:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 16 Dec 2023 01:59:23 GMT
ENV JAVA_VERSION=23-ea+2
# Sat, 16 Dec 2023 01:59:23 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_windows-x64_bin.zip
# Sat, 16 Dec 2023 01:59:24 GMT
ENV JAVA_SHA256=bf19a08c126e820eb3d622dbae9c2928853561d1227235461046491413e7f649
# Sat, 16 Dec 2023 02:00:01 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 16 Dec 2023 02:00:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24f607eefb5afd54004adcf2b9132c70ff63c3383cfc4d54c5acab545bc715b`  
		Last Modified: Sat, 16 Dec 2023 02:00:14 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c8c5ed6ea27912c99273f814e33238c11cd84d0f6fcd3fdecf7c888af621bd`  
		Last Modified: Sat, 16 Dec 2023 02:00:14 GMT  
		Size: 458.2 KB (458191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f23a4fb604d2a2ef4a2ae2817f3b07e375f4c3f3b59de27502ce25cb34400c`  
		Last Modified: Sat, 16 Dec 2023 02:00:13 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57272257502e3018181529f6177e29a3544e1298be66e59742a9ef6c54d19977`  
		Last Modified: Sat, 16 Dec 2023 02:00:14 GMT  
		Size: 335.6 KB (335583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79991df59ee5324a4d5d6046074e1b5ee7c0d676764814118dd8f37260a3ef6`  
		Last Modified: Sat, 16 Dec 2023 02:00:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec7f897b38c82c23cb751e35e34d64075640bb5c26cdb79b51890a11e190343`  
		Last Modified: Sat, 16 Dec 2023 02:00:12 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7850104ceaa3a87176c7d49b0b1c2d2daa6ef0256f5ecfbee0a76ae8af42c1fc`  
		Last Modified: Sat, 16 Dec 2023 02:00:11 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3576634d2d7560e1f574456e3ee2aed2c80af5ffbd78d06bf7be7955d0d21ca`  
		Last Modified: Sat, 16 Dec 2023 02:00:23 GMT  
		Size: 197.8 MB (197762533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee54342f02cc37d9b1a074c854d8dfed3227800ad5ad33dde7d7105acaeaf230`  
		Last Modified: Sat, 16 Dec 2023 02:00:11 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
