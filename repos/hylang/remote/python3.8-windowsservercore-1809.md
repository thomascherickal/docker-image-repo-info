## `hylang:python3.8-windowsservercore-1809`

```console
$ docker pull hylang@sha256:cac4ef5f5c7d3a8fc9f95dbd34c5afa41826eeefbdfb2cddbe0e5dc18098faa0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `hylang:python3.8-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull hylang@sha256:7405df93a9610f83bd61c3e5d902f48c1bd5a860521a5bab746d4c80c40c8c19
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2447862509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65938426318b858d60e6b5041c6029190c7831fdb12e72a83b5dec361e89d30e`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 30 Oct 2020 00:18:21 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 30 Oct 2020 00:31:39 GMT
ENV PYTHON_VERSION=3.8.6
# Fri, 30 Oct 2020 00:31:40 GMT
ENV PYTHON_RELEASE=3.8.6
# Fri, 30 Oct 2020 00:33:15 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:33:17 GMT
ENV PYTHON_PIP_VERSION=20.2.4
# Fri, 30 Oct 2020 00:33:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8283828b8fd6f1783daf55a765384e6d8d2c5014/get-pip.py
# Fri, 30 Oct 2020 00:33:18 GMT
ENV PYTHON_GET_PIP_SHA256=2250ab0a7e70f6fd22b955493f7f5cf1ea53e70b584a84a32573644a045b4bfb
# Fri, 30 Oct 2020 00:34:00 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:34:01 GMT
CMD ["python"]
# Fri, 30 Oct 2020 01:09:01 GMT
ENV HY_VERSION=0.19.0
# Fri, 30 Oct 2020 01:09:36 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Fri, 30 Oct 2020 01:09:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb794c56bcd1cabc090769fa40a9a01dc0b440ce7fd0dfbd8d3e17dab67ebd04`  
		Last Modified: Fri, 30 Oct 2020 00:43:41 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334bdef833ee3e719293a3e5cc2d497a10c7d8f65f05bde4912c8b1c39dc9cd5`  
		Last Modified: Fri, 30 Oct 2020 00:48:23 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2dfd09571bae793655e8a4e3840f1b415ba2153f0b82d13419c43557eb6e2c`  
		Last Modified: Fri, 30 Oct 2020 00:48:22 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016c601be9eee4dafc5fa5ab6462e3aecadfa27c26cda0569a9214d179e1b73f`  
		Last Modified: Fri, 30 Oct 2020 00:49:30 GMT  
		Size: 57.9 MB (57922512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c0c4be0b43911ea5d413b283a688e934077ced6d431f98b4245a0c7ed3d33e`  
		Last Modified: Fri, 30 Oct 2020 00:48:19 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e741d95046e3b48bb037805eb1314c4fc2be3d69763cb419ae1b867018f8106`  
		Last Modified: Fri, 30 Oct 2020 00:48:19 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce6bbf9ce88d991b496d61355ed42efec147ea7aa6d2e80540bf40e83dc880`  
		Last Modified: Fri, 30 Oct 2020 00:48:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd53a27d8357d43303e5369b561a287b78f30aa9260405e5bb4ba3e3bb61caf9`  
		Last Modified: Fri, 30 Oct 2020 00:48:31 GMT  
		Size: 10.3 MB (10292690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08530fa7527e067176728c91e33f7392e856db9c01172917d74269e9fb4f68da`  
		Last Modified: Fri, 30 Oct 2020 00:48:19 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7671d41d2e27aa81142edce05a1ff7015d6e63048e909959b6882201a8851b0c`  
		Last Modified: Fri, 30 Oct 2020 01:14:25 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccc65a01d62653b3707f9e46c5d97ce476ff30d4f8a6f10b247055260e6f639`  
		Last Modified: Fri, 30 Oct 2020 01:14:27 GMT  
		Size: 5.5 MB (5545725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da6937db839074d75e44004e729ccd4fd18efcd768dc63034d9e1502bda51c4`  
		Last Modified: Fri, 30 Oct 2020 01:14:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
