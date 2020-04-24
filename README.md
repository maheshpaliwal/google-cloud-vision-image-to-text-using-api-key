# google-cloud-vision-image-to-text-using-api-key
Node js library to extract text from images using google cloud vision api
To install this library 
```

```
### Features of Library
#### Extracting text from external url of an image
```
var glib=require('google-cloud-vision-image-to-text-using-api-key')
var externalUrl="your url"
var gcloudVisionKey="your key"
var lang="en"
glib.textDetectionByUrl(externalUrl,gcloudVisionKey,lang,(err,response)=>{
if(!err){
console.log(response);
}})
```
#### Extracting text from encode bytes of image
```
var glib=require('google-cloud-vision-image-to-text-using-api-key')
var encodedBytes="base64-encoded-image"
var gcloudVisionKey="your key"
var lang="en"
glib.textDetectionByEncodedImage(encodedBytes,gcloudVisionKey,lang,(err,response)=>{
if(!err){
console.log(response);
}})
```
#### extracting text from google cloud storage image
```
var glib=require('google-cloud-vision-image-to-text-using-api-key')
var gStorageUri="uri"
var gcloudVisionKey="your key"
var lang="en"
glib.textDetectionByCloudUri(gStorageUri,gcloudVisionKey,lang,(err,response)=>{
if(!err){
console.log(response);
}})
```
