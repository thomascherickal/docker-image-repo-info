## `python:rc-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:0e8650d4e9f8f4031666548fee60444ba8c1bbd3a2d45241ab49c90f0a059fb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `python:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull python@sha256:330d8f044d646012506013f62cd44c6b9257886e1c286f81442f003e85556a22
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5862705468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4838d61b0b205d76afb9e451fe4a2ecf7826fed2f38c272fa45b793d83e06c22`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:15:18 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 14 Apr 2021 16:15:19 GMT
ENV PYTHON_VERSION=3.10.0a7
# Wed, 14 Apr 2021 16:15:20 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 14 Apr 2021 16:18:14 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 27 Apr 2021 22:15:27 GMT
ENV PYTHON_PIP_VERSION=21.1
# Tue, 27 Apr 2021 22:15:28 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ab9dde151f662745c13461f00c453dcf32a51ea9/public/get-pip.py
# Tue, 27 Apr 2021 22:15:28 GMT
ENV PYTHON_GET_PIP_SHA256=0ed17e859b835ad5bf00851f4dc8bbc3520c13dfff6c131d410cdb3a92ff0af9
# Tue, 27 Apr 2021 22:17:25 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 27 Apr 2021 22:17:26 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b4598ab88dab64b25b4257872564af9825cc6cd41fc8cc1ad11c32958d0da9`  
		Last Modified: Wed, 14 Apr 2021 16:39:38 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1311eb2840794f0fcf4ebfe6e57fefbd0bd92a00118e655c18e3a75392e4cd54`  
		Last Modified: Wed, 14 Apr 2021 16:39:41 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09619313575c6e229a1fa5368aca94a22dbcb2460d205d2df906d7985431214`  
		Last Modified: Wed, 14 Apr 2021 16:39:42 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208f3c11f1d3691183615afa032ff11a8bad281acb95472f389252c31370c0df`  
		Last Modified: Wed, 14 Apr 2021 16:39:50 GMT  
		Size: 56.3 MB (56263121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d980761de8da6ffb56022d4af5fb9bcc9197f116395162338b4e6a302a80234`  
		Last Modified: Tue, 27 Apr 2021 22:24:43 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77d2f8a35900d8a50e361ebd706621e18354d84819a408976349b162d8a6e10`  
		Last Modified: Tue, 27 Apr 2021 22:24:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74137b0693c6d9ef09b779f0cf5f2ebf6d695080d5d4c08d6d9f47cd962b5be`  
		Last Modified: Tue, 27 Apr 2021 22:24:44 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9c4f720438cbb2989630b486941ea3594bbf9106db2fe7386a5eedc7c91433`  
		Last Modified: Tue, 27 Apr 2021 22:24:56 GMT  
		Size: 11.5 MB (11547241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b19091fde04c699a4f14f5f72efa319bd193ea67d2226127f9141b1823930e`  
		Last Modified: Tue, 27 Apr 2021 22:24:46 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
