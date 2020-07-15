## `openjdk:16-ea-jdk`

```console
$ docker pull openjdk@sha256:8fd8b222205f7ea28489062c32870653da525a525f4cac37f5d550de3fb3a321
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `openjdk:16-ea-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:7169d2452b1832bb800462982002836ac1cfd4c464ab8fd90eeb74d7243602f4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.6 MB (254610198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b735a7317062722d6b8beabad9a74cc4a3cdbd0fc70c861fc3188df60fa4d8dc`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Wed, 10 Jun 2020 18:22:32 GMT
ADD file:79bb5b8b89fe54ba99fd9d42d4f8774bfb9c1319ac3ead17a2005a3bde852451 in / 
# Wed, 10 Jun 2020 18:22:32 GMT
CMD ["/bin/bash"]
# Wed, 10 Jun 2020 18:39:27 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 10 Jun 2020 18:39:28 GMT
ENV LANG=en_US.UTF-8
# Thu, 18 Jun 2020 20:37:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 18 Jun 2020 20:37:39 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jul 2020 04:44:24 GMT
ENV JAVA_VERSION=16-ea+5
# Fri, 10 Jul 2020 04:45:21 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/5/GPL/openjdk-16-ea+5_linux-aarch64_bin.tar.gz; 			downloadSha256=0a29b196a14e038769ff1b506e473dbae610a51c15fe965db7d192413c4c6992; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/5/GPL/openjdk-16-ea+5_linux-x64_bin.tar.gz; 			downloadSha256=78cd9a7c222ca3c23b74734a74011729d0260e60e65186c73806341109402e12; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java --version; 	javac --version
# Fri, 10 Jul 2020 04:45:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fa926a7d213a8145d6a906d68a085b21909a4b26871f142804e68b322bf8881f`  
		Last Modified: Wed, 10 Jun 2020 18:23:43 GMT  
		Size: 43.5 MB (43457466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22aed8993d2fb0bb3a658c631a1dfbd05c0e5d42218f419d18238996bd06ea08`  
		Last Modified: Wed, 10 Jun 2020 18:42:25 GMT  
		Size: 14.8 MB (14760261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c598789de1549dbc2a76aae4da01bc67ba780183799875523f289c144cdb704`  
		Last Modified: Fri, 10 Jul 2020 04:52:13 GMT  
		Size: 196.4 MB (196392471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:eda5f289cbda64204a0df10039d2db457f410a6863bd894ec7e021fdcfd81db9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (234015487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6cdf3aa61b0ea9ba89e9685ecce1b4cbf5b663687d9d6f2ff999c200a2b535d`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 May 2019 21:40:52 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Wed, 10 Jun 2020 18:54:47 GMT
ADD file:64c488ae0df14676929e149538eb50b12e9a99518a126c88ee9704e8a88424e5 in / 
# Wed, 10 Jun 2020 18:54:49 GMT
CMD ["/bin/bash"]
# Wed, 10 Jun 2020 19:12:05 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 10 Jun 2020 19:12:06 GMT
ENV LANG=en_US.UTF-8
# Thu, 18 Jun 2020 23:55:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 18 Jun 2020 23:55:13 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jul 2020 02:31:19 GMT
ENV JAVA_VERSION=16-ea+5
# Fri, 10 Jul 2020 02:32:15 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/5/GPL/openjdk-16-ea+5_linux-aarch64_bin.tar.gz; 			downloadSha256=0a29b196a14e038769ff1b506e473dbae610a51c15fe965db7d192413c4c6992; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/5/GPL/openjdk-16-ea+5_linux-x64_bin.tar.gz; 			downloadSha256=78cd9a7c222ca3c23b74734a74011729d0260e60e65186c73806341109402e12; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java --version; 	javac --version
# Fri, 10 Jul 2020 02:32:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9b791ce794f1b8ac779f7e2bb939c8f822209f7507dbc7f70d072d98b700e55a`  
		Last Modified: Wed, 10 Jun 2020 18:55:52 GMT  
		Size: 44.1 MB (44072411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7857b3d293f1062b1c04189b86491b9bbfd2e793fec6975e1bdcabf4ef9ed3`  
		Last Modified: Wed, 10 Jun 2020 19:14:19 GMT  
		Size: 15.0 MB (15012793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6d0ca741f47b03f289397eb94d166052464c02d0cb48bfb6119ef918f7292b`  
		Last Modified: Fri, 10 Jul 2020 02:37:36 GMT  
		Size: 174.9 MB (174930283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-jdk` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:383989d8e9e29827b971704f8853e943caa02548852be5fe2d2bbe9bbd7ecb9d
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2516279760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb0b11d932c53849d07566ad283b49616f046e13169fb162ca291be23632324`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 01:45:44 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 15 Jul 2020 01:45:45 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 15 Jul 2020 01:46:14 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 01:46:14 GMT
ENV JAVA_VERSION=16-ea+5
# Wed, 15 Jul 2020 01:46:15 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/5/GPL/openjdk-16-ea+5_windows-x64_bin.zip
# Wed, 15 Jul 2020 01:46:16 GMT
ENV JAVA_SHA256=35d6b27ea5cc47f5caad0171e0a6bd120277c572c30c4e0d83d19ef63b74bc4a
# Wed, 15 Jul 2020 01:48:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 01:48:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca5cb7caf11332b67bae426682385af17fa897c718adce9713b111340eb0d71`  
		Last Modified: Wed, 15 Jul 2020 02:42:28 GMT  
		Size: 9.1 MB (9136637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13330fed5347a7e9912941992a3007161aa1fb49b13311deeecee172e5fb8dce`  
		Last Modified: Wed, 15 Jul 2020 02:42:24 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc29d35785aa1c3c0a383049b069e22805c21a9bb9cad32461bcab9457f3e69`  
		Last Modified: Wed, 15 Jul 2020 02:42:24 GMT  
		Size: 293.2 KB (293174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bdf92767da0f8891b56c7a041584266effa05317f3a7b559d3494d1adf210d`  
		Last Modified: Wed, 15 Jul 2020 02:42:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5051a3b20081773b6992bd55eeb550362f9e4747bbdf8584fb114fa6d4f40c3`  
		Last Modified: Wed, 15 Jul 2020 02:42:22 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67aa71c339c714b3ac84e8be1414c7aa91a11d73a42816f9f1c2c7430381bd5`  
		Last Modified: Wed, 15 Jul 2020 02:42:22 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81988434eb0ae3d568d4c03765fc384484d85e0f4c9c950724fa5b436c7c87fc`  
		Last Modified: Wed, 15 Jul 2020 02:42:44 GMT  
		Size: 196.7 MB (196650860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef46a56a2cc955b374fe2a6f49a0283f2dd2cc8041f3170bb38262c6f923bfe`  
		Last Modified: Wed, 15 Jul 2020 02:42:22 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-jdk` - windows version 10.0.14393.3808; amd64

```console
$ docker pull openjdk@sha256:1a59f09807cacbc1781f2b894b2d8d43da938f348c487e0edda359f04ff595c5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5954447110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784dd2fe30d72ad574d70ae4c33090cfe44a1f6f17e04f9bbda56fe5dca81cb8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 01:50:16 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 15 Jul 2020 01:50:18 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 15 Jul 2020 01:51:44 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 01:51:45 GMT
ENV JAVA_VERSION=16-ea+5
# Wed, 15 Jul 2020 01:51:46 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/5/GPL/openjdk-16-ea+5_windows-x64_bin.zip
# Wed, 15 Jul 2020 01:51:47 GMT
ENV JAVA_SHA256=35d6b27ea5cc47f5caad0171e0a6bd120277c572c30c4e0d83d19ef63b74bc4a
# Wed, 15 Jul 2020 01:54:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 01:54:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccabcd61311861039196ce34ec8b8b74f236a3b135a888ca230811c6f8a439bc`  
		Last Modified: Wed, 15 Jul 2020 02:43:13 GMT  
		Size: 9.9 MB (9852381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe0ef8e7d2128d8c84e3f4ee9aa336c9283b3593612b51d5064c853e7b29678`  
		Last Modified: Wed, 15 Jul 2020 02:43:08 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452c9dc43f44e3a09fe36211818cb5063135234cfea03935d12c62801b50888c`  
		Last Modified: Wed, 15 Jul 2020 02:43:10 GMT  
		Size: 5.3 MB (5333218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f08f97065c8c81b23d4d61b0be3d07d9efb88f01334b79d01f244eb141f360`  
		Last Modified: Wed, 15 Jul 2020 02:43:06 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c848d527d8ae5bbc2b0fa70e4a6b2df1aa7a5f4aa96c354631a35849dbfb2912`  
		Last Modified: Wed, 15 Jul 2020 02:43:06 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e6073e9474745744d68001f099891d441c3a8c0cfa27c94e27cf25c0848ead`  
		Last Modified: Wed, 15 Jul 2020 02:43:06 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568a510e3755c6b34f439afcdd4aa36642d3f8fa4b3811343ffa55e39c41ba97`  
		Last Modified: Wed, 15 Jul 2020 02:43:31 GMT  
		Size: 201.8 MB (201792534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e0c4a097b6659c3e1958ca7f57d7643a5b12056d7fee076019e8ec50dd8460`  
		Last Modified: Wed, 15 Jul 2020 02:43:06 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
