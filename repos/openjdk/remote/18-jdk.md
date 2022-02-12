## `openjdk:18-jdk`

```console
$ docker pull openjdk@sha256:2305892e5ad255cf08d0720ea55b1f43351a358ff7828b04c6cafe3d9324a81f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.524; amd64
	-	windows version 10.0.17763.2565; amd64

### `openjdk:18-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:d15718c1f14e027dc4cd6e3ee8662fbfcbb7e9c5ae047bfbce8847b3baaa9e9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244288666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aecf72a3a839d0103789ac1e29c571ca33c4789d759c4ec393819da1732c0f70`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Feb 2022 18:20:31 GMT
ADD file:636d5d8575ec6ddd380a3bbf41530219d37249378b4abd151d94842377cc55d9 in / 
# Fri, 11 Feb 2022 18:20:32 GMT
CMD ["/bin/bash"]
# Fri, 11 Feb 2022 19:02:04 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Feb 2022 19:02:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 11 Feb 2022 19:02:43 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:02:44 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:51:26 GMT
ENV JAVA_VERSION=18-ea+35
# Fri, 11 Feb 2022 23:51:45 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_linux-x64_bin.tar.gz'; 			downloadSha256='62a711fdc1a8f7051551113d62f8cc7e3be42e57335d11d605dab060f29a12e2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_linux-aarch64_bin.tar.gz'; 			downloadSha256='cf0298eeac8e0d1d93fb1615916e08c12cd1a0e372a132cec2e66b2a30de6815'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:51:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:010357f4c091049bd23724817a1881f575ff94d35f4c621b4f87b2876049650b`  
		Last Modified: Fri, 11 Feb 2022 18:21:24 GMT  
		Size: 42.1 MB (42105112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1b16b3652a6874ccb11ec011003800c33c1d2f3481ede4da46773eb1415faf`  
		Last Modified: Fri, 11 Feb 2022 19:12:10 GMT  
		Size: 13.5 MB (13514759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b23c3b56d41d702c95b08ce3bee75de206be11df04b8bb18cf40568fa0502`  
		Last Modified: Sat, 12 Feb 2022 00:14:57 GMT  
		Size: 188.7 MB (188668795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:48b1bfdc146145a1de65cf34338b5d99e2a09c2b06d933f9875e2504b26c6ec8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243929601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9892b28543aa139ab9ff9fb1390e97d0689061427ed910a238f10f8435f6711c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Feb 2022 18:58:36 GMT
ADD file:8d5a0dcc45ab23c7b507e80b63e5752d94837f490600ce95fb8ba8ed2f7baa2d in / 
# Fri, 11 Feb 2022 18:58:37 GMT
CMD ["/bin/bash"]
# Fri, 11 Feb 2022 19:19:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Feb 2022 19:20:44 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 11 Feb 2022 19:20:44 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:20:45 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:08:53 GMT
ENV JAVA_VERSION=18-ea+35
# Sat, 12 Feb 2022 00:09:07 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_linux-x64_bin.tar.gz'; 			downloadSha256='62a711fdc1a8f7051551113d62f8cc7e3be42e57335d11d605dab060f29a12e2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_linux-aarch64_bin.tar.gz'; 			downloadSha256='cf0298eeac8e0d1d93fb1615916e08c12cd1a0e372a132cec2e66b2a30de6815'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:09:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ffdd659a9f05cadeed9c2d5cead839f585163662ca7f847a41fd64bb4e503f0c`  
		Last Modified: Fri, 11 Feb 2022 18:59:38 GMT  
		Size: 42.0 MB (42018804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73433a5e38bf6b279d0c685ed5c2c34fcb8e2d6755228a9c6c3f3a2313bef9b`  
		Last Modified: Fri, 11 Feb 2022 19:35:51 GMT  
		Size: 14.3 MB (14305278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbd47b9449a6269d5cc52132b96fa8b070bb9faa6d6cdf0a04faf2e23948837`  
		Last Modified: Sat, 12 Feb 2022 00:33:11 GMT  
		Size: 187.6 MB (187605519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-jdk` - windows version 10.0.20348.524; amd64

```console
$ docker pull openjdk@sha256:867a3fc654566f9fc429f5d866796f2f958c5489b286b7596c6cd3b8e59e510d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2400605966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:445462a89e2738aeed3444639b9555fa3e29bb5298ba0f92f4beefb8efb2d2da`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Tue, 01 Feb 2022 02:49:40 GMT
RUN Install update ltsc2022-amd64
# Wed, 09 Feb 2022 13:37:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Feb 2022 18:40:17 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Feb 2022 18:46:45 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 09 Feb 2022 18:47:05 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 11 Feb 2022 23:19:41 GMT
ENV JAVA_VERSION=18-ea+35
# Fri, 11 Feb 2022 23:19:42 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_windows-x64_bin.zip
# Fri, 11 Feb 2022 23:19:43 GMT
ENV JAVA_SHA256=de188474290055ecb1ca874816a529859bdf60f2818a089b993f712cb7eca55b
# Fri, 11 Feb 2022 23:20:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 11 Feb 2022 23:20:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:898469748ff68223ab87b654b29fb366c1f4f2b7cfad7a37426346ea16db8dfa`  
		Size: 963.2 MB (963225591 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7062696b7aef1ca33afdf32084a532f7e3151a844eb7cb2455bcc907e0f42a58`  
		Last Modified: Wed, 09 Feb 2022 14:28:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fc5298c05f3e14d89c86be0ac333bd8cfa150ada3565e9f2736c19d8cac25b`  
		Last Modified: Wed, 09 Feb 2022 19:16:25 GMT  
		Size: 616.4 KB (616433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a2082a9f8e2d1c33d405eb96d623567e53b859d9c88db074aabd0fdf14e002`  
		Last Modified: Wed, 09 Feb 2022 19:21:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8771100366dd0834481987ac6a452860365a800b0e8e9504ad44e630ca85f2`  
		Last Modified: Wed, 09 Feb 2022 19:21:32 GMT  
		Size: 533.3 KB (533257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f673b531092ea947f4cd4584a55a6ae4920d6e33b6986f8ca5c19e7bddba718`  
		Last Modified: Fri, 11 Feb 2022 23:41:29 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f22a44ab32322afea15a6632894e2fbbe922ce23954381fcb96ab9024e640b`  
		Last Modified: Fri, 11 Feb 2022 23:41:30 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52edce9ac56e6292128bd42b01469c53e897dc6923970088cd906a63299414d5`  
		Last Modified: Fri, 11 Feb 2022 23:41:29 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df23f9f9f6dc77a1df027e587e682c631cba1003e3de0758236d3be1b5b388e7`  
		Last Modified: Fri, 11 Feb 2022 23:41:49 GMT  
		Size: 184.5 MB (184523135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5ba08e608e506256d1e966a49b07bd767d0d2c5d93a17c8344987cfad73a93`  
		Last Modified: Fri, 11 Feb 2022 23:41:30 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-jdk` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:24a51e51193e9ab2e724b967aead0ad3bebbf7b0cd7a40c2529b683e3267c894
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2898733969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ec3689d31ef2b95d7f4540b6acb7489e5a2f29219574a68c62edb29e60d0ff`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 13:09:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Feb 2022 18:42:45 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Feb 2022 18:48:26 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 09 Feb 2022 18:49:21 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 11 Feb 2022 23:21:08 GMT
ENV JAVA_VERSION=18-ea+35
# Fri, 11 Feb 2022 23:21:10 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_windows-x64_bin.zip
# Fri, 11 Feb 2022 23:21:11 GMT
ENV JAVA_SHA256=de188474290055ecb1ca874816a529859bdf60f2818a089b993f712cb7eca55b
# Fri, 11 Feb 2022 23:22:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 11 Feb 2022 23:23:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f0c1566a9285d9465334dc923e9d6fd93a51b3ef6cb8497efcacbcf64e3b93fc`  
		Last Modified: Wed, 09 Feb 2022 13:26:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b68a1fe6e4f618e81fe842c9b07d5a79ffffc2c21933db69d5c9e6105091560`  
		Last Modified: Wed, 09 Feb 2022 19:20:09 GMT  
		Size: 358.3 KB (358257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ac907de79675ad8ddc8f1bbe7505ab46561f1143ec72e0aa5199f6e3521080`  
		Last Modified: Wed, 09 Feb 2022 19:22:14 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa20c4d5b2f8ccaf2901ca9ad11be6db1a5c698aceb2ea78e874cbbdb5af5b3`  
		Last Modified: Wed, 09 Feb 2022 19:22:13 GMT  
		Size: 311.8 KB (311840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ea1afa1b874796cd6379497aa4b04f917c74e60b8bd8fa9149b7130d00e05`  
		Last Modified: Fri, 11 Feb 2022 23:42:08 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99927319cce8c63939424e959d241723f6981ed029d138be57af79516e91008a`  
		Last Modified: Fri, 11 Feb 2022 23:42:08 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137108794ce3f8707cdd18ce1e15f5d7947a3e34709c8f2cf9cb43c58316eca`  
		Last Modified: Fri, 11 Feb 2022 23:42:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed96a7047c5b385b11c146789f8d7b61ca776cf81ee00c0582bf0b110b83e2ff`  
		Last Modified: Fri, 11 Feb 2022 23:42:28 GMT  
		Size: 184.3 MB (184340616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a71f71ec66c715bd612aa8edf7cafa064372150748eaad3b9429b8c083f615`  
		Last Modified: Fri, 11 Feb 2022 23:42:08 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
