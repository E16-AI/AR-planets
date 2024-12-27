---
uid: arfoundation-exif-data
---
# EXIF data

Please check the following table to know what EXIF tags are supported. Please refer to this [link](https://web.archive.org/web/20190624045241if_/http://www.cipa.jp:80/std/documents/e/DC-008-Translation-2019-E.pdf) to understand the EXIF specification in greater detail.

| Supported EXIF Tag Name | EXIF 2.32 Specification |
| :---------------------- | :---------------------- |
| ApertureValue | The lens aperture. The unit is the APEX (Additive System of Photographic Exposure) value. |
| BrightnessValue | The value of brightness. The unit is the APEX value. Ordinarily it is given in the range of -99.99 to 99.99. |
| ColorSpace | The color space information tag (ColorSpace) is always recorded as the color space specifier. Normally sRGB (=1) is used to define the color space based on the PC monitor conditions and environment. If a color space other than sRGB is used, Uncalibrated (=FFFF.H) is set. Image data recorded as Uncalibrated may be treated as sRGB when is converted to Flashpix. |
| ExposureBiasValue | The exposure bias. The unit is the APEX value. Ordinarily it is given in the range of -99.99 to 99.99. |
| ExposureTime | Exposure time, given in seconds (sec). |
| FNumber | The F number, also known as F-stop, is the ratio of a lens's focal length to its aperture diameter. Refer to Adobe's [What is f-stop on a camera?](https://www.adobe.com/creativecloud/photography/discover/f-stop.html) to learn more. |
| Flash | This tag indicates the status of flash when the image was shot. Bit 0 indicates the flash firing status, bits 1 and 2 indicate the flash return status, bits 3 and 4 indicate the flash mode, bit 5 indicates whether the flash function is present, and bit 6 indicates "red eye" mode. |
| FocalLength | The actual focal length of the lens, in mm. Conversion is not made to the focal length of a 35 mm film camera. |
| PhotographicSensitivity | This tag indicates the sensitivity of the camera or input device when the image was shot. More specifically, it indicates one of the following values that are parameters defined in ISO 12232: standard output sensitivity (SOS), recommended exposure index (REI), or ISO speed. Accordingly, if a tag corresponding to a parameter that is designated by a SensitivityType tag is recorded, the values of the tag and of this PhotographicSensitivity tag are the same. However, if the value is 65535 (the maximum value of SHORT) or higher, the value of the tag shall be 65535. When recording this tag, the SensitivityType tag should also be recorded. In addition, while "Count = Any", only 1 count should be used when recording this tag. Note that this tag was referred to as "ISOSpeedRatings" in versions of this standard up to Version 2.21. |
| MeteringMode | The metering mode. Default = 0. 0 = Unknown. 1 = Average. 2 = CenterWeightedAverage. 3 = Spot. 4 = MultiSpote. 5 = Pattern. 6 = Partial. 255 = Other. Other = reserved. |
| ShutterSpeedValue | Shutter speed. The unit is the APEX value. |