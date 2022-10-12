## `openjdk:latest`

```console
$ docker pull openjdk@sha256:be9f94b9cc3ea5a74eb99bcd155ea99bd7d2a20e4ed1e5504fff022fc01b1be0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1129; amd64
	-	windows version 10.0.17763.3532; amd64

### `openjdk:latest` - linux; amd64

```console
$ docker pull openjdk@sha256:d737e7b122d6868e882fca9c7c61266f092af32285dc5bcd8f0d2257e36da569
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.6 MB (241566445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7acac241890b1fffe5eae13f756b1ebdf28294891eae13c029f5aaacbfebdc79`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:40 GMT
ADD file:40e1b0533d9ae91c868834395cbd4b74cf2a47965791be201c03ae764f9da2b0 in / 
# Fri, 07 Oct 2022 20:31:41 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 20:50:12 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 07 Oct 2022 20:51:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 07 Oct 2022 20:51:21 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 20:51:21 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 20:51:21 GMT
ENV JAVA_VERSION=18.0.2.1
# Fri, 07 Oct 2022 20:51:31 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 07 Oct 2022 20:51:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:295ca23427284cb123fd4c132a1ecb521e7f787ac75dadec342f744a343efec4`  
		Last Modified: Fri, 07 Oct 2022 20:33:22 GMT  
		Size: 40.6 MB (40589568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f95ca5341d49c7c99a979d862484e30b44156db525868b136dd3cf8c0535aa`  
		Last Modified: Fri, 07 Oct 2022 20:54:09 GMT  
		Size: 12.2 MB (12231949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97eecaf86326cdd1b6497dd4685d711a1ca757e5a68fa707f4bb47d12d18d75a`  
		Last Modified: Fri, 07 Oct 2022 20:55:57 GMT  
		Size: 188.7 MB (188744928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:latest` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d776c289aaeec3831d290de9e896f045a7a6253f1f3a8541063e30c0891294e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.1 MB (240123021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adcc07146b4fd7a78436e918da5bf204677a2d285b1b403bf76227186c187d2`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 07 Oct 2022 20:51:45 GMT
ADD file:6eb7b065ffe8855d82638de19bd23fba329883c96f01d093e7bc6bdb5da836a3 in / 
# Fri, 07 Oct 2022 20:51:46 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:13:40 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:15:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 07 Oct 2022 21:15:38 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 21:15:39 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 21:15:40 GMT
ENV JAVA_VERSION=18.0.2.1
# Fri, 07 Oct 2022 21:15:54 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 07 Oct 2022 21:15:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5d45c82139e084eb338a0a2346c4ec4c6d2bfa4acda9194cf6602728b4a3e89f`  
		Last Modified: Fri, 07 Oct 2022 20:53:34 GMT  
		Size: 39.4 MB (39409020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e39aebf905a4bfcc927f63602bf79927ed6767d85862e1311b9e8f0e5924ad`  
		Last Modified: Fri, 07 Oct 2022 21:21:10 GMT  
		Size: 13.1 MB (13054492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099885326771e976fe3f2dd54a4c9f1dc091573577751165c77c8efecb8ba030`  
		Last Modified: Fri, 07 Oct 2022 21:23:35 GMT  
		Size: 187.7 MB (187659509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:latest` - windows version 10.0.20348.1129; amd64

```console
$ docker pull openjdk@sha256:2a4e07ecda09337b08966ec9d795000b7a7d2e214d5837c016ba5ce0f4bdc4b0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2602246293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4db33cde07cf05d8397a715d298d06db2bf599569e836170bdda399b1cf5e5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:39:02 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:44:42 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 12 Oct 2022 16:45:00 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:45:01 GMT
ENV JAVA_VERSION=18.0.2.1
# Wed, 12 Oct 2022 16:45:01 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_windows-x64_bin.zip
# Wed, 12 Oct 2022 16:45:02 GMT
ENV JAVA_SHA256=fc08052175eb2f66cedfcca368ab5d51c55f50d6f440b124e4512499825cb7b1
# Wed, 12 Oct 2022 16:45:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:45:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cbc434576dbff410ee0aa4228c6f0fa038ee64fba58d8b81df98ab5bd3e8e5`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 609.6 KB (609572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6b3de9da78eaf2a9366fa332117984b73bceff8a4d196ba8705a5787587a47`  
		Last Modified: Wed, 12 Oct 2022 16:53:50 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8754ca31e7da9de26690dfcdc8c6af7befe2502513de66e78710cc746c8c7431`  
		Last Modified: Wed, 12 Oct 2022 16:53:50 GMT  
		Size: 525.5 KB (525484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dc86abb9b233e0561750bb5413dd1ecf28e902631ce52d58f44e20cedfe5eb`  
		Last Modified: Wed, 12 Oct 2022 16:53:47 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce6181375e5e3f0d5a3752c7e680f571b0d36f8c6236c3583e105f5e5310759`  
		Last Modified: Wed, 12 Oct 2022 16:53:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640d999f8d67d9977263ea8b2a6b21fcdc5b8db2b37017dc662b87a9ed9258f9`  
		Last Modified: Wed, 12 Oct 2022 16:53:48 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362570e7828376e56c477c0f82658dbac129375038b33a2a39f34e9aba881e3c`  
		Last Modified: Wed, 12 Oct 2022 16:54:04 GMT  
		Size: 184.9 MB (184879391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379f9b5f4b5c9784a28c213a51a9360fddab56a3ce39fc2f3fcceee193d09ae9`  
		Last Modified: Wed, 12 Oct 2022 16:53:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:latest` - windows version 10.0.17763.3532; amd64

```console
$ docker pull openjdk@sha256:209f5c23c1fcb87e8db89be500d8bcf2528639e31c094bcd870122eecea37c6e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2896507872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b00c006f23e4d5f4b01ee4faac9e0a1ca609d0b727c8dc4825b2b789dbe7a3c3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:41:21 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:46:09 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 12 Oct 2022 16:47:14 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:47:15 GMT
ENV JAVA_VERSION=18.0.2.1
# Wed, 12 Oct 2022 16:47:16 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_windows-x64_bin.zip
# Wed, 12 Oct 2022 16:47:18 GMT
ENV JAVA_SHA256=fc08052175eb2f66cedfcca368ab5d51c55f50d6f440b124e4512499825cb7b1
# Wed, 12 Oct 2022 16:49:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:49:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891dd6ec2fa598da717e21a05ad77857caf95e46fc5861ed7e79aab507e9fd11`  
		Last Modified: Wed, 12 Oct 2022 16:52:29 GMT  
		Size: 347.9 KB (347943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a84034b46d932e57ff044c1977d2bf8c336c29bfa39ebe1f0f4c948f379ae7`  
		Last Modified: Wed, 12 Oct 2022 16:54:38 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f00c79774c9b6154f2d4c74e191db1673be872b2a3be692af0a5eaff8f12760`  
		Last Modified: Wed, 12 Oct 2022 16:54:38 GMT  
		Size: 310.5 KB (310480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2df68caf6b0249eda4b4c804f7014f93b9c7b0774756b5f775aa874defb3ef`  
		Last Modified: Wed, 12 Oct 2022 16:54:36 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f668febd3f85588118ed2d57c5f3c0ded26401299d5773c9ae875d8251f590`  
		Last Modified: Wed, 12 Oct 2022 16:54:36 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7fda581d6cc276f7da21ebbda1b56ad16721d978f99dc9fb0ecb321d40ff3d`  
		Last Modified: Wed, 12 Oct 2022 16:54:36 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34d6b14bcf4432c184f9ffe60c2df26126583d3e6cea41ff049958a678bc83f`  
		Last Modified: Wed, 12 Oct 2022 16:54:55 GMT  
		Size: 184.7 MB (184677027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ab05a5e4fec6cb7c3b9a0a886dc235dd77ff17d98ad08215ac2bc61a1b37ba`  
		Last Modified: Wed, 12 Oct 2022 16:54:36 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
