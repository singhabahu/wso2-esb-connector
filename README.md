## General information for esb-connector-gdrive
- connector name: "esb-connector-gdrive"
- file_id: 1Pv97OssKTABUUcSr-zvjktXU62-mCsm5CNepsz8ABDM
- query: title+%3d+%27MTIT+Test+Doc%27

In the URL's below where `file_id` and `query` are used, use the params given above. I have shared the Google Doc named `MTIT Test Doc` with you, so we can add comments to the same doc.


### Information about user [GET] 
- https://www.googleapis.com/drive/v2/about
- Headers: Authorization,Bearer <access_token>

### Drive file List [GET]   
- https://www.googleapis.com/drive/v2/files
- Headers: Authorization,Bearer <access_token>

### Search for specific file [GET] 
- https://www.googleapis.com/drive/v2/files?q=<query>
- Headers: Authorization,Bearer <access_token>


### Get comments for file [GET] 
- https://www.googleapis.com/drive/v2/files/<file_id>/comments/
- Headers: Authorization,Bearer <access_token>

### Add file comment [POST] 
- https://www.googleapis.com/drive/v2/files/<file_id>/comments/
- Headers: Authorization,Bearer <access_token>
- Request Body: (application/json)
```
{
 	"content": "this is a comment"
}
```

### Delete file comment [DELETE] 
- https://www.googleapis.com/drive/v2/files/<file_id>/comments/<comment_id>
- Headers: Authorization,Bearer <access_token>



