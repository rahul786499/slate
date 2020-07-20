--- 

title: Scholar Onboarding Rest APIs documentation 

language_tabs: 
   - shell 

toc_footers: 
   - <a href='#'>Sign Up for a Developer Key</a> 
   - <a href='https://github.com/lavkumarv'>Documentation Powered by lav</a> 

includes: 
   - errors 

search: true 

--- 

# Introduction 

**Version:** 1.0.0 

# /BATCH/CREATE
## ***POST*** 

**Summary:** createBatch

### HTTP Request 
`***POST*** /batch/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /BATCH/GETALL
## ***GET*** 

**Summary:** getAllBatches

### HTTP Request 
`***GET*** /batch/getAll` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /BATCH/{BATCHID}/DELETE
## ***POST*** 

**Summary:** deleteBatch

### HTTP Request 
`***POST*** /batch/{batchId}/delete` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| batchId | path | batchId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /BATCH/{BATCHID}/UPDATE
## ***POST*** 

**Summary:** updateBatch

### HTTP Request 
`***POST*** /batch/{batchId}/update` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| batchId | path | batchId | Yes | integer |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /COMMENT/{COMMENTID}
## ***DELETE*** 

**Summary:** deleteQueries

### HTTP Request 
`***DELETE*** /comment/{commentId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| commentId | path | commentId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 204 | No Content |
| 401 | Unauthorized |
| 403 | Forbidden |

# /CONNECTIONS
## ***POST*** 

**Summary:** assignBuddy

### HTTP Request 
`***POST*** /connections` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /CONNECTIONS/ADMIN/{USERID}
## ***GET*** 

**Summary:** getAllBuddies

### HTTP Request 
`***GET*** /connections/admin/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /CONNECTIONS/{USERID}
## ***GET*** 

**Summary:** getBuddy

### HTTP Request 
`***GET*** /connections/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /COURSE/DELETE/{COURSEID}
## ***GET*** 

**Summary:** deletecourse

### HTTP Request 
`***GET*** /course/delete/{courseId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| courseId | path | courseId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /COURSE/GETALL
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /course/getAll` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /COURSE/INSERT
## ***POST*** 

**Summary:** insertcourse

### HTTP Request 
`***POST*** /course/insert` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| image | formData | image | Yes | file |
| payload | formData | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /DELETE/{FILEID}
## ***GET*** 

**Summary:** deleteFile

### HTTP Request 
`***GET*** /delete/{fileId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| fileId | path | fileId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /DOWNLOAD/{FILEID}
## ***GET*** 

**Summary:** download

### HTTP Request 
`***GET*** /download/{fileId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| fileId | path | fileId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /ERROR
## ***GET*** 

**Summary:** errorHtml

### HTTP Request 
`***GET*** /error` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

## ***POST*** 

**Summary:** errorHtml

### HTTP Request 
`***POST*** /error` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

## ***PUT*** 

**Summary:** errorHtml

### HTTP Request 
`***PUT*** /error` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

## ***DELETE*** 

**Summary:** errorHtml

### HTTP Request 
`***DELETE*** /error` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 204 | No Content |
| 401 | Unauthorized |
| 403 | Forbidden |

## ***OPTIONS*** 

**Summary:** errorHtml

### HTTP Request 
`***OPTIONS*** /error` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 204 | No Content |
| 401 | Unauthorized |
| 403 | Forbidden |

## ***PATCH*** 

**Summary:** errorHtml

### HTTP Request 
`***PATCH*** /error` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 204 | No Content |
| 401 | Unauthorized |
| 403 | Forbidden |

# /EVENTS/DELETE/{EVENTSID}
## ***GET*** 

**Summary:** deleteevents

### HTTP Request 
`***GET*** /events/delete/{eventsId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| eventsId | path | eventsId | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /EVENTS/GETALL
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /events/getAll` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /EVENTS/INSERT
## ***POST*** 

**Summary:** insertevents

### HTTP Request 
`***POST*** /events/insert` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| image | formData | image | Yes | file |
| payload | formData | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /EVENTS/UPDATE
## ***POST*** 

**Summary:** updateevents

### HTTP Request 
`***POST*** /events/update` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| image | formData | image | No | file |
| payload | formData | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /EVENTS/{EVENTSID}/IMAGE
## ***GET*** 

**Summary:** get

### HTTP Request 
`***GET*** /events/{eventsId}/image` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| eventsId | path | eventsId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /FEEDBACK/GETALL
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /feedback/getAll` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /FEEDBACK/INSERT
## ***POST*** 

**Summary:** insertFeedback

### HTTP Request 
`***POST*** /feedback/insert` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /FORM/ADD
## ***POST*** 

**Summary:** addForm

### HTTP Request 
`***POST*** /form/add` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /FORM/ADDRESPONSE
## ***POST*** 

**Summary:** addResponse

### HTTP Request 
`***POST*** /form/addResponse` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /FORM/DELETE/{FORMID}
## ***GET*** 

**Summary:** deleteForms

### HTTP Request 
`***GET*** /form/delete/{formId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| formId | path | formId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /FORM/GETALL
## ***GET*** 

**Summary:** getAllforms

### HTTP Request 
`***GET*** /form/getAll` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /FORM/TOGGLEACTIVE/{FORMID}
## ***GET*** 

**Summary:** toggleActive

### HTTP Request 
`***GET*** /form/toggleActive/{formId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| formId | path | formId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /FORM/UPDATE
## ***POST*** 

**Summary:** updateForm

### HTTP Request 
`***POST*** /form/update` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /FORM/{FORMID}
## ***GET*** 

**Summary:** getform

### HTTP Request 
`***GET*** /form/{formId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| formId | path | formId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /GETALL/{USERID}
## ***GET*** 

**Summary:** refreshAllModels

### HTTP Request 
`***GET*** /getAll/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /GETALLFILES
## ***GET*** 

**Summary:** getFileList

### HTTP Request 
`***GET*** /getAllFiles` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /ISSUES/GETALL
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /issues/getAll` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /ISSUES/INSERT
## ***POST*** 

**Summary:** insertFeedback

### HTTP Request 
`***POST*** /issues/insert` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /LOGIN/CHANGEPASSWORD
## ***POST*** 

**Summary:** changePassword

### HTTP Request 
`***POST*** /login/changePassword` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /LOGIN/GETBYEMAIL
## ***POST*** 

**Summary:** getByEmail

### HTTP Request 
`***POST*** /login/getByEmail` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /LOGIN/INITIATERESET
## ***POST*** 

**Summary:** resetEmail

### HTTP Request 
`***POST*** /login/initiateReset` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /LOGIN/LOCK/{USERID}
## ***GET*** 

**Summary:** lock

### HTTP Request 
`***GET*** /login/lock/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /LOGIN/LOGIN
## ***POST*** 

**Summary:** login

### HTTP Request 
`***POST*** /login/login` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /LOGIN/PWDRESETTOKENVERIFY
## ***POST*** 

**Summary:** resetTokenVerify

### HTTP Request 
`***POST*** /login/pwdResetTokenVerify` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /LOGIN/RESET
## ***POST*** 

**Summary:** reset

### HTTP Request 
`***POST*** /login/reset` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /LOGIN/UNLOCK/{USERID}
## ***GET*** 

**Summary:** unlock

### HTTP Request 
`***GET*** /login/unlock/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /MAIL/SENT
## ***POST*** 

**Summary:** addForm

### HTTP Request 
`***POST*** /mail/sent` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /NOTIFICATIONS/CLEARALL/{USERID}
## ***GET*** 

**Summary:** clearAll

### HTTP Request 
`***GET*** /notifications/clearAll/{userid}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| userid | path | userid | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /NOTIFICATIONS/DELETE/{NOTIFICATIONSID}
## ***GET*** 

**Summary:** deletenotifications

### HTTP Request 
`***GET*** /notifications/delete/{notificationsId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| notificationsId | path | notificationsId | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /NOTIFICATIONS/GETALL
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /notifications/getAll` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /NOTIFICATIONS/GETALL/{USERID}
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /notifications/getAll/{userid}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| userid | path | userid | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /NOTIFICATIONS/INSERT
## ***POST*** 

**Summary:** insertnotifications

### HTTP Request 
`***POST*** /notifications/insert` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /NOTIFICATIONS/{NOTIFICATIONID}/CLEAR/{USERID}
## ***GET*** 

**Summary:** clear

### HTTP Request 
`***GET*** /notifications/{notificationId}/clear/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| notificationId | path | notificationId | Yes | integer |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/DELETE/{POSTSID}
## ***DELETE*** 

**Summary:** deleteposts

### HTTP Request 
`***DELETE*** /posts/delete/{postsId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| postsId | path | postsId | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 204 | No Content |
| 401 | Unauthorized |
| 403 | Forbidden |

# /POSTS/GETALL
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /posts/getAll` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| pageNo | query | pageNo | No | integer |
| pageSize | query | pageSize | No | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/GETALL/ALLPOSTS
## ***GET*** 

**Summary:** getAllPosts

### HTTP Request 
`***GET*** /posts/getAll/allPosts` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| pageNo | query | pageNo | No | integer |
| pageSize | query | pageSize | No | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/GETALL/NONAPPROVED
## ***GET*** 

**Summary:** getAllUnapproved

### HTTP Request 
`***GET*** /posts/getAll/nonApproved` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| pageNo | query | pageNo | No | integer |
| pageSize | query | pageSize | No | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/INSERT
## ***POST*** 

**Summary:** createPosts

### HTTP Request 
`***POST*** /posts/insert` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| file | formData | file | No | file |
| payload | formData | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/UPDATE
## ***POST*** 

**Summary:** updatePosts

### HTTP Request 
`***POST*** /posts/update` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| file | formData | file | No | file |
| payload | formData | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/{POSTSID}/APPROVE
## ***POST*** 

**Summary:** changePostStatusToAccept

### HTTP Request 
`***POST*** /posts/{postsId}/approve` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| postsId | path | postsId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/{POSTSID}/COMMENT
## ***GET*** 

**Summary:** getComment

### HTTP Request 
`***GET*** /posts/{postsId}/comment` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| pageNo | query | pageNo | No | integer |
| pageSize | query | pageSize | No | integer |
| postsId | path | postsId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

## ***POST*** 

**Summary:** postComment

### HTTP Request 
`***POST*** /posts/{postsId}/comment` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |
| postsId | path | postsId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/{POSTSID}/IMAGE
## ***GET*** 

**Summary:** get

### HTTP Request 
`***GET*** /posts/{postsId}/image` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| postsId | path | postsId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/{POSTSID}/LIKE
## ***GET*** 

**Summary:** postLike

### HTTP Request 
`***GET*** /posts/{postsId}/like` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| postsId | path | postsId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/{POSTSID}/LIKES
## ***GET*** 

**Summary:** getLikesInPagination

### HTTP Request 
`***GET*** /posts/{postsId}/likes` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| pageNo | query | pageNo | No | integer |
| pageSize | query | pageSize | No | integer |
| postsId | path | postsId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /POSTS/{POSTSID}/REJECT
## ***POST*** 

**Summary:** changePostStatusToReject

### HTTP Request 
`***POST*** /posts/{postsId}/reject` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| postsId | path | postsId | Yes | integer |
| reason | query | reason | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /PREREQUISITE/DONE/{USERID}/{PRID}
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /prerequisite/done/{userId}/{prId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| prId | path | prId | Yes | integer |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /PREREQUISITE/GETALL
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /prerequisite/getAll` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /PREREQUISITES/DELETE/{PREREQUISITESID}
## ***GET*** 

**Summary:** deleteprerequisites

### HTTP Request 
`***GET*** /prerequisites/delete/{prerequisitesId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| prerequisitesId | path | prerequisitesId | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /PREREQUISITES/INSERT
## ***POST*** 

**Summary:** insertprerequisites

### HTTP Request 
`***POST*** /prerequisites/insert` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /PREREQUISITES/UPDATE
## ***POST*** 

**Summary:** updateprerequisites

### HTTP Request 
`***POST*** /prerequisites/update` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /QUERIES
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /queries` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

## ***PUT*** 

**Summary:** insertQueries

### HTTP Request 
`***PUT*** /queries` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /QUERIES/{QUERYID}
## ***DELETE*** 

**Summary:** deleteQueries

### HTTP Request 
`***DELETE*** /queries/{queryId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| queryId | path | queryId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 204 | No Content |
| 401 | Unauthorized |
| 403 | Forbidden |

# /QUERIES/{QUERYID}/CHANGESTATUS
## ***POST*** 

**Summary:** changeStatus

### HTTP Request 
`***POST*** /queries/{queryId}/changeStatus` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| payload | body | payload | Yes |  |
| queryId | path | queryId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /QUERIES/{QUERYID}/REPLY
## ***GET*** 

**Summary:** getReplies

### HTTP Request 
`***GET*** /queries/{queryId}/reply` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| queryId | path | queryId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

## ***PUT*** 

**Summary:** addReply

### HTTP Request 
`***PUT*** /queries/{queryId}/reply` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| payload | body | payload | Yes |  |
| queryId | path | queryId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /QUERIES/{QUERYID}/REPLY/{REPLYID}
## ***DELETE*** 

**Summary:** deleteReply

### HTTP Request 
`***DELETE*** /queries/{queryId}/reply/{replyId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| queryId | path | queryId | Yes | integer |
| replyId | path | replyId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 204 | No Content |
| 401 | Unauthorized |
| 403 | Forbidden |

# /QUERIES/{USERID}
## ***GET*** 

**Summary:** getQueriesByUserId

### HTTP Request 
`***GET*** /queries/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /THREAD/ADDMESSAGE
## ***POST*** 

**Summary:** addMessage

### HTTP Request 
`***POST*** /thread/addMessage` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /THREAD/CREATETHREAD
## ***POST*** 

**Summary:** createThread

### HTTP Request 
`***POST*** /thread/createThread` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /THREAD/GETTHREAD/{USERID}
## ***GET*** 

**Summary:** getThread

### HTTP Request 
`***GET*** /thread/getThread/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /THREAD/{THREADID}
## ***DELETE*** 

**Summary:** deleteposts

### HTTP Request 
`***DELETE*** /thread/{threadId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| threadId | path | threadId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 204 | No Content |
| 401 | Unauthorized |
| 403 | Forbidden |

# /THREAD/{THREADID}/MESSAGES
## ***GET*** 

**Summary:** getMessages

### HTTP Request 
`***GET*** /thread/{threadId}/messages` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| page | query | page | Yes | string |
| threadId | path | threadId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /TRACKINFO/GETALL
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /trackinfo/getAll` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /UPLOAD
## ***POST*** 

**Summary:** insertImage

### HTTP Request 
`***POST*** /upload` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| file | formData | file | Yes | file |
| fileDesc | formData | fileDesc | Yes |  |
| userId | formData | userId | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERCOURSE/ADD
## ***POST*** 

**Summary:** insertusercourse

### HTTP Request 
`***POST*** /usercourse/add` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERCOURSE/PROGRESS
## ***POST*** 

**Summary:** updateProgress

### HTTP Request 
`***POST*** /usercourse/progress` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERCOURSE/REMOVE/{USERCOURSEID}
## ***GET*** 

**Summary:** deleteusercourse

### HTTP Request 
`***GET*** /usercourse/remove/{usercourseId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| usercourseId | path | usercourseId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERCOURSE/{USERID}
## ***GET*** 

**Summary:** getusercourse

### HTTP Request 
`***GET*** /usercourse/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/DELETE/{USERINFOID}
## ***GET*** 

**Summary:** deleteuserinfo

### HTTP Request 
`***GET*** /userinfo/delete/{userinfoId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| userinfoId | path | userinfoId | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/DOWNLOADDATA/{USERID}
## ***GET*** 

**Summary:** downloadData

### HTTP Request 
`***GET*** /userinfo/downloadData/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/GET123ALL
## ***GET*** 

**Summary:** get123All

### HTTP Request 
`***GET*** /userinfo/get123All` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/GETALL
## ***GET*** 

**Summary:** getAll

### HTTP Request 
`***GET*** /userinfo/getAll` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/GETCONFIG/{USERID}
## ***GET*** 

**Summary:** getConfig

### HTTP Request 
`***GET*** /userinfo/getConfig/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/GETFULLIMAGE/{USERID}
## ***GET*** 

**Summary:** getFullImage

### HTTP Request 
`***GET*** /userinfo/getFullImage/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/IMAGE
## ***POST*** 

**Summary:** insertImage

### HTTP Request 
`***POST*** /userinfo/image` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| image | formData | image | Yes | file |
| userId | formData | userId | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/INSERT
## ***POST*** 

**Summary:** insertuserinfo

### HTTP Request 
`***POST*** /userinfo/insert` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/SETACTIVEALL
## ***GET*** 

**Summary:** setActiveAll

### HTTP Request 
`***GET*** /userinfo/setActiveAll` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/SETCONFIG/{USERID}
## ***POST*** 

**Summary:** setConfig

### HTTP Request 
`***POST*** /userinfo/setConfig/{userId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/STATUS
## ***POST*** 

**Summary:** updateStatus

### HTTP Request 
`***POST*** /userinfo/status` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/UNDELETE/{USERINFOID}
## ***GET*** 

**Summary:** undeleteuserinfo

### HTTP Request 
`***GET*** /userinfo/undelete/{userinfoId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| userinfoId | path | userinfoId | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/UPDATE
## ***POST*** 

**Summary:** updateuserinfo

### HTTP Request 
`***POST*** /userinfo/update` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization | Yes | string |
| payload | body | payload | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 201 | Created |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

# /USERINFO/{USERID}/GDPR
## ***PATCH*** 

**Summary:** Gdpr

### HTTP Request 
`***PATCH*** /userinfo/{userId}/gdpr` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| payload | body | payload | Yes |  |
| userId | path | userId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 204 | No Content |
| 401 | Unauthorized |
| 403 | Forbidden |

# /USERINFO/{USERINFOID}
## ***GET*** 

**Summary:** getuserinfo

### HTTP Request 
`***GET*** /userinfo/{userinfoId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| userinfoId | path | userinfoId | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | OK |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
