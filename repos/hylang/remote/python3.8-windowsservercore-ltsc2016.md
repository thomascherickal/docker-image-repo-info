## `hylang:python3.8-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:ea9d42753f3bafd95c2cfd97c23287d65bb848078d20f1eaf85f4de4a2310682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `hylang:python3.8-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull hylang@sha256:61856c9bf78386d141a4fca8fb27cb4501d76aedafbb9cb6fd514e153a0dc641
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821390582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f392a21b6d5422728ba60c5cb5e2af41e41882a8aae9fb579916b26d95d37b`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 21 Jul 2020 17:54:36 GMT
ENV PYTHON_VERSION=3.8.5
# Tue, 21 Jul 2020 17:54:37 GMT
ENV PYTHON_RELEASE=3.8.5
# Tue, 21 Jul 2020 17:57:08 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Tue, 04 Aug 2020 22:18:40 GMT
ENV PYTHON_PIP_VERSION=20.2.1
# Tue, 04 Aug 2020 22:18:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5578af97f8b2b466f4cdbebe18a3ba2d48ad1434/get-pip.py
# Tue, 04 Aug 2020 22:18:42 GMT
ENV PYTHON_GET_PIP_SHA256=d4d62a0850fe0c2e6325b2cc20d818c580563de5a2038f917e3cb0e25280b4d1
# Tue, 04 Aug 2020 22:20:31 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 04 Aug 2020 22:20:34 GMT
CMD ["python"]
# Tue, 04 Aug 2020 22:46:14 GMT
ENV HY_VERSION=0.19.0
# Tue, 04 Aug 2020 22:47:52 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 04 Aug 2020 22:47:54 GMT
CMD ["hy"]
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
	-	`sha256:d3d7ec3f9f2d24e997d93fb18f7ee2d26be25a890248396d7734e959a270a174`  
		Last Modified: Tue, 21 Jul 2020 18:05:09 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e8e910e5f34358935ec3a4c3ce99d111dbecca77ab2cb178fca2cce4237d2c`  
		Last Modified: Tue, 21 Jul 2020 18:05:09 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0cf46a9c2c98cffd335ca954926a0aa9f2b0cbcff6547e82a9c32ff1f28c3f`  
		Last Modified: Tue, 21 Jul 2020 18:05:19 GMT  
		Size: 57.9 MB (57874585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1848043873a0a791131b74e6194cc480300081ecd76591270dcc21547639e7d9`  
		Last Modified: Tue, 04 Aug 2020 22:26:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c0a7ee203976b5cfbfaefe3bbfa2672ae24fa0bad6a8eaf5f12b9222062c04`  
		Last Modified: Tue, 04 Aug 2020 22:26:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c715f9abf2dc3ccb5a3f1b5e13ee0f8a381a4f071f629d6ac925a296522d58`  
		Last Modified: Tue, 04 Aug 2020 22:26:04 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ee734bbd528735b4c270862efb739a1e0313a335692017c328f7cc157c217c`  
		Last Modified: Tue, 04 Aug 2020 22:26:08 GMT  
		Size: 15.4 MB (15411851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb447b6c2d613165abd7dac03e1764ec71c74df676b93334daf3ab2e8f7fa9b`  
		Last Modified: Tue, 04 Aug 2020 22:26:04 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efae7ab1f43619f61a120d6b544f2e4bc134c927dcd28d4dc03104c2d189bb5`  
		Last Modified: Tue, 04 Aug 2020 22:52:17 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c0d91108d1249bcc0f4407055f304b59c02fa16218c2538aa934f0a4ccea6d`  
		Last Modified: Tue, 04 Aug 2020 22:52:20 GMT  
		Size: 10.6 MB (10631780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555d00840dc8c6201c6a8c5cea0cc1e6755ccb039ea19d68000c7c4089013efc`  
		Last Modified: Tue, 04 Aug 2020 22:52:17 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
