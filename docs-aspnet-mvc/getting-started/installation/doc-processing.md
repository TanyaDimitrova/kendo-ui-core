---
title: Document Processing Libraries
page_title: Document Processing Libraries| Download and Installation | Telerik UI for ASP.NET MVC
description: "Get started with Telerik UI for ASP.NET MVC and import and export content between different formats and work with archive files by using Telerik Document Processing."
slug: docsprocessing_aspnetmvc
previous_url: /doc-processing, /getting-started/doc-processing
position: 6
---

# Telerik Document Processing

Telerik Document Processing is a set of UI-independent and cross-platform libraries that let you process content between different formats and work with archive files.

## List of Libraries

Telerik Document Processing includes the following libraries:

* [RadPdfProcessing](http://docs.telerik.com/devtools/document-processing/libraries/radpdfprocessing/overview)&mdash;Create, import, and export PDF documents.
* [RadSpreadProcessing](http://docs.telerik.com/devtools/document-processing/libraries/radspreadprocessing/overview)&mdash;Create, modify, and save spreadsheet documents.
* [RadSpreadStreamProcessing](http://docs.telerik.com/devtools/document-processing/libraries/radspreadstreamprocessing/overview)&mdash;Export large `XLSX` and `CSV` spreadsheet documents with low memory footprint and great performance.
* [RadWordsProcessing](http://docs.telerik.com/devtools/document-processing/libraries/radwordsprocessing/overview)&mdash;Create, import, and export `DOCX`, `HTML`, `RTF`, and `TXT` documents, and export them to PDF.
* [RadZipLibrary](http://docs.telerik.com/devtools/document-processing/libraries/radziplibrary/overview)&mdash;Compress and decompress `ZIP` files.

## Supported File Formats

The Telerik Document Processing libraries support the following file formats:

* `DOCX`
* `HTML`
* `RTF`
* `TXT`
* `PDF`
* `XLSX`
* `CSV`
* `ZIP`

## Available Assemblies

Telerik Document Processing supports [.NET Framework 4.0](https://dotnet.microsoft.com/download/dotnet-framework/net40) and [.NET Framework 4.5](https://www.microsoft.com/en-us/download/details.aspx?id=30653) or later versions. To handle the demands of your project, take the required assembly from the `Bin40` or `Bin45` folder respectively:

* `Telerik.Windows.Documents.Core.dll`&mdash;The main assembly from the Telerik Document Processing libraries. Required when you plan to use the library.
* `Telerik.Windows.Documents.Flow.dll`&mdash;The assembly is part of the Word (text) processing library. Required for processing `HTML`, `DOCX`, `RTF`, and `TXT` documents.
* `Telerik.Windows.Documents.Flow.FormatProviders.Pdf`&mdash;The assembly allows for exporting of flow documents, such as `DOCX` and `RTF`, to PDF.
* `Telerik.Documents.SpreadsheetStreaming.dll`&mdash;The main assembly for generating huge spreadsheet files and using minimum resources.
* `Telerik.Windows.Documents.Fixed.dll`&mdash;The assembly is required when processing PDF documents.* `Telerik.Windows.Documents.Spreadsheet.dll`&mdash;The main assembly for spreadsheet processing. Required when processing `XLSX`, `CSV`, and `TXT` documents.
* `Telerik.Windows.Documents.Spreadsheet.FormatProviders.OpenXml.dll`&mdash;The assembly is required when processing `XLSX` documents.
* `Telerik.Windows.Documents.Spreadsheet.FormatProviders.Pdf.dll`&mdash;The assembly is required when processing PDF documents.
* `Telerik.Windows.Zip.dll`&mdash;The assembly of the [**Telerik Zip Library**](http://demos.telerik.com/aspnet-ajax/ziplibrary/examples/overview/defaultcs.aspx). Required when working with zipped formats, such as `DOCX` and `XLSX`, and PDF.
* `Telerik.Windows.Zip.Extensions.dll`&mdash;The assembly extends `Telerik.Windows.Zip` with additional helper methods (Zip Extensions).

## Licensing

Telerik Document Processing is available as part of the following suites:

* DevCraft
* Telerik UI for ASP.NET AJAX
* Telerik UI for ASP.NET MVC
* Telerik UI for ASP.NET Core
* Telerik UI for WPF
* Telerik UI for WinForms
* Telerik UI for Silverlight

## See Also

* [Get Started with Telerik Document Processing](http://docs.telerik.com/devtools/document-processing/installation-and-deployment/installing-on-your-computer)
* [Telerik UI for ASP.NET MVC Overview]({% slug overview_aspnetmvc %})
