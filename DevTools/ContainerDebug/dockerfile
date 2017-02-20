# escape=`

FROM microsoft/nanoserver

ARG VS_REMOTE_DEBUGGER_PATH
ARG VS_OUT_DIR

ADD $VS_REMOTE_DEBUGGER_PATH "c:\windows"

VOLUME $VS_OUT_DIR

WORKDIR $VS_OUT_DIR

ENTRYPOINT msvsmon.exe /noauth /anyuser /silent /nostatus /noclrwarn /nosecuritywarn /nofirewallwarn /nowowwarn /timeout:36000