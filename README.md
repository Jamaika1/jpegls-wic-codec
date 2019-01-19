# JPEG-LS Windows Codec

This Windows codec plugin makes it possible to **decode** JPEG-LS (.jls) files in Windows aplications that can used codecs that provide the Windows Imaging Component (WIC) API. This allows e.g., to see JPEG-LS files in Windows PhotoViewer and Windows Explorer.

## WIC

### Codec Identity

The following table provides codec identification information

|||
|---|---|
|Formal Name|JPEG-LS Format|
|File Name Extension|.jls|
|MIME type| image/jls|
|Specification Support| JPEG-LS (ISO/IEC 14495-1), SPIFF header (ISO/IEC 10918-3)|

The following table lists the GUIDs used to identify the native JPEG-LS codec components.

|Component|Friendly Name|GUID
|---|---|---|
|Container Format|GUID_ContainerFormatJpegLS|52c25458-282d-4ef4-a69f-021bb2984543
|Decoder|CLSID_JpegLSDecoder|e57dc18b-019c-47f2-8ed0-bf587be4ff1b|

## Build Instructions

1. Open Visual Studio 20175 or newer and open jpeg-wic-codec.sln
2. Batch build all projects

## Installation

1. open a command prompt with elevated rights
2. navigate to folder with the jpegls-wic-codec.dll
3. execute:

```shell
regsvr32 jpegls-wic-codec.dll
```

## Uninstall

1. open a command prompt with elevated rights
2. navigate to folder with the jpegls-wic-codec.dll
3. execute:

```shell
regsvr32 -u jpegls-wic-codec.dll
```