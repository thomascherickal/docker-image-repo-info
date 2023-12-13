## `openjdk:22-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:96209d5f2acfc511d52e0f9acce821a64eb9de771a301e3f78f6d9c6d5f99e84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `openjdk:22-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull openjdk@sha256:1a301119fc5890c16ca9421d80a8d8d9a682f9e25687331d5650adcfaed1951b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087668804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540d6305381c0f2709ef5bc71c04fac5820594ea94e4667fc229476a10c6668e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Tue, 12 Dec 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 02:06:37 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Dec 2023 02:14:22 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 13 Dec 2023 02:14:45 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 13 Dec 2023 02:14:46 GMT
ENV JAVA_VERSION=22-ea+27
# Wed, 13 Dec 2023 02:14:47 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_windows-x64_bin.zip
# Wed, 13 Dec 2023 02:14:48 GMT
ENV JAVA_SHA256=522347f78607019a5c2d2478846c2ca0715ee700a7db3f78aff024e9935b1091
# Wed, 13 Dec 2023 02:16:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 13 Dec 2023 02:16:08 GMT
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
	-	`sha256:95d0c853ded9068434b9128a8016b3ae5e18f748f62801c7bb6e6092495300ec`  
		Last Modified: Wed, 13 Dec 2023 00:02:39 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7817aaa693cefbfd0445b1f134cd6c870f5b31f9fa34a8deb5924f745a5407`  
		Last Modified: Wed, 13 Dec 2023 02:21:14 GMT  
		Size: 466.4 KB (466444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbdd67272665d1191a996e1b04d87eb52af36f6bc046d1101ac2c6b05d35a9ea`  
		Last Modified: Wed, 13 Dec 2023 02:23:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd35b2335fa310a8cb3642b720740198e5efdf3361cb73e230149f020277e4d9`  
		Last Modified: Wed, 13 Dec 2023 02:23:12 GMT  
		Size: 279.3 KB (279265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc1eb3fc9c46ac72487f84a148cb23bd4053a577c5815c0464495200b342e63`  
		Last Modified: Wed, 13 Dec 2023 02:23:09 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe02c673f75afa72a15a6f8de5f1d1d57b0abd9c5222fcffd155cb7e4154d46`  
		Last Modified: Wed, 13 Dec 2023 02:23:09 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92916b693abd25c6cd6beeafadaa223f0e8b573f44510af504613cc2560a0435`  
		Last Modified: Wed, 13 Dec 2023 02:23:09 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0b6726397e440b4ea6980ed8e4bd7c396759d11f8182c40ca5c8d3b1a447ec`  
		Last Modified: Wed, 13 Dec 2023 02:23:29 GMT  
		Size: 197.6 MB (197641508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a299647e233c5e25e1adbcc23ec116ffc0e5721cf6d6ba66004b770637489bb3`  
		Last Modified: Wed, 13 Dec 2023 02:23:09 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
