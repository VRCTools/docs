---
title: Texture2D Loader
nav_order: 251
parent: Local Converters
layout: component
component_name: Local Texture2D Loader Converter
since_version: 0.1.0
---

Attempts to load a texture using the url provided by a local URL value.

## Parameters

| Parameter Name            | Default Value | Description                                                                                               |
|---------------------------|---------------|-----------------------------------------------------------------------------------------------------------|
| Local Url                 | None          | Value from which to pull the object state.                                                                |
| Local Texture2D           | None          | Texture value to which the image will be written.                                                         |
| Default Texture           | None          | Default texture to which the image will be set if no URL is specified.                                    |
| Loading Texture           | None          | Texture to which the image will be set while downloading.                                                 |
| Error Texture             | None          | Texture to which the image will be set if an error occurs and no more specific image has been configured. |
| Access Denied Texture     | None          | Texture to which the image will be set if access to the given url is denied.                              |
| Download Error Texture    | None          | Texture to which the image will be set if the given url fails to download.                                |
| Invalid Error Texture     | None          | Texture to which the image will be set if the given url does not point to a supported image file.         |
| Too Many Requests Texture | None          | Texture to which the image will be set if too many download requests have been sent recently.             |
| Invalid URL Texture       | None          | Texture to which the image will be set if the URL itself is invalid.                                      |

**Note:** Generally `Error Texture` is picked when an error occurs unless one of the more specific variations has been
given.