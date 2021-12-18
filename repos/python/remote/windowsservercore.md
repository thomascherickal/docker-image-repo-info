## `python:windowsservercore`

```console
$ docker pull python@sha256:9bda3432a0867411fc0c893a27a9110a5fb79f344537effb7ae124ea8ffcb63f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `python:windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull python@sha256:4669363f7f17d1ff860fa9cf68f3dbc336f6992bae60bf5d5c885cf98c2a861d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2244156252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a36da98fb07c5f234b948a6684894c10cc237ecd4b7ad620c271372a6a2cf09`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 04:37:55 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 18 Dec 2021 04:44:49 GMT
ENV PYTHON_VERSION=3.10.1
# Sat, 18 Dec 2021 04:44:50 GMT
ENV PYTHON_RELEASE=3.10.1
# Sat, 18 Dec 2021 04:46:15 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 04:46:18 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 18 Dec 2021 04:46:19 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 18 Dec 2021 04:46:20 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Sat, 18 Dec 2021 04:46:21 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Sat, 18 Dec 2021 04:47:18 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 04:47:19 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ff57c573acaff14c082599c0e5869774744dfcb78f52c78a5d4cf81a917c7d`  
		Last Modified: Sat, 18 Dec 2021 05:07:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e0906a9bf464092a4cd801e452c2cbc66828344784ed0f76ca9d02102f006d`  
		Last Modified: Sat, 18 Dec 2021 05:09:26 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51648e7c8627e23a9f24dcb46c6bd264f4282867ee356112eae1783ba3e7b3fb`  
		Last Modified: Sat, 18 Dec 2021 05:09:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3688f5ea6ff3c96b500da910a2fbb8a6d74062747e2c31c127681d68b0e0d3d6`  
		Last Modified: Sat, 18 Dec 2021 05:09:34 GMT  
		Size: 46.7 MB (46666867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddd4699facd2ebcbd047514b29b50ee7057cddb70eabb69e0f1dbaa67726de0`  
		Last Modified: Sat, 18 Dec 2021 05:09:26 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4c1a2ed038701f06137a6b318ca737762cf005a178ad9e24a03c6bedcf24b6`  
		Last Modified: Sat, 18 Dec 2021 05:09:23 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfbfc16110230baaafb9a8e95437136a1ac89bc074fe24d6e2b696c113690b9`  
		Last Modified: Sat, 18 Dec 2021 05:09:23 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0825a5b94792d264e1c4e46ff02724652d84d730503318b425bca90337edc528`  
		Last Modified: Sat, 18 Dec 2021 05:09:23 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2078dc836a220bff5370f3d521d7af7f88ef5c657b7a9fdac8f903acb80611a2`  
		Last Modified: Sat, 18 Dec 2021 05:09:31 GMT  
		Size: 6.7 MB (6704989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23dfce5e21c11cee25cf914cf9ffe7ecbaf6a56a7e6b2362024054b0cdfda8d`  
		Last Modified: Sat, 18 Dec 2021 05:09:23 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull python@sha256:e8d7a904ffcdf98159c8c78fccaddad666d16a96b31d662509e61deb5d524157
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2761530945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d87d87b1f3436e3b8aed50b886072422495df077fe4437f9f8553ff7700ac0cf`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 17 Dec 2021 23:40:28 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 18 Dec 2021 04:47:32 GMT
ENV PYTHON_VERSION=3.10.1
# Sat, 18 Dec 2021 04:47:33 GMT
ENV PYTHON_RELEASE=3.10.1
# Sat, 18 Dec 2021 04:49:30 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 04:49:32 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 18 Dec 2021 04:49:33 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 18 Dec 2021 04:49:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Sat, 18 Dec 2021 04:49:35 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Sat, 18 Dec 2021 04:51:11 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 04:51:12 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacd9d567f7b3b5dfa281ce42662ff8283bc17b367e2701cd822bee574e07bdc`  
		Last Modified: Fri, 17 Dec 2021 23:48:12 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca68b85bd2250cf3664ec86fa7f91e4f1630e172ff7ed46a846b65f8966fbb92`  
		Last Modified: Sat, 18 Dec 2021 05:09:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37710c2637bded9ed1b127d82d39f2aa6257e8c01bc1ef5330299007cd6bcaab`  
		Last Modified: Sat, 18 Dec 2021 05:09:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eae8b13642bfdab6e26111ffb1c3bb99682e73645726828496a4031c88b651`  
		Last Modified: Sat, 18 Dec 2021 05:10:40 GMT  
		Size: 46.4 MB (46430952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e29bef7d1a601f64b80ec6c7d81a95512aa0fcfb558bd0b56046f4ab4c521f`  
		Last Modified: Sat, 18 Dec 2021 05:09:51 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c96066819f278b6553a51caf2337baf400e7bf91db37b71b103eb34d8816b`  
		Last Modified: Sat, 18 Dec 2021 05:09:49 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97925f31f52df7e95ed8976795b32bca851902d2abdf0d29d06bc1bfad28bd9f`  
		Last Modified: Sat, 18 Dec 2021 05:09:49 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f155ca016e7e5ec8775c3685c7b16dd0db029bec25f5b4910913db108eecbe2`  
		Last Modified: Sat, 18 Dec 2021 05:09:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2952bc04b953ebaa199b01edf9fd84bd39dd3ab8b1a70c840ad830ba0be3348`  
		Last Modified: Sat, 18 Dec 2021 05:09:52 GMT  
		Size: 6.5 MB (6482750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab14f8c75d5736a447ab866df5d893d3e716857a93aa973f46cf15fe125e4859`  
		Last Modified: Sat, 18 Dec 2021 05:09:49 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull python@sha256:a5292ca15ff16d8b59da90b4bbfe6faa50e3cf95abf1d462682d8795f88f60fd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6332013193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd33397f0c4458c9a37d12ad5638b76a986049698bf6b67fde54a5c5d91c8e69`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 04:51:29 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 18 Dec 2021 04:51:30 GMT
ENV PYTHON_VERSION=3.10.1
# Sat, 18 Dec 2021 04:51:31 GMT
ENV PYTHON_RELEASE=3.10.1
# Sat, 18 Dec 2021 04:53:46 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 04:53:47 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 18 Dec 2021 04:53:48 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 18 Dec 2021 04:53:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Sat, 18 Dec 2021 04:53:50 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Sat, 18 Dec 2021 04:55:35 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 04:55:36 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b032dea64559edddd8d7d51de64c99d62a953cc056d3a265d67caf85bb31e91`  
		Last Modified: Sat, 18 Dec 2021 05:10:59 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c613836f41f0f6d29ed53b7330d2645f037257110151715c72490fe9a07c73`  
		Last Modified: Sat, 18 Dec 2021 05:10:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f96a3bdb9b0f6630cc8f201f383efb0bb40581fb18884a92452d834cc534dfe`  
		Last Modified: Sat, 18 Dec 2021 05:10:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aab7a379552fd144ce95401f794206ed41264f1b7bb6166e533eebd2dc6116d`  
		Last Modified: Sat, 18 Dec 2021 05:11:53 GMT  
		Size: 50.8 MB (50836365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec543d622faa4d509208e01302d2fb819cd7e822f05e7031e72eeac3fe72c93`  
		Last Modified: Sat, 18 Dec 2021 05:10:57 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd302f1dfff0f7e7d550f3962db64a5f36765623fa65a0b4bb4bbcfdc4e15b57`  
		Last Modified: Sat, 18 Dec 2021 05:10:55 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20628a6a839fa65417a788f6e11f25da99a2d37a16206ffd9e2a66fa9bc844f6`  
		Last Modified: Sat, 18 Dec 2021 05:10:54 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19e8a777ed491675a710ebbde773378c300e9999fe26a7e3c7918cc1ab5da48`  
		Last Modified: Sat, 18 Dec 2021 05:10:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a9a74bc032c0c93499bd575f9f1cc2ac87fa2b41581d510111ed8deb0b0432`  
		Last Modified: Sat, 18 Dec 2021 05:11:02 GMT  
		Size: 6.4 MB (6449376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f12d8ba0e32cde28e32d88cf709be966c6d9e3499c19f23f4cd4cde5e3c511`  
		Last Modified: Sat, 18 Dec 2021 05:10:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
