# EVO PDF Client for .NET Core


[![EVO PDF Logo Image](http://www.evopdf.com/images/evopdf-logo-banner.jpg)](http://www.evopdf.com/netcore-html-to-pdf-converter.aspx)

[Features](http://www.evopdf.com/netcore-html-to-pdf-converter.aspx) | [Online Demo](http://www.evopdf.com/evopdf-client-netcore-html-to-pdf-demo/) | [Documentation](http://www.evopdf.com/documentation/evopdf-client-netcore/) | [Free Trial](http://www.evopdf.com/download.aspx) | [Licensing](http://www.evopdf.com/buy.aspx) | [Support](http://www.evopdf.com/contact.aspx)

**EVO PDF Client library for .NET Core** can be easily integrated in any application targeting the .NET Core or .NET Standard 2.0 and above to create, read, edit and save PDF documents.

The library offers the **HTML to PDF**, **Word to PDF**, **Excel to PDF**, **PDF to Text**, **PDF to Image**, **PDF to HTML** and **PDF Images Extractor** components from EVO PDF Toolkit in a single library under a single namespace that you can access in your .NET applications.

## Components and Features

* HTML to PDF Converter with advanced support for CSS3, SVG, Web Fonts and JavaScript
* Automatically create PDF links, forms, bookmarks and table of contents from HTML tags
* Place content from multiple HTML documents at any position in PDF pages, headers or footers
* HTML to Image Converter to create JPEG, PNG and Bitmap raster images from HTML documents
* HTML to SVG Converter to create high quality vector images from HTML documents
* Create PDF documents with text, graphics, images, headers and footers
* Create PDF documents with security features and digital signatures
* Create interactive PDF documents with forms, internal links, text notes and JavaScript actions
* Edit, stamp and merge PDF documents
* Word to PDF Converter
* Excel to PDF Converter
* PDF to Image Converter
* PDF to HTML Converter
* PDF to Text Converter
* Search text in PDF
* Extract images from PDF
 

## Compatibility

The client library for .NET Core is compatible with any platform which supports .NET Standard 2.0 or above, including the platforms listed below:

* .NET Core 7, 6, 5, 3, 2, .NET Standard 2.0 , .NET Framework 4.6.2 (and above)
* Windows, Linux, macOS, Azure including App Service and Functions
* Any type of application including Web, Console and Desktop applications


## Getting Started

Before starting to use the EVO PDF Client for .NET Core in your applications you first have to install the EVO PDF Server.
The server can be installed as Azure Cloud Service Worker Role, Azure Cloud Service Web Role, Azure Service Fabric Application, IIS ASP.NET Web Application or Windows Service. 

### EVO PDF Server

EVO PDF Server can be downloaded from [EVO PDF Downloads](http://www.evopdf.com/download.aspx) page of the website, under *Download EVO PDF Server* section.
EVO PDF Server package contains the server files and detailed installation instructions for each platform.

After the EVO PDF Server was installed, you are ready to use the EVO PDF Client Library for .NET Core in your applications.

### C# Code Sample

Copy the C# code lines from the section below to use the HTML to PDF Converter component to create a PDF document from a web page or from a HTML string and save the result to a memory buffer for further processing or to a PDF file.
The EVO PDF Client for .NET Core API is made available to your application by the ```using EvoPdfClient;``` statement from first line.

The 'server_ip' is assigned during server installation and it can be omitted from HtmlToPdfConverter constructor if the server was installed on the 
localhost IP address 127.0.0.1 on default port 40001, for example if you installed the EVO PDF Server as a Windows Service on the local development machine.
There are also variants of the constructor accepting an URL instead of IP address if the server was installed as a web service in Azure or in IIS.

```
using EvoPdfClient;
HtmlToPdfConverter htmlToPdfConverter = new HtmlToPdfConverter("server_ip");

// convert URL to a memory buffer
byte[] outPdfBuffer = htmlToPdfConverter.ConvertUrl(url);
	
// convert URL to a PDF file
htmlToPdfConverter.ConvertUrlToFile(url, "result.pdf");

// convert HTML to a memory buffer
byte[] outPdfBuffer = htmlToPdfConverter.ConvertHtml("<b>Hello World</b> from EVO PDF!", null);
	
// convert HTML to a PDF file
htmlToPdfConverter.ConvertUrlToFile(("<b>Hello World</b> from EVO PDF!", null, "result.pdf");
```

## Free Trial

You can download the full EVO PDF Client for .NET package from [EVO PDF Downloads](http://www.evopdf.com/download.aspx) page of the website.
The package contains the product binaries, demo Visual Studio projects with full C# code for ASP.NET Core targeting .NET Core 6.0 and later versions, the library documentation in CHM format.

There are separate demo projects for each major component of the library, including HTML to PDF, Word to PDF, Excel to PDF, PDF to Text, PDF to Image, PDF to HTML and PDF Images Extractor.

You can evaluate the library for free as long as it is needed to ensure that the solution fits your application needs.

## Licensing

The EVO PDF Software licenses are perpetual which means they never expire for a version of the product and include free maintenance for the first year. You can find [more details about licensing](http://www.evopdf.com/buy.aspx) on website.

The same license keys for EVO PDF software works both with regular libraries for .NET Core and with EVO PDF Client for .NET Core. For example, a license key for EVO PDF Toolkit works with all components from client library, while a license for HTML to PDF Converter will work only with this component of the client library.

## Support

For technical and sales questions or for general inquiries about our software and company you can contact us using the email addresses from the [contact page](http://www.evopdf.com/contact.aspx) on the website. 
