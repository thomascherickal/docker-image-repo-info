## `openjdk:23-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:d99ed42603f417b9f2a4b3b392714d3f7b142f5cb383850b0239ce9cbc225bf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `openjdk:23-jdk-windowsservercore` - windows version 10.0.20348.2159; amd64

```console
$ docker pull openjdk@sha256:f6ebf263caf314eb11dd47d1a72ac337c91744be25a4266d8659ea47e0eb62af
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087910182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647bd8f07e91045a3d30463d680f2685a01ccf386be35af45a086d0cf5f4f9ed`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Fri, 15 Dec 2023 22:55:23 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 15 Dec 2023 22:55:39 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:55:40 GMT
ENV JAVA_HOME=C:\openjdk-23
# Fri, 15 Dec 2023 22:55:45 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:55:46 GMT
ENV JAVA_VERSION=23-ea+1
# Fri, 15 Dec 2023 22:55:46 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_windows-x64_bin.zip
# Fri, 15 Dec 2023 22:55:47 GMT
ENV JAVA_SHA256=b60d20ad423ec31c88a18679854a31bdef66003224227d86dcbd10781fe14db1
# Fri, 15 Dec 2023 22:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:56:10 GMT
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
	-	`sha256:febf4a241d42e30659860321594cdc1835cf88940ed65bcb5437baefa660ed19`  
		Last Modified: Fri, 15 Dec 2023 22:56:17 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b21110e546408563bab2f253c866475bd0ebd8181afd34d913dd24ef57bc67`  
		Last Modified: Fri, 15 Dec 2023 22:56:18 GMT  
		Size: 505.6 KB (505551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e5a5ccae27786feb6afcb52b0de34fce9409dc99ed6b7fda05b2dc9c8317b5`  
		Last Modified: Fri, 15 Dec 2023 22:56:17 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb9d041558efee289872f90141037b36fbce446d47061b3e7bd16a5dea233e0`  
		Last Modified: Fri, 15 Dec 2023 22:56:18 GMT  
		Size: 356.7 KB (356718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5cb2c8db90ba2ed5d2da8f9035b24441b1186bc19fa919c77b9dac6a947054`  
		Last Modified: Fri, 15 Dec 2023 22:56:16 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b6692c963c7de761f4c19f8c994da94ee0973d3155f3aa94db14ac9f0be219`  
		Last Modified: Fri, 15 Dec 2023 22:56:15 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a1d5fee6c9465437de8442e0d2a5d91f6c41f9879bae6cb30858a15b01b20d`  
		Last Modified: Fri, 15 Dec 2023 22:56:15 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71df1dce496a0203c1051ed544387659c3bd163115bd7a7c1b63a880a2b3f53c`  
		Last Modified: Fri, 15 Dec 2023 22:56:27 GMT  
		Size: 197.8 MB (197766556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1ac19dae54d2dee494e89695dcae4b4d72fd0c889be472465443a362eef5ca`  
		Last Modified: Fri, 15 Dec 2023 22:56:15 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:23-jdk-windowsservercore` - windows version 10.0.17763.5206; amd64

```console
$ docker pull openjdk@sha256:b830cf78dde50071a036884bb94fd1bb6175409e16fc577746ef7db7290fa6ff
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258285936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b93826679e943e960222935631add0dfdb52410c102e897ac4e8a1bfe0e29ac`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Fri, 15 Dec 2023 22:20:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 15 Dec 2023 22:21:15 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:21:16 GMT
ENV JAVA_HOME=C:\openjdk-23
# Fri, 15 Dec 2023 22:21:36 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:21:36 GMT
ENV JAVA_VERSION=23-ea+1
# Fri, 15 Dec 2023 22:21:37 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_windows-x64_bin.zip
# Fri, 15 Dec 2023 22:21:37 GMT
ENV JAVA_SHA256=b60d20ad423ec31c88a18679854a31bdef66003224227d86dcbd10781fe14db1
# Fri, 15 Dec 2023 22:22:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:22:16 GMT
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
	-	`sha256:41b07be79186bada004046f6b749cb6555157f896380e88635714586b3b96e3a`  
		Last Modified: Fri, 15 Dec 2023 22:22:20 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d96aca320c72c08112922be54c59d0cdeeadfb127ce8e0a7befd5f3976db09`  
		Last Modified: Fri, 15 Dec 2023 22:22:20 GMT  
		Size: 485.4 KB (485386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38467a9a9f8a64bf926ea81cd7db78dfcfe07d24eb3d890adc15a843cf6cef2b`  
		Last Modified: Fri, 15 Dec 2023 22:22:20 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af5242e82081edaa4b479eeffdd04a62c5c42ee16c08b31d1804e31f1eb4d68`  
		Last Modified: Fri, 15 Dec 2023 22:22:20 GMT  
		Size: 330.0 KB (329963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d27aa5f28e6d90fc737293538f8746708be4133598f7af304e23e09b85c15f`  
		Last Modified: Fri, 15 Dec 2023 22:22:19 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24c73731f85bc23cd10201ba4a9c8e37f3c2605ef556c3f9ca83b28c7293e3d`  
		Last Modified: Fri, 15 Dec 2023 22:22:19 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edadf6896caeb6df946fc3e6e77c18e3ee3fbaf9897d47eff04eab5186cfadc4`  
		Last Modified: Fri, 15 Dec 2023 22:22:19 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd87cc9c84e32ecd1b704df4fca63235b4a12662884bee2ed49eb20ee04c028`  
		Last Modified: Fri, 15 Dec 2023 22:22:31 GMT  
		Size: 197.8 MB (197753833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714de47a6a6f9b79b48c738744597137bee13da27ed4a8721186e926c1f150dc`  
		Last Modified: Fri, 15 Dec 2023 22:22:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
