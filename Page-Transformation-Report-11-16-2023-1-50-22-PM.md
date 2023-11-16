# Modernization Summary Report

Date  |  Duration  |  Source Page  |  Target Page Url  |  Status
-------------  |  -------------  |  -------------  |  -------------  |  -------------
11/16/2023 1:50:22 PM  |  00:00:06  |  [/SitePages/BE - Speaker Interest.aspx](https://contoso.sharepoint.com/teams/DWT-Operations-COE/SitePages/BE%20-%20Speaker%20Interest.aspx)  |  []()  |  A issue prevented successful transformation
## Critical Errors during transformation

### 11/16/2023 1:50:28 PM - [/SitePages/BE - Speaker Interest.aspx](https://contoso.sharepoint.com/teams/DWT-Operations-COE/SitePages/BE - Speaker Interest.aspx)

_'t' is invalid after a value. Expected either ',', '}', or ']'. Path: $ | LineNumber: 0 | BytePositionInLine: 84.   at System.Text.Json.ThrowHelper.ReThrowWithPath(ReadStack& state, JsonReaderException ex)
   at System.Text.Json.Serialization.JsonConverter`1.ReadCore(Utf8JsonReader& reader, JsonSerializerOptions options, ReadStack& state)
   at System.Text.Json.JsonSerializer.ReadFromSpan[TValue](ReadOnlySpan`1 utf8Json, JsonTypeInfo jsonTypeInfo, Nullable`1 actualByteCount)
   at System.Text.Json.JsonSerializer.ReadFromSpan[TValue](ReadOnlySpan`1 json, JsonTypeInfo jsonTypeInfo)
   at System.Text.Json.JsonSerializer.Deserialize[TValue](String json, JsonSerializerOptions options)
   at PnP.Core.Model.SharePoint.PageWebPart.set_PropertiesJson(String value)
   at PnP.Framework.Modernization.Transform.ContentTransformator.Transform(List`1 webParts)
   at PnP.Framework.Modernization.Transform.PageTransformator.Transform(PageTransformationInformation pageTransformationInformation)_ 

# Individual Page details
## Transformation Details: /SitePages/BE - Speaker Interest.aspx

- Report date: 11/16/2023 1:50:22 PM
- Transform duration: 00:00:06
- Mode:  Wiki Page Transformation
- Transforming from site: https://contoso.sharepoint.com/teams/DWT-Operations-COE
- Transforming page: /teams/DWT-Operations-COE/SitePages/BE - Speaker Interest.aspx
- Source SharePoint version:  Online (16.0.0.24301)
-  A critical error occurred - transformation did not complete

### Page Transformation Settings

Property  |  Setting
-------------  |  -------------
Engine version   |   1.13.1.0
Target Page Takes Source Page Name   |   True
Target Page Prefix   |   Migrated_
Source Page Prefix   |   Previous_
Copy Page Metadata   |   False
Set Author In Page Header   |   False
Replace Home Page With Default Home Page   |   False
Overwrite   |   True
Target Page Name   |   
Target Page Folder   |   
Target Page Folder Overrides Default Folder   |   False
Keep Page Specific Permissions   |   True
Remove Empty Sections And Columns   |   True
Handle Wiki Images And Videos   |   True
Add Table List Image As Image Web Part   |   True
Keep Page Creation Modification Information   |   True
Publish Created Page   |   True
Post As News   |   False
Disable Page Comments   |   False
Skip Url Rewrite   |   False
Skip Default Url Rewrite   |   False
Url Mapping File   |   
Skip Hidden Web Parts   |   False
Term Mapping File   |   
Skip Term Store Mapping   |   False
Skip User Mapping   |   False
User Mapping File   |   
L D A P Connection String   |   
Skip Telemetry   |   False
### Transformation Operation Details

Date  |  Operation  |  Actions Performed
-------------  |  -------------  |  ------------- 
11/16/2023 1:50:22 PM  |  _Input Validation_  |  _Validation checks complete_
11/16/2023 1:50:22 PM  |  _SharePoint Connection_  |  _Loading client context objects_
11/16/2023 1:50:22 PM  |  _Page Creation_  |  _Detect if the page is living inside a folder_
11/16/2023 1:50:22 PM  |  Page Creation  |  Using the supplied prefix
11/16/2023 1:50:22 PM  |  _Page Creation_  |  _Just try to load the page in the fastest possible manner, we only want to see if the page exists or not_
11/16/2023 1:50:24 PM  |  Load  |  Page does not exist in current web
11/16/2023 1:50:24 PM  |  Page Creation  |  Checking Page Exists
11/16/2023 1:50:26 PM  |  Page Creation  |  Modern page created 
11/16/2023 1:50:26 PM  |  _Home page handling_  |  _Check if the transformed page is the web's home page_
11/16/2023 1:50:26 PM  |  Home page handling  |  Welcome page setting does exist, checking if the transform page is a home page
11/16/2023 1:50:26 PM  |  Home page handling  |  The current page is not used as the site home page
11/16/2023 1:50:26 PM  |  Article page handling  |  Transforming source page as Article page
11/16/2023 1:50:26 PM  |  Article page handling  |  Page Header Set to None. Removing the page header
11/16/2023 1:50:26 PM  |  Article page handling  |  Recognized source page as a Wiki Page. - Analyzing web parts and page layouts
11/16/2023 1:50:28 PM  |  Content Transform  |  Source page contains web part `One Trick Pony` of type `Microsoft.SharePoint.WebPartPages.ScriptEditorWebPart`
11/16/2023 1:50:28 PM  |  Content Transform  |  Source page contains web part `Wiki Search` of type `Microsoft.Office.Server.Search.WebControls.SearchBoxScriptWebPart`
11/16/2023 1:50:28 PM  |  Content Transform  |  Source page contains web part `Page Owner` of type `Microsoft.SharePoint.WebPartPages.XsltListViewWebPart`
11/16/2023 1:50:28 PM  |  Article page handling  |  Splitting images and videos from wiki text - as modern text web part does not support embedded images and videos
11/16/2023 1:50:28 PM  |  Set Page Title  |  Setting the modern page title: BE - Speaker Interest
11/16/2023 1:50:28 PM  |  _Article page handling_  |  _Preparing content transformation_
11/16/2023 1:50:28 PM  |  Article page handling  |  Transforming content
11/16/2023 1:50:28 PM  |  Content Transform  |  Transforming web parts
11/16/2023 1:50:28 PM  |  Web Part Mapping  |  Web Part:'Wiki text' of type 'SharePointPnP.Modernization.WikiTextPart' is being transformed
11/16/2023 1:50:28 PM  |  _Web Part Mapping_  |  _Processing selector functions_
11/16/2023 1:50:28 PM  |  _Web Part Mapping_  |  _Combining mapping data_
11/16/2023 1:50:28 PM  |  Adding Web Parts to Target Page  |  Added 'Client Side Text Web Part' to target page
11/16/2023 1:50:28 PM  |  Web Part Mapping  |  Web Part:'Image in wiki text' of type 'SharePointPnP.Modernization.WikiImagePart' is being transformed
11/16/2023 1:50:28 PM  |  _Web Part Mapping_  |  _Processing selector functions_
11/16/2023 1:50:28 PM  |  _Web Part Mapping_  |  _Combining mapping data_
11/16/2023 1:50:28 PM  |  Adding Web Parts to Target Page  |  Using 'Image' modern web part

