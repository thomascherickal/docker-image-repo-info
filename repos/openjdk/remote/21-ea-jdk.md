## `openjdk:21-ea-jdk`

```console
$ docker pull openjdk@sha256:db67ae060ba64633550ad36a696baeaf9caf9175271fb7f9e225db6ef35624ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1607; amd64
	-	windows version 10.0.17763.4131; amd64

### `openjdk:21-ea-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:0aed5cb6f9710553f09c0fa293553a227fa6c6414a8f772ec245d658f3ac3ae0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261020740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e80072c1e464ffef2d890e2059d8b31c467369a14a69c11c17c60f9046cdfef`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:15:05 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:15:05 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 23 Mar 2023 00:15:05 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 00:15:05 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 00:15:05 GMT
ENV JAVA_VERSION=21-ea+14
# Thu, 23 Mar 2023 00:15:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='5ff9e95f12627e7f9c4b2e61d4ddfa5eb224f6106eff7620a487244be71d9787'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='32b9ef0cafec4114aac8917e9ad754c7a3bdcfbc47143e4e5182757a0311ae66'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Mar 2023 00:15:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363fdaa54a1583c24462f316031891a2beb8144c7ccd8851f6b6a8869b86ed3b`  
		Last Modified: Thu, 23 Mar 2023 00:15:51 GMT  
		Size: 15.0 MB (15018388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c294c9204234fd36b4cd3499a8fb039514cf71b3e33696bb1b5b4a10cd1b91`  
		Last Modified: Thu, 23 Mar 2023 00:16:04 GMT  
		Size: 201.4 MB (201438976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:2ff8c3b50cbad6486240ea3f5371c9fa62f8f79e6af88669dbe430a8cff20367
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259212996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9677ba1bc7186fb6e5c92f24c86df26d0cc8f4b103b96fba5fbde3f5fec5d36`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:23:23 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:23:24 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 23 Mar 2023 00:23:24 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 00:23:24 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 00:23:24 GMT
ENV JAVA_VERSION=21-ea+14
# Thu, 23 Mar 2023 00:23:36 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='5ff9e95f12627e7f9c4b2e61d4ddfa5eb224f6106eff7620a487244be71d9787'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='32b9ef0cafec4114aac8917e9ad754c7a3bdcfbc47143e4e5182757a0311ae66'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Mar 2023 00:23:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafbc18f0b64482aa39e4830fa399092a7a9f9a39c37c154966aa80bef2ece45`  
		Last Modified: Thu, 23 Mar 2023 00:24:08 GMT  
		Size: 15.8 MB (15834377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37091e4ad405d038b50bdb2a8957e0af6b472f5fa50eac4031fe4c801fcc7e29`  
		Last Modified: Thu, 23 Mar 2023 00:24:18 GMT  
		Size: 199.9 MB (199918582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk` - windows version 10.0.20348.1607; amd64

```console
$ docker pull openjdk@sha256:730dfc484c48c9795bc80b0d7ab9c9ea9289f3abd584bc0347a29d21ccfe9fcb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1911886943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9442fef3b44d0c80df572719fa6e0d787df120caa3824da00df8b66e623a8079`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:14:25 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Mar 2023 04:14:26 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 16 Mar 2023 04:14:53 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Tue, 21 Mar 2023 00:15:25 GMT
ENV JAVA_VERSION=21-ea+14
# Tue, 21 Mar 2023 00:15:26 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_windows-x64_bin.zip
# Tue, 21 Mar 2023 00:15:27 GMT
ENV JAVA_SHA256=8dba94712d3e80ae3ecc982cb1c4e5b3986c6cd7e71de80239ef7bed943dd8e1
# Tue, 21 Mar 2023 00:16:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 21 Mar 2023 00:16:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9232261c30bc22ec57212f386e8fea077a0775299f58234bfec01a611d98144`  
		Last Modified: Thu, 16 Mar 2023 04:30:43 GMT  
		Size: 736.0 KB (736009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545d4a9e39b1cc7dac0d42fb0a331c120f1bfed624e7850e1faa4eb99110ce01`  
		Last Modified: Thu, 16 Mar 2023 04:30:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8063d1ae112267a681a9e7feb4d398e107825072b3fd2b95b3bad2efc8571978`  
		Last Modified: Thu, 16 Mar 2023 04:30:43 GMT  
		Size: 538.0 KB (538004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e594ac73d3ea757d7e949feeb3e28689bccb55bb5f29d79a569334355e06a9b9`  
		Last Modified: Tue, 21 Mar 2023 00:21:59 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2828617510eb4cf81b057485931c58e5a9e26d8f78bc29374240158b827051`  
		Last Modified: Tue, 21 Mar 2023 00:21:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583c15c53b5ca52fea33ba3de528941d616b833db04c98af59db2f0671017b1d`  
		Last Modified: Tue, 21 Mar 2023 00:21:59 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6c5140f0904bafd3500511d25b7bf156c8372fe73e01b54413b3fae1745d5f`  
		Last Modified: Tue, 21 Mar 2023 00:22:21 GMT  
		Size: 196.7 MB (196664361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f68d451ad865a0a2edad7aabcd049b8920ff44515c5190a7da29fb5c059191`  
		Last Modified: Tue, 21 Mar 2023 00:21:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk` - windows version 10.0.17763.4131; amd64

```console
$ docker pull openjdk@sha256:4d32d752ac48655976f5d55f79411343f9ca339ee775b9b4d20706d83bcc4d40
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2210750880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:567027b545ea99e84e0288ae83d08858c875512ecfdb25ed816f6eb5c6047f09`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:17:49 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Mar 2023 04:17:50 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 16 Mar 2023 04:19:13 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Tue, 21 Mar 2023 00:17:09 GMT
ENV JAVA_VERSION=21-ea+14
# Tue, 21 Mar 2023 00:17:10 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_windows-x64_bin.zip
# Tue, 21 Mar 2023 00:17:11 GMT
ENV JAVA_SHA256=8dba94712d3e80ae3ecc982cb1c4e5b3986c6cd7e71de80239ef7bed943dd8e1
# Tue, 21 Mar 2023 00:19:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 21 Mar 2023 00:19:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6954ad7da48d4dd7acf8132bc41996dfcd7f157b30b2ca35ec4814ffc26a94d3`  
		Last Modified: Thu, 16 Mar 2023 04:31:25 GMT  
		Size: 480.4 KB (480436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8087e24b23846aed99e303ff6d5268f444daecd74c150fb70198dabc16487141`  
		Last Modified: Thu, 16 Mar 2023 04:31:25 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2836db1b10d5ae1b6c026b5fc8f9667c86fafa8854926472e99f786aea1aaf7f`  
		Last Modified: Thu, 16 Mar 2023 04:31:25 GMT  
		Size: 309.7 KB (309740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e175ffecbfaaee4a89edb750a18bf749cf139289dde93780c68d0346409bd470`  
		Last Modified: Tue, 21 Mar 2023 00:22:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9817775d563cdf68565928daec973982b3b5585dec8890bc9652f5358349d28a`  
		Last Modified: Tue, 21 Mar 2023 00:22:41 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3106a077503c01f522faaaf452a970f713ad9ac9d2c79e502761bc2a5afc6e`  
		Last Modified: Tue, 21 Mar 2023 00:22:41 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a56e89a21746771a8a18de93bb29344057f3d8f62e4ae41d43114f46a726ee8`  
		Last Modified: Tue, 21 Mar 2023 00:23:02 GMT  
		Size: 196.4 MB (196443248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b06f4944e696fd8230c488da00d86c77a5dba39d760d3ea64705a6d8494497`  
		Last Modified: Tue, 21 Mar 2023 00:22:41 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
