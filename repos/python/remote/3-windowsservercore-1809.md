## `python:3-windowsservercore-1809`

```console
$ docker pull python@sha256:f5427322fdc921c2595ac313a247e1b589801180ef7b13e09b5f60c1ccc937e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `python:3-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull python@sha256:056884759b451a89cef2e62e23113bfd48f27acad349666af106373ca7b48cdf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2458497923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aad7e970de2886736cb0cfee59a08de2a7ebbeedefa631652036dd9e4536f5e`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 17:13:40 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 11 Nov 2020 17:20:33 GMT
ENV PYTHON_VERSION=3.9.0
# Wed, 11 Nov 2020 17:20:34 GMT
ENV PYTHON_RELEASE=3.9.0
# Wed, 11 Nov 2020 17:22:12 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 02 Dec 2020 01:20:12 GMT
ENV PYTHON_PIP_VERSION=20.3
# Wed, 02 Dec 2020 01:20:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2357a5f805565496648ebf597bcffe9e2d9ce379/get-pip.py
# Wed, 02 Dec 2020 01:20:13 GMT
ENV PYTHON_GET_PIP_SHA256=7f28b41ce236af61a00dfcbd6fd38c52d46488ece91fb4585b95775b076bbc85
# Wed, 02 Dec 2020 01:21:00 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 02 Dec 2020 01:21:01 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba27fafdef0dd2d90225160fe1fa0393acbcfbe112b6442bf74fa7f41916bcfb`  
		Last Modified: Wed, 11 Nov 2020 17:38:15 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919bf62a63dcc1a613cb9e396022f5204b19dbcde218fe6eb473996c61aa6ff6`  
		Last Modified: Wed, 11 Nov 2020 17:39:38 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48f5de8a3e68f04294d2e4685b27b65ceb2f93cb61fc39bacb100c2daf7bc1c`  
		Last Modified: Wed, 11 Nov 2020 17:39:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2429988255b52ff1002cfc6656f4e7907f5dd542f690168ab44808652acf4f61`  
		Last Modified: Wed, 11 Nov 2020 17:39:48 GMT  
		Size: 60.1 MB (60103518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d8e4641ab596ddfb209daa2b12c1c72dfcf2e9459ce84a39ab2ce8004eeecd`  
		Last Modified: Wed, 02 Dec 2020 01:28:43 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674346756705a0ae0c0de8b8d1da40c8794f475d7955d6f13b30fa8e0f5c50b4`  
		Last Modified: Wed, 02 Dec 2020 01:28:43 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55913752f7106a4adc266266b81da2697f0bfcc765011d84a794d34a9e96daa`  
		Last Modified: Wed, 02 Dec 2020 01:28:43 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e09b4207e1d627a770d150209c150c3fc21d61cabf87c3eebc63f5e9e2fe0c`  
		Last Modified: Wed, 02 Dec 2020 01:28:45 GMT  
		Size: 10.4 MB (10356067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae6d0bb2dd651eccaaf2f2f7fce2e89e1362209ec72325d8940b4d0d33b5ed4`  
		Last Modified: Wed, 02 Dec 2020 01:28:44 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
