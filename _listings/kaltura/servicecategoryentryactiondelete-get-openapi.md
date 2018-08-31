---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Categoryentry Action Delete
  description: Delete CategoryEntry
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/accesscontrol/action/add:
    get:
      summary: Get Service Access Control Action Add
      description: Add new Access Control Profile
      operationId: accessControl.add
      x-api-path-slug: serviceaccesscontrolactionadd-get
      parameters:
      - in: query
        name: accessControl[description]
        description: The description of the Access Control Profile
      - in: query
        name: accessControl[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`True if this Conversion Profile
          is the default'
      - in: query
        name: accessControl[name]
        description: The name of the Access Control Profile
      - in: query
        name: accessControl[restrictions]
      - in: query
        name: accessControl[systemName]
        description: System name of the Access Control Profile
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrol
      - Action
      - Add
  /service/accesscontrol/action/delete:
    get:
      summary: Get Service Access Control Action Delete
      description: Delete Access Control Profile by id
      operationId: accessControl.delete
      x-api-path-slug: serviceaccesscontrolactiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrol
      - Action
      - Delete
  /service/accesscontrol/action/get:
    get:
      summary: Get Service Access Control Action Get
      description: Get Access Control Profile by id
      operationId: accessControl.get
      x-api-path-slug: serviceaccesscontrolactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrol
      - Action
      - Get
  /service/accesscontrol/action/list:
    get:
      summary: Get Service Access Control Action List
      description: List Access Control Profiles by filter and pager
      operationId: accessControl.list
      x-api-path-slug: serviceaccesscontrolactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrol
      - Action
      - List
  /service/accesscontrol/action/update:
    get:
      summary: Get Service Access Control Action Update
      description: Update Access Control Profile by id
      operationId: accessControl.update
      x-api-path-slug: serviceaccesscontrolactionupdate-get
      parameters:
      - in: query
        name: accessControl[description]
        description: The description of the Access Control Profile
      - in: query
        name: accessControl[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`True if this Conversion Profile
          is the default'
      - in: query
        name: accessControl[name]
        description: The name of the Access Control Profile
      - in: query
        name: accessControl[restrictions]
      - in: query
        name: accessControl[systemName]
        description: System name of the Access Control Profile
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrol
      - Action
      - Update
  /service/accesscontrolprofile/action/add:
    get:
      summary: Get Service Access Controlprofile Action Add
      description: Add new access control profile
      operationId: accessControlProfile.add
      x-api-path-slug: serviceaccesscontrolprofileactionadd-get
      parameters:
      - in: query
        name: accessControlProfile[description]
        description: The description of the Access Control Profile
      - in: query
        name: accessControlProfile[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`True if this access control
          profile is the partner default'
      - in: query
        name: accessControlProfile[name]
        description: The name of the Access Control Profile
      - in: query
        name: accessControlProfile[rules]
      - in: query
        name: accessControlProfile[systemName]
        description: System name of the Access Control Profile
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrolprofile
      - Action
      - Add
  /service/accesscontrolprofile/action/delete:
    get:
      summary: Get Service Access Controlprofile Action Delete
      description: Delete access control profile by id
      operationId: accessControlProfile.delete
      x-api-path-slug: serviceaccesscontrolprofileactiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrolprofile
      - Action
      - Delete
  /service/accesscontrolprofile/action/get:
    get:
      summary: Get Service Access Controlprofile Action Get
      description: Get access control profile by id
      operationId: accessControlProfile.get
      x-api-path-slug: serviceaccesscontrolprofileactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrolprofile
      - Action
      - Get
  /service/accesscontrolprofile/action/list:
    get:
      summary: Get Service Access Controlprofile Action List
      description: List access control profiles by filter and pager
      operationId: accessControlProfile.list
      x-api-path-slug: serviceaccesscontrolprofileactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrolprofile
      - Action
      - List
  /service/accesscontrolprofile/action/update:
    get:
      summary: Get Service Access Controlprofile Action Update
      description: Update access control profile by id
      operationId: accessControlProfile.update
      x-api-path-slug: serviceaccesscontrolprofileactionupdate-get
      parameters:
      - in: query
        name: accessControlProfile[description]
        description: The description of the Access Control Profile
      - in: query
        name: accessControlProfile[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`True if this access control
          profile is the partner default'
      - in: query
        name: accessControlProfile[name]
        description: The name of the Access Control Profile
      - in: query
        name: accessControlProfile[rules]
      - in: query
        name: accessControlProfile[systemName]
        description: System name of the Access Control Profile
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Accesscontrolprofile
      - Action
      - Update
  /service/adminuser/action/login:
    get:
      summary: Get Service Adminuser Action Login
      description: Get an admin session using admin email and password (Used for login
        to the KMC application)
      operationId: adminUser.login
      x-api-path-slug: serviceadminuseractionlogin-get
      parameters:
      - in: query
        name: email
      - in: query
        name: No Name
      - in: query
        name: partnerId
      - in: query
        name: password
      responses:
        200:
          description: OK
      tags:
      - Service
      - Adminuser
      - Action
      - Login
  /service/adminuser/action/resetPassword:
    get:
      summary: Get Service Adminuser Action Resetpassword
      description: Reset admin user password and send it to the users email address
      operationId: adminUser.resetPassword
      x-api-path-slug: serviceadminuseractionresetpassword-get
      parameters:
      - in: query
        name: email
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Adminuser
      - Action
      - ResetPassword
  /service/adminuser/action/setInitialPassword:
    get:
      summary: Get Service Adminuser Action Setinitialpassword
      description: Set initial users password
      operationId: adminUser.setInitialPassword
      x-api-path-slug: serviceadminuseractionsetinitialpassword-get
      parameters:
      - in: query
        name: hashKey
      - in: query
        name: newPassword
        description: new password to set
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Adminuser
      - Action
      - SetInitialPassword
  /service/adminuser/action/updatePassword:
    get:
      summary: Get Service Adminuser Action Updatepassword
      description: Update admin user password and email
      operationId: adminUser.updatePassword
      x-api-path-slug: serviceadminuseractionupdatepassword-get
      parameters:
      - in: query
        name: email
      - in: query
        name: newEmail
        description: Optional, provide only when you want to update the email
      - in: query
        name: newPassword
      - in: query
        name: No Name
      - in: query
        name: password
      responses:
        200:
          description: OK
      tags:
      - Service
      - Adminuser
      - Action
      - UpdatePassword
  /service/analytics/action/query:
    get:
      summary: Get Service Analytics Action Query
      description: report query action allows to get a analytics data for specific
        query dimensions, metrics and filters.
      operationId: analytics.query
      x-api-path-slug: serviceanalyticsactionquery-get
      parameters:
      - in: query
        name: filter[dimensions]
        description: Comma separated dimensions list
      - in: query
        name: filter[filters]
      - in: query
        name: filter[from_time]
        description: Query start time (in local time) MM/dd/yyyy HH:mi
      - in: query
        name: filter[metrics]
        description: Comma separated metrics list
      - in: query
        name: filter[orderBy]
        description: Query order by metric/dimension
      - in: query
        name: filter[to_time]
        description: Query end time (in local time) MM/dd/yyyy HH:mi
      - in: query
        name: filter[utcOffset]
        description: Timezone offset from UTC (in minutes)
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Analytics
      - Action
      - Query
  /service/annotation_annotation/action/add:
    get:
      summary: Get Service Annotation Annotation Action Add
      description: Allows you to add an annotation object associated with an entry
      operationId: annotation.add
      x-api-path-slug: serviceannotation-annotationactionadd-get
      parameters:
      - in: query
        name: annotation[adType]
        description: 'Enum Type: `KalturaAdType`'
      - in: query
        name: annotation[answerKey]
      - in: query
        name: annotation[assetId]
      - in: query
        name: annotation[code]
      - in: query
        name: annotation[correctAnswerKeys]
      - in: query
        name: annotation[description]
      - in: query
        name: annotation[duration]
        description: Duration in milliseconds
      - in: query
        name: annotation[endTime]
        description: End time in milliseconds
      - in: query
        name: annotation[entryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[eventType]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: annotation[explanation]
      - in: query
        name: annotation[forceStop]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: annotation[hint]
      - in: query
        name: annotation[isPublic]
        description: 'Enum Type: `KalturaNullableBoolean`Is the annotation public'
      - in: query
        name: annotation[objectType]
      - in: query
        name: annotation[optionalAnswers]
      - in: query
        name: annotation[parentId]
        description: '`insertOnly`'
      - in: query
        name: annotation[partnerData]
      - in: query
        name: annotation[partnerSortValue]
      - in: query
        name: annotation[protocolType]
        description: '`insertOnly`Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: annotation[question]
      - in: query
        name: annotation[quizUserEntryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[searchableOnEntry]
        description: 'Enum Type: `KalturaNullableBoolean`Should the cue point get
          indexed on the entry'
      - in: query
        name: annotation[sourceUrl]
      - in: query
        name: annotation[startTime]
        description: Start time in milliseconds
      - in: query
        name: annotation[subType]
        description: 'Enum Type: `KalturaThumbCuePointSubType`The sub type of the
          ThumbCuePoint'
      - in: query
        name: annotation[systemName]
      - in: query
        name: annotation[tags]
      - in: query
        name: annotation[text]
      - in: query
        name: annotation[thumbOffset]
      - in: query
        name: annotation[title]
      - in: query
        name: annotation[triggeredAt]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Add
  /service/annotation_annotation/action/addFromBulk:
    post:
      summary: Post Service Annotation Annotation Action Addfrombulk
      description: Allows you to add multiple cue points objects by uploading XML
        that contains multiple cue point definitions
      operationId: annotation.addFromBulk
      x-api-path-slug: serviceannotation-annotationactionaddfrombulk-post
      parameters:
      - in: formData
        name: fileData
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - AddFromBulk
  /service/annotation_annotation/action/clone:
    get:
      summary: Get Service Annotation Annotation Action Clone
      description: Clone cuePoint with id to given entry
      operationId: annotation.clone
      x-api-path-slug: serviceannotation-annotationactionclone-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Clone
  /service/annotation_annotation/action/count:
    get:
      summary: Get Service Annotation Annotation Action Count
      description: count cue point objects by filter
      operationId: annotation.count
      x-api-path-slug: serviceannotation-annotationactioncount-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[codeEqual]
      - in: query
        name: filter[codeIn]
      - in: query
        name: filter[codeLike]
      - in: query
        name: filter[codeMultiLikeAnd]
      - in: query
        name: filter[codeMultiLikeOr]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[cuePointTypeEqual]
        description: 'Enum Type: `KalturaCuePointType`'
      - in: query
        name: filter[cuePointTypeIn]
      - in: query
        name: filter[descriptionLike]
      - in: query
        name: filter[descriptionMultiLikeAnd]
      - in: query
        name: filter[descriptionMultiLikeOr]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[endTimeGreaterThanOrEqual]
      - in: query
        name: filter[endTimeLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[eventTypeEqual]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: filter[eventTypeIn]
      - in: query
        name: filter[forceStopEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[isPublicEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentIdEqual]
      - in: query
        name: filter[parentIdIn]
      - in: query
        name: filter[partnerSortValueEqual]
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueIn]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[protocolTypeEqual]
        description: 'Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: filter[protocolTypeIn]
      - in: query
        name: filter[questionLike]
      - in: query
        name: filter[questionMultiLikeAnd]
      - in: query
        name: filter[questionMultiLikeOr]
      - in: query
        name: filter[quizUserEntryIdEqual]
      - in: query
        name: filter[quizUserEntryIdIn]
      - in: query
        name: filter[startTimeGreaterThanOrEqual]
      - in: query
        name: filter[startTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaCuePointStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[subTypeEqual]
        description: 'Enum Type: `KalturaThumbCuePointSubType`'
      - in: query
        name: filter[subTypeIn]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[textLike]
      - in: query
        name: filter[textMultiLikeAnd]
      - in: query
        name: filter[textMultiLikeOr]
      - in: query
        name: filter[titleLike]
      - in: query
        name: filter[titleMultiLikeAnd]
      - in: query
        name: filter[titleMultiLikeOr]
      - in: query
        name: filter[triggeredAtGreaterThanOrEqual]
      - in: query
        name: filter[triggeredAtLessThanOrEqual]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqualCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqual]
      - in: query
        name: filter[userIdIn]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Count
  /service/annotation_annotation/action/delete:
    get:
      summary: Get Service Annotation Annotation Action Delete
      description: delete cue point by id, and delete all children cue points
      operationId: annotation.delete
      x-api-path-slug: serviceannotation-annotationactiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Delete
  /service/annotation_annotation/action/get:
    get:
      summary: Get Service Annotation Annotation Action Get
      description: Retrieve an CuePoint object by id
      operationId: annotation.get
      x-api-path-slug: serviceannotation-annotationactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Get
  /service/annotation_annotation/action/list:
    get:
      summary: Get Service Annotation Annotation Action List
      description: List annotation objects by filter and pager
      operationId: annotation.list
      x-api-path-slug: serviceannotation-annotationactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[codeEqual]
      - in: query
        name: filter[codeIn]
      - in: query
        name: filter[codeLike]
      - in: query
        name: filter[codeMultiLikeAnd]
      - in: query
        name: filter[codeMultiLikeOr]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[cuePointTypeEqual]
        description: 'Enum Type: `KalturaCuePointType`'
      - in: query
        name: filter[cuePointTypeIn]
      - in: query
        name: filter[descriptionLike]
      - in: query
        name: filter[descriptionMultiLikeAnd]
      - in: query
        name: filter[descriptionMultiLikeOr]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[endTimeGreaterThanOrEqual]
      - in: query
        name: filter[endTimeLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[eventTypeEqual]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: filter[eventTypeIn]
      - in: query
        name: filter[forceStopEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[isPublicEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentIdEqual]
      - in: query
        name: filter[parentIdIn]
      - in: query
        name: filter[partnerSortValueEqual]
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueIn]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[protocolTypeEqual]
        description: 'Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: filter[protocolTypeIn]
      - in: query
        name: filter[questionLike]
      - in: query
        name: filter[questionMultiLikeAnd]
      - in: query
        name: filter[questionMultiLikeOr]
      - in: query
        name: filter[quizUserEntryIdEqual]
      - in: query
        name: filter[quizUserEntryIdIn]
      - in: query
        name: filter[startTimeGreaterThanOrEqual]
      - in: query
        name: filter[startTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaCuePointStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[subTypeEqual]
        description: 'Enum Type: `KalturaThumbCuePointSubType`'
      - in: query
        name: filter[subTypeIn]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[textLike]
      - in: query
        name: filter[textMultiLikeAnd]
      - in: query
        name: filter[textMultiLikeOr]
      - in: query
        name: filter[titleLike]
      - in: query
        name: filter[titleMultiLikeAnd]
      - in: query
        name: filter[titleMultiLikeOr]
      - in: query
        name: filter[triggeredAtGreaterThanOrEqual]
      - in: query
        name: filter[triggeredAtLessThanOrEqual]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqualCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqual]
      - in: query
        name: filter[userIdIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - List
  /service/annotation_annotation/action/serveBulk:
    get:
      summary: Get Service Annotation Annotation Action Servebulk
      description: Download multiple cue points objects as XML definitions
      operationId: annotation.serveBulk
      x-api-path-slug: serviceannotation-annotationactionservebulk-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[codeEqual]
      - in: query
        name: filter[codeIn]
      - in: query
        name: filter[codeLike]
      - in: query
        name: filter[codeMultiLikeAnd]
      - in: query
        name: filter[codeMultiLikeOr]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[cuePointTypeEqual]
        description: 'Enum Type: `KalturaCuePointType`'
      - in: query
        name: filter[cuePointTypeIn]
      - in: query
        name: filter[descriptionLike]
      - in: query
        name: filter[descriptionMultiLikeAnd]
      - in: query
        name: filter[descriptionMultiLikeOr]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[endTimeGreaterThanOrEqual]
      - in: query
        name: filter[endTimeLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[eventTypeEqual]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: filter[eventTypeIn]
      - in: query
        name: filter[forceStopEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[isPublicEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentIdEqual]
      - in: query
        name: filter[parentIdIn]
      - in: query
        name: filter[partnerSortValueEqual]
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueIn]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[protocolTypeEqual]
        description: 'Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: filter[protocolTypeIn]
      - in: query
        name: filter[questionLike]
      - in: query
        name: filter[questionMultiLikeAnd]
      - in: query
        name: filter[questionMultiLikeOr]
      - in: query
        name: filter[quizUserEntryIdEqual]
      - in: query
        name: filter[quizUserEntryIdIn]
      - in: query
        name: filter[startTimeGreaterThanOrEqual]
      - in: query
        name: filter[startTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaCuePointStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[subTypeEqual]
        description: 'Enum Type: `KalturaThumbCuePointSubType`'
      - in: query
        name: filter[subTypeIn]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[textLike]
      - in: query
        name: filter[textMultiLikeAnd]
      - in: query
        name: filter[textMultiLikeOr]
      - in: query
        name: filter[titleLike]
      - in: query
        name: filter[titleMultiLikeAnd]
      - in: query
        name: filter[titleMultiLikeOr]
      - in: query
        name: filter[triggeredAtGreaterThanOrEqual]
      - in: query
        name: filter[triggeredAtLessThanOrEqual]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqualCurrent]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[userIdEqual]
      - in: query
        name: filter[userIdIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - ServeBulk
  /service/annotation_annotation/action/update:
    get:
      summary: Get Service Annotation Annotation Action Update
      description: Update annotation by id
      operationId: annotation.update
      x-api-path-slug: serviceannotation-annotationactionupdate-get
      parameters:
      - in: query
        name: annotation[adType]
        description: 'Enum Type: `KalturaAdType`'
      - in: query
        name: annotation[answerKey]
      - in: query
        name: annotation[assetId]
      - in: query
        name: annotation[code]
      - in: query
        name: annotation[correctAnswerKeys]
      - in: query
        name: annotation[description]
      - in: query
        name: annotation[duration]
        description: Duration in milliseconds
      - in: query
        name: annotation[endTime]
        description: End time in milliseconds
      - in: query
        name: annotation[entryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[eventType]
        description: 'Enum Type: `KalturaEventType`'
      - in: query
        name: annotation[explanation]
      - in: query
        name: annotation[forceStop]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: annotation[hint]
      - in: query
        name: annotation[isPublic]
        description: 'Enum Type: `KalturaNullableBoolean`Is the annotation public'
      - in: query
        name: annotation[objectType]
      - in: query
        name: annotation[optionalAnswers]
      - in: query
        name: annotation[parentId]
        description: '`insertOnly`'
      - in: query
        name: annotation[partnerData]
      - in: query
        name: annotation[partnerSortValue]
      - in: query
        name: annotation[protocolType]
        description: '`insertOnly`Enum Type: `KalturaAdProtocolType`'
      - in: query
        name: annotation[question]
      - in: query
        name: annotation[quizUserEntryId]
        description: '`insertOnly`'
      - in: query
        name: annotation[searchableOnEntry]
        description: 'Enum Type: `KalturaNullableBoolean`Should the cue point get
          indexed on the entry'
      - in: query
        name: annotation[sourceUrl]
      - in: query
        name: annotation[startTime]
        description: Start time in milliseconds
      - in: query
        name: annotation[subType]
        description: 'Enum Type: `KalturaThumbCuePointSubType`The sub type of the
          ThumbCuePoint'
      - in: query
        name: annotation[systemName]
      - in: query
        name: annotation[tags]
      - in: query
        name: annotation[text]
      - in: query
        name: annotation[thumbOffset]
      - in: query
        name: annotation[title]
      - in: query
        name: annotation[triggeredAt]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - Update
  /service/annotation_annotation/action/updateStatus:
    get:
      summary: Get Service Annotation Annotation Action Updatestatus
      description: Update cuePoint status by id
      operationId: annotation.updateStatus
      x-api-path-slug: serviceannotation-annotationactionupdatestatus-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: status
        description: 'Enum Type: `KalturaCuePointStatus`'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Annotation
      - Annotation
      - Action
      - UpdateStatus
  /service/apptoken/action/add:
    get:
      summary: Get Service Apptoken Action Add
      description: Add new application authentication token
      operationId: appToken.add
      x-api-path-slug: serviceapptokenactionadd-get
      parameters:
      - in: query
        name: appToken[expiry]
        description: Expiry time of current token (unix timestamp in seconds)
      - in: query
        name: appToken[hashType]
        description: 'Enum Type: `KalturaAppTokenHashType`'
      - in: query
        name: appToken[sessionDuration]
        description: Expiry duration of KS (Kaltura Session) that created using the
          current token (in seconds)
      - in: query
        name: appToken[sessionPrivileges]
        description: Comma separated privileges to be applied on KS (Kaltura Session)
          that created using the current token
      - in: query
        name: appToken[sessionType]
        description: 'Enum Type: `KalturaSessionType`Type of KS (Kaltura Session)
          that created using the current token'
      - in: query
        name: appToken[sessionUserId]
        description: User id of KS (Kaltura Session) that created using the current
          token
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Apptoken
      - Action
      - Add
  /service/apptoken/action/delete:
    get:
      summary: Get Service Apptoken Action Delete
      description: Delete application authentication token by id
      operationId: appToken.delete
      x-api-path-slug: serviceapptokenactiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Apptoken
      - Action
      - Delete
  /service/apptoken/action/get:
    get:
      summary: Get Service Apptoken Action Get
      description: Get application authentication token by id
      operationId: appToken.get
      x-api-path-slug: serviceapptokenactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Apptoken
      - Action
      - Get
  /service/apptoken/action/list:
    get:
      summary: Get Service Apptoken Action List
      description: List application authentication tokens by filter and pager
      operationId: appToken.list
      x-api-path-slug: serviceapptokenactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaAppTokenStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Apptoken
      - Action
      - List
  /service/apptoken/action/startSession:
    get:
      summary: Get Service Apptoken Action Startsession
      description: Starts a new KS (kaltura Session) based on application authentication
        token id
      operationId: appToken.startSession
      x-api-path-slug: serviceapptokenactionstartsession-get
      parameters:
      - in: query
        name: expiry
        description: session expiry (in seconds), could be overwritten by shorter
          expiry of the application token and the session-expiry that defined on the
          application token
      - in: query
        name: id
        description: application token id
      - in: query
        name: No Name
      - in: query
        name: tokenHash
        description: hashed token, built of sha1 on current KS concatenated with the
          application token
      - in: query
        name: type
        description: 'Enum Type: `KalturaSessionType`session type, will be ignored
          if a different session type already defined on the application token'
      - in: query
        name: userId
        description: session user id, will be ignored if a different user id already
          defined on the application token
      responses:
        200:
          description: OK
      tags:
      - Service
      - Apptoken
      - Action
      - StartSession
  /service/apptoken/action/update:
    get:
      summary: Get Service Apptoken Action Update
      description: Update application authentication token by id
      operationId: appToken.update
      x-api-path-slug: serviceapptokenactionupdate-get
      parameters:
      - in: query
        name: appToken[expiry]
        description: Expiry time of current token (unix timestamp in seconds)
      - in: query
        name: appToken[hashType]
        description: 'Enum Type: `KalturaAppTokenHashType`'
      - in: query
        name: appToken[sessionDuration]
        description: Expiry duration of KS (Kaltura Session) that created using the
          current token (in seconds)
      - in: query
        name: appToken[sessionPrivileges]
        description: Comma separated privileges to be applied on KS (Kaltura Session)
          that created using the current token
      - in: query
        name: appToken[sessionType]
        description: 'Enum Type: `KalturaSessionType`Type of KS (Kaltura Session)
          that created using the current token'
      - in: query
        name: appToken[sessionUserId]
        description: User id of KS (Kaltura Session) that created using the current
          token
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Apptoken
      - Action
      - Update
  /service/aspera_aspera/action/getFaspUrl:
    get:
      summary: Get Service Aspera Aspera Action Getfaspurl
      description: ""
      operationId: aspera.getFaspUrl
      x-api-path-slug: serviceaspera-asperaactiongetfaspurl-get
      parameters:
      - in: query
        name: flavorAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Aspera
      - Aspera
      - Action
      - GetFaspUrl
  /service/attachment_attachmentasset/action/add:
    get:
      summary: Get Service Attachment Attachmentasset Action Add
      description: Add attachment asset
      operationId: attachmentAsset.add
      x-api-path-slug: serviceattachment-attachmentassetactionadd-get
      parameters:
      - in: query
        name: attachmentAsset[accuracy]
        description: The accuracy of the transcript - values between 0 and 1
      - in: query
        name: attachmentAsset[actualSourceAssetParamsIds]
        description: Comma separated list of source flavor params ids
      - in: query
        name: attachmentAsset[fileExt]
        description: '`insertOnly`The file extension'
      - in: query
        name: attachmentAsset[filename]
        description: The filename of the attachment asset content
      - in: query
        name: attachmentAsset[format]
        description: 'Enum Type: `KalturaAttachmentType`The attachment format'
      - in: query
        name: attachmentAsset[humanVerified]
        description: 'Enum Type: `KalturaNullableBoolean`Was verified by human or
          machine'
      - in: query
        name: attachmentAsset[language]
        description: 'Enum Type: `KalturaLanguage`The language of the transcript'
      - in: query
        name: attachmentAsset[objectType]
      - in: query
        name: attachmentAsset[partnerData]
        description: Partner private data
      - in: query
        name: attachmentAsset[partnerDescription]
        description: Partner friendly description
      - in: query
        name: attachmentAsset[providerType]
        description: 'Enum Type: `KalturaTranscriptProviderType`The provider of the
          transcript'
      - in: query
        name: attachmentAsset[tags]
        description: Tags used to identify the Flavor Asset in various scenarios
      - in: query
        name: attachmentAsset[title]
        description: Attachment asset title
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Add
  /service/attachment_attachmentasset/action/delete:
    get:
      summary: Get Service Attachment Attachmentasset Action Delete
      description: ""
      operationId: attachmentAsset.delete
      x-api-path-slug: serviceattachment-attachmentassetactiondelete-get
      parameters:
      - in: query
        name: attachmentAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Delete
  /service/attachment_attachmentasset/action/get:
    get:
      summary: Get Service Attachment Attachmentasset Action Get
      description: ""
      operationId: attachmentAsset.get
      x-api-path-slug: serviceattachment-attachmentassetactionget-get
      parameters:
      - in: query
        name: attachmentAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Get
  /service/attachment_attachmentasset/action/getRemotePaths:
    get:
      summary: Get Service Attachment Attachmentasset Action Getremotepaths
      description: Get remote storage existing paths for the asset
      operationId: attachmentAsset.getRemotePaths
      x-api-path-slug: serviceattachment-attachmentassetactiongetremotepaths-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - GetRemotePaths
  /service/attachment_attachmentasset/action/getUrl:
    get:
      summary: Get Service Attachment Attachmentasset Action Geturl
      description: Get download URL for the asset
      operationId: attachmentAsset.getUrl
      x-api-path-slug: serviceattachment-attachmentassetactiongeturl-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: storageId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - GetUrl
  /service/attachment_attachmentasset/action/list:
    get:
      summary: Get Service Attachment Attachmentasset Action List
      description: List attachment Assets by filter and pager
      operationId: attachmentAsset.list
      x-api-path-slug: serviceattachment-attachmentassetactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[captionParamsIdEqual]
      - in: query
        name: filter[captionParamsIdIn]
      - in: query
        name: filter[contentLike]
      - in: query
        name: filter[contentMultiLikeAnd]
      - in: query
        name: filter[contentMultiLikeOr]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[deletedAtGreaterThanOrEqual]
      - in: query
        name: filter[deletedAtLessThanOrEqual]
      - in: query
        name: filter[endTimeGreaterThanOrEqual]
      - in: query
        name: filter[endTimeLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[flavorParamsIdEqual]
      - in: query
        name: filter[flavorParamsIdIn]
      - in: query
        name: filter[formatEqual]
        description: 'Enum Type: `KalturaAttachmentType`'
      - in: query
        name: filter[formatIn]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[labelEqual]
      - in: query
        name: filter[labelIn]
      - in: query
        name: filter[languageEqual]
        description: 'Enum Type: `KalturaLanguage`'
      - in: query
        name: filter[languageIn]
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerDescriptionLike]
      - in: query
        name: filter[partnerDescriptionMultiLikeAnd]
      - in: query
        name: filter[partnerDescriptionMultiLikeOr]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[sizeGreaterThanOrEqual]
      - in: query
        name: filter[sizeLessThanOrEqual]
      - in: query
        name: filter[startTimeGreaterThanOrEqual]
      - in: query
        name: filter[startTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaAttachmentAssetStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[statusNotIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[thumbParamsIdEqual]
      - in: query
        name: filter[thumbParamsIdIn]
      - in: query
        name: filter[typeIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - List
  /service/attachment_attachmentasset/action/serve:
    get:
      summary: Get Service Attachment Attachmentasset Action Serve
      description: Serves attachment by its id
      operationId: attachmentAsset.serve
      x-api-path-slug: serviceattachment-attachmentassetactionserve-get
      parameters:
      - in: query
        name: attachmentAssetId
      - in: query
        name: No Name
      - in: query
        name: serveOptions[download]
      - in: query
        name: serveOptions[referrer]
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Serve
  /service/attachment_attachmentasset/action/setContent:
    post:
      summary: Post Service Attachment Attachmentasset Action Setcontent
      description: Update content of attachment asset
      operationId: attachmentAsset.setContent
      x-api-path-slug: serviceattachment-attachmentassetactionsetcontent-post
      parameters:
      - in: query
        name: contentResource[assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[content]
        description: Textual content
      - in: query
        name: contentResource[dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[objectType]
      - in: query
        name: contentResource[privateKey]
        description: SSH private key
      - in: query
        name: contentResource[publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resources]
      - in: query
        name: contentResource[resource][assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[resource][content]
        description: Textual content
      - in: query
        name: contentResource[resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[resource][entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[resource][objectType]
      - in: query
        name: contentResource[resource][privateKey]
        description: SSH private key
      - in: query
        name: contentResource[resource][publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resource][resources]
      - in: query
        name: contentResource[resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[resource][resource][content]
        description: Textual content
      - in: query
        name: contentResource[resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[resource][resource][objectType]
      - in: query
        name: contentResource[resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: contentResource[resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resource][resource][resources]
      - in: query
        name: contentResource[resource][resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[resource][resource][resource][content]
        description: Textual content
      - in: query
        name: contentResource[resource][resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[resource][resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[resource][resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[resource][resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[resource][resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[resource][resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[resource][resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[resource][resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[resource][resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[resource][resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[resource][resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[resource][resource][resource][objectType]
      - in: query
        name: contentResource[resource][resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: contentResource[resource][resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resource][resource][resource][resources]
      - in: query
        name: contentResource[resource][resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[resource][resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: contentResource[resource][resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[resource][resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: contentResource[resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: contentResource[resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: contentResource[resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[resource][token]
        description: Token that returned from upload
      - in: query
        name: contentResource[resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[resource][version]
        description: The version of the file sync object
      - in: query
        name: contentResource[storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[token]
        description: Token that returned from upload
      - in: query
        name: contentResource[url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[version]
        description: The version of the file sync object
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - SetContent
  /service/attachment_attachmentasset/action/update:
    get:
      summary: Get Service Attachment Attachmentasset Action Update
      description: Update attachment asset
      operationId: attachmentAsset.update
      x-api-path-slug: serviceattachment-attachmentassetactionupdate-get
      parameters:
      - in: query
        name: attachmentAsset[accuracy]
        description: The accuracy of the transcript - values between 0 and 1
      - in: query
        name: attachmentAsset[actualSourceAssetParamsIds]
        description: Comma separated list of source flavor params ids
      - in: query
        name: attachmentAsset[fileExt]
        description: '`insertOnly`The file extension'
      - in: query
        name: attachmentAsset[filename]
        description: The filename of the attachment asset content
      - in: query
        name: attachmentAsset[format]
        description: 'Enum Type: `KalturaAttachmentType`The attachment format'
      - in: query
        name: attachmentAsset[humanVerified]
        description: 'Enum Type: `KalturaNullableBoolean`Was verified by human or
          machine'
      - in: query
        name: attachmentAsset[language]
        description: 'Enum Type: `KalturaLanguage`The language of the transcript'
      - in: query
        name: attachmentAsset[objectType]
      - in: query
        name: attachmentAsset[partnerData]
        description: Partner private data
      - in: query
        name: attachmentAsset[partnerDescription]
        description: Partner friendly description
      - in: query
        name: attachmentAsset[providerType]
        description: 'Enum Type: `KalturaTranscriptProviderType`The provider of the
          transcript'
      - in: query
        name: attachmentAsset[tags]
        description: Tags used to identify the Flavor Asset in various scenarios
      - in: query
        name: attachmentAsset[title]
        description: Attachment asset title
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attachment
      - Attachmentasset
      - Action
      - Update
  /service/attuversedistribution_attuverse/action/getFeed:
    get:
      summary: Get Service Attuversedistribution Attuverse Action Getfeed
      description: ""
      operationId: attUverse.getFeed
      x-api-path-slug: serviceattuversedistribution-attuverseactiongetfeed-get
      parameters:
      - in: query
        name: distributionProfileId
      - in: query
        name: hash
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Attuversedistribution
      - Attuverse
      - Action
      - GetFeed
  /service/audit_audittrail/action/add:
    get:
      summary: Get Service Audit Audittrail Action Add
      description: Allows you to add an audit trail object and audit trail content
        associated with Kaltura object
      operationId: auditTrail.add
      x-api-path-slug: serviceaudit-audittrailactionadd-get
      parameters:
      - in: query
        name: auditTrail[action]
        description: 'Enum Type: `KalturaAuditTrailAction`'
      - in: query
        name: auditTrail[auditObjectType]
        description: 'Enum Type: `KalturaAuditTrailObjectType`'
      - in: query
        name: auditTrail[data][changedItems]
      - in: query
        name: auditTrail[data][dc]
      - in: query
        name: auditTrail[data][fileType]
        description: 'Enum Type: `KalturaAuditTrailFileSyncType`'
      - in: query
        name: auditTrail[data][info]
      - in: query
        name: auditTrail[data][objectSubType]
      - in: query
        name: auditTrail[data][objectType]
      - in: query
        name: auditTrail[data][original]
      - in: query
        name: auditTrail[data][version]
      - in: query
        name: auditTrail[entryId]
      - in: query
        name: auditTrail[objectId]
      - in: query
        name: auditTrail[relatedObjectId]
      - in: query
        name: auditTrail[relatedObjectType]
        description: 'Enum Type: `KalturaAuditTrailObjectType`'
      - in: query
        name: auditTrail[userId]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Audit
      - Audittrail
      - Action
      - Add
  /service/audit_audittrail/action/get:
    get:
      summary: Get Service Audit Audittrail Action Get
      description: Retrieve an audit trail object by id
      operationId: auditTrail.get
      x-api-path-slug: serviceaudit-audittrailactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Audit
      - Audittrail
      - Action
      - Get
  /service/audit_audittrail/action/list:
    get:
      summary: Get Service Audit Audittrail Action List
      description: List audit trail objects by filter and pager
      operationId: auditTrail.list
      x-api-path-slug: serviceaudit-audittrailactionlist-get
      parameters:
      - in: query
        name: filter[actionEqual]
        description: 'Enum Type: `KalturaAuditTrailAction`'
      - in: query
        name: filter[actionIn]
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[auditObjectTypeEqual]
        description: 'Enum Type: `KalturaAuditTrailObjectType`'
      - in: query
        name: filter[auditObjectTypeIn]
      - in: query
        name: filter[clientTagEqual]
      - in: query
        name: filter[contextEqual]
        description: 'Enum Type: `KalturaAuditTrailContext`'
      - in: query
        name: filter[contextIn]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[entryPointEqual]
      - in: query
        name: filter[entryPointIn]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[ipAddressEqual]
      - in: query
        name: filter[ipAddressIn]
      - in: query
        name: filter[ksEqual]
      - in: query
        name: filter[masterPartnerIdEqual]
      - in: query
        name: filter[masterPartnerIdIn]
      - in: query
        name: filter[objectIdEqual]
      - in: query
        name: filter[objectIdIn]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parsedAtGreaterThanOrEqual]
      - in: query
        name: filter[parsedAtLessThanOrEqual]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[relatedObjectIdEqual]
      - in: query
        name: filter[relatedObjectIdIn]
      - in: query
        name: filter[relatedObjectTypeEqual]
        description: 'Enum Type: `KalturaAuditTrailObjectType`'
      - in: query
        name: filter[relatedObjectTypeIn]
      - in: query
        name: filter[requestIdEqual]
      - in: query
        name: filter[requestIdIn]
      - in: query
        name: filter[serverNameEqual]
      - in: query
        name: filter[serverNameIn]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaAuditTrailStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[userIdEqual]
      - in: query
        name: filter[userIdIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Audit
      - Audittrail
      - Action
      - List
  /service/avndistribution_avn/action/getFeed:
    get:
      summary: Get Service Avndistribution Avn Action Getfeed
      description: ""
      operationId: avn.getFeed
      x-api-path-slug: serviceavndistribution-avnactiongetfeed-get
      parameters:
      - in: query
        name: distributionProfileId
      - in: query
        name: hash
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Avndistribution
      - Avn
      - Action
      - GetFeed
  /service/baseentry/action/add:
    get:
      summary: Get Service Baseentry Action Add
      description: Generic add entry, should be used when the uploaded entry type
        is not known.
      operationId: baseEntry.add
      x-api-path-slug: servicebaseentryactionadd-get
      parameters:
      - in: query
        name: entry[accessControlId]
        description: The Access Control ID assigned to this entry (null when not set,
          send -1 to remove)
      - in: query
        name: entry[adminTags]
        description: Entry admin tags can be updated only by administrators
      - in: query
        name: entry[bitrates]
      - in: query
        name: entry[categoriesIds]
        description: Comma separated list of ids of categories to which this entry
          belongs
      - in: query
        name: entry[categories]
        description: Comma separated list of full names of categories to which this
          entry belongs
      - in: query
        name: entry[conversionProfileId]
        description: Override the default ingestion profile
      - in: query
        name: entry[conversionQuality]
        description: '`insertOnly`Override the default conversion quality'
      - in: query
        name: entry[creatorId]
        description: '`insertOnly`The ID of the user who created this entry'
      - in: query
        name: entry[creditUrl]
        description: The URL for credits
      - in: query
        name: entry[creditUserName]
        description: The user name used for credits
      - in: query
        name: entry[currentBroadcastStartTime]
        description: The time (unix timestamp in milliseconds) in which the entry
          broadcast started or 0 when the entry is off the air
      - in: query
        name: entry[dataContent]
        description: The data of the entry
      - in: query
        name: entry[description]
        description: Entry description
      - in: query
        name: entry[displayInSearch]
        description: 'Enum Type: `KalturaEntryDisplayInSearchType`should we display
          this entry in search'
      - in: query
        name: entry[documentType]
        description: '`insertOnly`Enum Type: `KalturaDocumentType`The type of the
          document'
      - in: query
        name: entry[dvrStatus]
        description: 'Enum Type: `KalturaDVRStatus`DVR Status Enabled/Disabled'
      - in: query
        name: entry[dvrWindow]
        description: Window of time which the DVR allows for backwards scrubbing (in
          minutes)
      - in: query
        name: entry[editorType]
        description: 'Enum Type: `KalturaEditorType`The editor type used to edit the
          metadata'
      - in: query
        name: entry[encodingIP1]
        description: The broadcast primary ip
      - in: query
        name: entry[encodingIP2]
        description: The broadcast secondary ip
      - in: query
        name: entry[endDate]
        description: Entry scheduling end date (null when not set, send -1 to remove)
      - in: query
        name: entry[entitledUsersEdit]
        description: list of user ids that are entitled to edit the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: entry[entitledUsersPublish]
        description: list of user ids that are entitled to publish the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: entry[externalSourceType]
        description: '`insertOnly`Enum Type: `KalturaExternalMediaSourceType`The source
          type of the external media'
      - in: query
        name: entry[filters]
      - in: query
        name: entry[groupId]
      - in: query
        name: entry[hlsStreamUrl]
        description: HLS URL - URL for live stream playback on mobile device
      - in: query
        name: entry[lastElapsedRecordingTime]
        description: Elapsed recording time (in msec) up to the point where the live
          stream was last stopped (unpublished)
      - in: query
        name: entry[licenseType]
        description: 'Enum Type: `KalturaLicenseType`License type used for this entry'
      - in: query
        name: entry[liveStreamConfigurations]
      - in: query
        name: entry[mediaType]
        description: '`insertOnly`Enum Type: `KalturaMediaType`The media type of the
          entry'
      - in: query
        name: entry[msDuration]
        description: The duration in miliseconds
      - in: query
        name: entry[name]
        description: Entry name (Min 1 chars)
      - in: query
        name: entry[objectType]
      - in: query
        name: entry[offlineMessage]
        description: The message to be presented when the stream is offline
      - in: query
        name: entry[operationAttributes]
      - in: query
        name: entry[parentEntryId]
        description: ID of source root entry, used for defining entires association
      - in: query
        name: entry[partnerData]
        description: Can be used to store various partner related data as a string
      - in: query
        name: entry[partnerSortValue]
        description: Can be used to store various partner related data as a numeric
          value
      - in: query
        name: entry[playlistContent]
        description: Content of the playlist - XML if the playlistType is dynamic
          text if the playlistType is static url if the playlistType is mRss
      - in: query
        name: entry[playlistId]
        description: Playlist id to be played
      - in: query
        name: entry[playlistType]
        description: 'Enum Type: `KalturaPlaylistType`Type of playlist'
      - in: query
        name: entry[primaryBroadcastingUrl]
      - in: query
        name: entry[primaryRtspBroadcastingUrl]
      - in: query
        name: entry[publishConfigurations]
      - in: query
        name: entry[pushPublishEnabled]
        description: 'Enum Type: `KalturaLivePublishStatus`Flag denoting whether entry
          should be published by the media server'
      - in: query
        name: entry[recordedEntryId]
        description: Recorded entry id
      - in: query
        name: entry[recordingOptions][shouldCopyEntitlement]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldCopyScheduling]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldCopyThumbnail]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldMakeHidden]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordStatus]
        description: 'Enum Type: `KalturaRecordStatus`Recording Status Enabled/Disabled'
      - in: query
        name: entry[redirectEntryId]
        description: IF not empty, points to an entry ID the should replace this current
          entrys id
      - in: query
        name: entry[referenceId]
        description: Entry external reference id
      - in: query
        name: entry[repeat]
        description: 'Enum Type: `KalturaNullableBoolean`Indicates that the segments
          should be repeated for ever'
      - in: query
        name: entry[retrieveDataContentByGet]
        description: '`insertOnly`indicator whether to return the object for get action
          with the dataContent field'
      - in: query
        name: entry[searchProviderId]
        description: '`insertOnly`The ID of the media in the importing site'
      - in: query
        name: entry[searchProviderType]
        description: '`insertOnly`Enum Type: `KalturaSearchProviderType`The search
          provider type used to import this entry'
      - in: query
        name: entry[secondaryBroadcastingUrl]
      - in: query
        name: entry[secondaryRtspBroadcastingUrl]
      - in: query
        name: entry[sourceType]
        description: '`insertOnly`Enum Type: `KalturaSourceType`The source type of
          the entry'
      - in: query
        name: entry[startDate]
        description: Entry scheduling start date (null when not set, send -1 to remove)
      - in: query
        name: entry[streamName]
      - in: query
        name: entry[streamPassword]
        description: The broadcast password
      - in: query
        name: entry[streams]
      - in: query
        name: entry[streamUrl]
        description: The stream url
      - in: query
        name: entry[tags]
        description: Entry tags
      - in: query
        name: entry[templateEntryId]
        description: '`insertOnly`Template entry id'
      - in: query
        name: entry[totalResults]
        description: Maximum count of results to be returned in playlist execution
      - in: query
        name: entry[type]
        description: 'Enum Type: `KalturaEntryType`The type of the entry, this is
          auto filled by the derived entry object'
      - in: query
        name: entry[urlManager]
        description: URL Manager to handle the live stream URL (for instance, add
          token)
      - in: query
        name: entry[userId]
        description: The ID of the user who is the owner of this entry
      - in: query
        name: No Name
      - in: query
        name: type
        description: 'Enum Type: `KalturaEntryType`'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Add
  /service/baseentry/action/addContent:
    post:
      summary: Post Service Baseentry Action Addcontent
      description: Attach content resource to entry in status NO_MEDIA
      operationId: baseEntry.addContent
      x-api-path-slug: servicebaseentryactionaddcontent-post
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      - in: query
        name: resource[assetId]
        description: ID of the source asset
      - in: query
        name: resource[content]
        description: Textual content
      - in: query
        name: resource[dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[entryId]
        description: ID of the source entry
      - in: formData
        name: resource[fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[objectType]
      - in: query
        name: resource[privateKey]
        description: SSH private key
      - in: query
        name: resource[publicKey]
        description: SSH public key
      - in: query
        name: resource[resources]
      - in: query
        name: resource[resource][assetId]
        description: ID of the source asset
      - in: query
        name: resource[resource][content]
        description: Textual content
      - in: query
        name: resource[resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[resource][entryId]
        description: ID of the source entry
      - in: formData
        name: resource[resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[resource][objectType]
      - in: query
        name: resource[resource][privateKey]
        description: SSH private key
      - in: query
        name: resource[resource][publicKey]
        description: SSH public key
      - in: query
        name: resource[resource][resources]
      - in: query
        name: resource[resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: resource[resource][resource][content]
        description: Textual content
      - in: query
        name: resource[resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: resource[resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[resource][resource][objectType]
      - in: query
        name: resource[resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: resource[resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: resource[resource][resource][resources]
      - in: query
        name: resource[resource][resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: resource[resource][resource][resource][content]
        description: Textual content
      - in: query
        name: resource[resource][resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[resource][resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: resource[resource][resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[resource][resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[resource][resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[resource][resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[resource][resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[resource][resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[resource][resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[resource][resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[resource][resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[resource][resource][resource][objectType]
      - in: query
        name: resource[resource][resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: resource[resource][resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: resource[resource][resource][resource][resources]
      - in: query
        name: resource[resource][resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[resource][resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: resource[resource][resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[resource][resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: resource[resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: resource[resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: resource[resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[resource][token]
        description: Token that returned from upload
      - in: query
        name: resource[resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[resource][version]
        description: The version of the file sync object
      - in: query
        name: resource[storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[token]
        description: Token that returned from upload
      - in: query
        name: resource[url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[version]
        description: The version of the file sync object
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - AddContent
  /service/baseentry/action/addFromUploadedFile:
    get:
      summary: Get Service Baseentry Action Addfromuploadedfile
      description: Generic add entry using an uploaded file, should be used when the
        uploaded entry type is not known.
      operationId: baseEntry.addFromUploadedFile
      x-api-path-slug: servicebaseentryactionaddfromuploadedfile-get
      parameters:
      - in: query
        name: entry[accessControlId]
        description: The Access Control ID assigned to this entry (null when not set,
          send -1 to remove)
      - in: query
        name: entry[adminTags]
        description: Entry admin tags can be updated only by administrators
      - in: query
        name: entry[bitrates]
      - in: query
        name: entry[categoriesIds]
        description: Comma separated list of ids of categories to which this entry
          belongs
      - in: query
        name: entry[categories]
        description: Comma separated list of full names of categories to which this
          entry belongs
      - in: query
        name: entry[conversionProfileId]
        description: Override the default ingestion profile
      - in: query
        name: entry[conversionQuality]
        description: '`insertOnly`Override the default conversion quality'
      - in: query
        name: entry[creatorId]
        description: '`insertOnly`The ID of the user who created this entry'
      - in: query
        name: entry[creditUrl]
        description: The URL for credits
      - in: query
        name: entry[creditUserName]
        description: The user name used for credits
      - in: query
        name: entry[currentBroadcastStartTime]
        description: The time (unix timestamp in milliseconds) in which the entry
          broadcast started or 0 when the entry is off the air
      - in: query
        name: entry[dataContent]
        description: The data of the entry
      - in: query
        name: entry[description]
        description: Entry description
      - in: query
        name: entry[displayInSearch]
        description: 'Enum Type: `KalturaEntryDisplayInSearchType`should we display
          this entry in search'
      - in: query
        name: entry[documentType]
        description: '`insertOnly`Enum Type: `KalturaDocumentType`The type of the
          document'
      - in: query
        name: entry[dvrStatus]
        description: 'Enum Type: `KalturaDVRStatus`DVR Status Enabled/Disabled'
      - in: query
        name: entry[dvrWindow]
        description: Window of time which the DVR allows for backwards scrubbing (in
          minutes)
      - in: query
        name: entry[editorType]
        description: 'Enum Type: `KalturaEditorType`The editor type used to edit the
          metadata'
      - in: query
        name: entry[encodingIP1]
        description: The broadcast primary ip
      - in: query
        name: entry[encodingIP2]
        description: The broadcast secondary ip
      - in: query
        name: entry[endDate]
        description: Entry scheduling end date (null when not set, send -1 to remove)
      - in: query
        name: entry[entitledUsersEdit]
        description: list of user ids that are entitled to edit the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: entry[entitledUsersPublish]
        description: list of user ids that are entitled to publish the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: entry[externalSourceType]
        description: '`insertOnly`Enum Type: `KalturaExternalMediaSourceType`The source
          type of the external media'
      - in: query
        name: entry[filters]
      - in: query
        name: entry[groupId]
      - in: query
        name: entry[hlsStreamUrl]
        description: HLS URL - URL for live stream playback on mobile device
      - in: query
        name: entry[lastElapsedRecordingTime]
        description: Elapsed recording time (in msec) up to the point where the live
          stream was last stopped (unpublished)
      - in: query
        name: entry[licenseType]
        description: 'Enum Type: `KalturaLicenseType`License type used for this entry'
      - in: query
        name: entry[liveStreamConfigurations]
      - in: query
        name: entry[mediaType]
        description: '`insertOnly`Enum Type: `KalturaMediaType`The media type of the
          entry'
      - in: query
        name: entry[msDuration]
        description: The duration in miliseconds
      - in: query
        name: entry[name]
        description: Entry name (Min 1 chars)
      - in: query
        name: entry[objectType]
      - in: query
        name: entry[offlineMessage]
        description: The message to be presented when the stream is offline
      - in: query
        name: entry[operationAttributes]
      - in: query
        name: entry[parentEntryId]
        description: ID of source root entry, used for defining entires association
      - in: query
        name: entry[partnerData]
        description: Can be used to store various partner related data as a string
      - in: query
        name: entry[partnerSortValue]
        description: Can be used to store various partner related data as a numeric
          value
      - in: query
        name: entry[playlistContent]
        description: Content of the playlist - XML if the playlistType is dynamic
          text if the playlistType is static url if the playlistType is mRss
      - in: query
        name: entry[playlistId]
        description: Playlist id to be played
      - in: query
        name: entry[playlistType]
        description: 'Enum Type: `KalturaPlaylistType`Type of playlist'
      - in: query
        name: entry[primaryBroadcastingUrl]
      - in: query
        name: entry[primaryRtspBroadcastingUrl]
      - in: query
        name: entry[publishConfigurations]
      - in: query
        name: entry[pushPublishEnabled]
        description: 'Enum Type: `KalturaLivePublishStatus`Flag denoting whether entry
          should be published by the media server'
      - in: query
        name: entry[recordedEntryId]
        description: Recorded entry id
      - in: query
        name: entry[recordingOptions][shouldCopyEntitlement]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldCopyScheduling]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldCopyThumbnail]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldMakeHidden]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordStatus]
        description: 'Enum Type: `KalturaRecordStatus`Recording Status Enabled/Disabled'
      - in: query
        name: entry[redirectEntryId]
        description: IF not empty, points to an entry ID the should replace this current
          entrys id
      - in: query
        name: entry[referenceId]
        description: Entry external reference id
      - in: query
        name: entry[repeat]
        description: 'Enum Type: `KalturaNullableBoolean`Indicates that the segments
          should be repeated for ever'
      - in: query
        name: entry[retrieveDataContentByGet]
        description: '`insertOnly`indicator whether to return the object for get action
          with the dataContent field'
      - in: query
        name: entry[searchProviderId]
        description: '`insertOnly`The ID of the media in the importing site'
      - in: query
        name: entry[searchProviderType]
        description: '`insertOnly`Enum Type: `KalturaSearchProviderType`The search
          provider type used to import this entry'
      - in: query
        name: entry[secondaryBroadcastingUrl]
      - in: query
        name: entry[secondaryRtspBroadcastingUrl]
      - in: query
        name: entry[sourceType]
        description: '`insertOnly`Enum Type: `KalturaSourceType`The source type of
          the entry'
      - in: query
        name: entry[startDate]
        description: Entry scheduling start date (null when not set, send -1 to remove)
      - in: query
        name: entry[streamName]
      - in: query
        name: entry[streamPassword]
        description: The broadcast password
      - in: query
        name: entry[streams]
      - in: query
        name: entry[streamUrl]
        description: The stream url
      - in: query
        name: entry[tags]
        description: Entry tags
      - in: query
        name: entry[templateEntryId]
        description: '`insertOnly`Template entry id'
      - in: query
        name: entry[totalResults]
        description: Maximum count of results to be returned in playlist execution
      - in: query
        name: entry[type]
        description: 'Enum Type: `KalturaEntryType`The type of the entry, this is
          auto filled by the derived entry object'
      - in: query
        name: entry[urlManager]
        description: URL Manager to handle the live stream URL (for instance, add
          token)
      - in: query
        name: entry[userId]
        description: The ID of the user who is the owner of this entry
      - in: query
        name: No Name
      - in: query
        name: type
        description: 'Enum Type: `KalturaEntryType`'
      - in: query
        name: uploadTokenId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - AddFromUploadedFile
  /service/baseentry/action/anonymousRank:
    get:
      summary: Get Service Baseentry Action Anonymousrank
      description: Anonymously rank an entry, no validation is done on duplicate rankings.
      operationId: baseEntry.anonymousRank
      x-api-path-slug: servicebaseentryactionanonymousrank-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      - in: query
        name: rank
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - AnonymousRank
  /service/baseentry/action/approve:
    get:
      summary: Get Service Baseentry Action Approve
      description: Approve the entry and mark the pending flags (if any) as moderated
        (this will make the entry playable).
      operationId: baseEntry.approve
      x-api-path-slug: servicebaseentryactionapprove-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Approve
  /service/baseentry/action/clone:
    get:
      summary: Get Service Baseentry Action Clone
      description: Clone an entry with optional attributes to apply to the clone
      operationId: baseEntry.clone
      x-api-path-slug: servicebaseentryactionclone-get
      parameters:
      - in: query
        name: entryId
        description: Id of entry to clone
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Clone
  /service/baseentry/action/count:
    get:
      summary: Get Service Baseentry Action Count
      description: Count base entries by filter.
      operationId: baseEntry.count
      x-api-path-slug: servicebaseentryactioncount-get
      parameters:
      - in: query
        name: filter[accessControlIdEqual]
      - in: query
        name: filter[accessControlIdIn]
      - in: query
        name: filter[adminTagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[adminTagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[adminTagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[assetParamsIdsMatchAnd]
      - in: query
        name: filter[assetParamsIdsMatchOr]
      - in: query
        name: filter[categoriesFullNameIn]
      - in: query
        name: filter[categoriesIdsEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[categoriesIdsMatchAnd]
      - in: query
        name: filter[categoriesIdsMatchOr]
        description: All entries of the categories, excluding their child categories
      - in: query
        name: filter[categoriesIdsNotContains]
      - in: query
        name: filter[categoriesMatchAnd]
      - in: query
        name: filter[categoriesMatchOr]
        description: All entries within these categories or their child categories
      - in: query
        name: filter[categoriesNotContains]
      - in: query
        name: filter[categoryAncestorIdIn]
        description: All entries within this categoy or in child categories
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system after a specific time/date (standard
          timestamp format)
      - in: query
        name: filter[createdAtLessThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system before a specific time/date (standard
          timestamp format)
      - in: query
        name: filter[creatorIdEqual]
      - in: query
        name: filter[documentTypeEqual]
        description: 'Enum Type: `KalturaDocumentType`'
      - in: query
        name: filter[documentTypeIn]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationGreaterThan]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[durationLessThan]
      - in: query
        name: filter[durationTypeMatchOr]
      - in: query
        name: filter[endDateGreaterThanOrEqualOrNull]
      - in: query
        name: filter[endDateGreaterThanOrEqual]
      - in: query
        name: filter[endDateLessThanOrEqualOrNull]
      - in: query
        name: filter[endDateLessThanOrEqual]
      - in: query
        name: filter[entitledUsersEditMatchAnd]
      - in: query
        name: filter[entitledUsersEditMatchOr]
      - in: query
        name: filter[entitledUsersPublishMatchAnd]
      - in: query
        name: filter[entitledUsersPublishMatchOr]
      - in: query
        name: filter[externalSourceTypeEqual]
        description: 'Enum Type: `KalturaExternalMediaSourceType`'
      - in: query
        name: filter[externalSourceTypeIn]
      - in: query
        name: filter[flavorParamsIdsMatchAnd]
      - in: query
        name: filter[flavorParamsIdsMatchOr]
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[groupIdEqual]
      - in: query
        name: filter[hasMediaServerHostname]
      - in: query
        name: filter[idEqual]
        description: This filter should be in use for retrieving only a specific entry
          (identified by its entryId)
      - in: query
        name: filter[idIn]
        description: This filter should be in use for retrieving few specific entries
          (string should include comma separated list of entryId strings)
      - in: query
        name: filter[idNotIn]
      - in: query
        name: filter[isLive]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[isRecordedEntryIdEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[isRoot]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[lastPlayedAtGreaterThanOrEqual]
      - in: query
        name: filter[lastPlayedAtLessThanOrEqual]
      - in: query
        name: filter[limit]
      - in: query
        name: filter[mediaDateGreaterThanOrEqual]
      - in: query
        name: filter[mediaDateLessThanOrEqual]
      - in: query
        name: filter[mediaTypeEqual]
        description: 'Enum Type: `KalturaMediaType`'
      - in: query
        name: filter[mediaTypeIn]
      - in: query
        name: filter[moderationStatusEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: filter[moderationStatusIn]
      - in: query
        name: filter[moderationStatusNotEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: filter[moderationStatusNotIn]
      - in: query
        name: filter[nameEqual]
        description: This filter should be in use for retrieving entries with a specific
          name
      - in: query
        name: filter[nameLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[nameMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[nameMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentEntryIdEqual]
      - in: query
        name: filter[partnerIdEqual]
        description: This filter should be in use for retrieving only entries which
          were uploaded by/assigned to users of a specific Kaltura Partner (identified
          by Partner ID)
      - in: query
        name: filter[partnerIdIn]
        description: This filter should be in use for retrieving only entries within
          Kaltura network which were uploaded by/assigned to users of few Kaltura
          Partners  (string should include comma separated list of PartnerIDs)
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[redirectFromEntryId]
        description: The id of the original entry
      - in: query
        name: filter[referenceIdEqual]
      - in: query
        name: filter[referenceIdIn]
      - in: query
        name: filter[replacedEntryIdEqual]
      - in: query
        name: filter[replacedEntryIdIn]
      - in: query
        name: filter[replacementStatusEqual]
        description: 'Enum Type: `KalturaEntryReplacementStatus`'
      - in: query
        name: filter[replacementStatusIn]
      - in: query
        name: filter[replacingEntryIdEqual]
      - in: query
        name: filter[replacingEntryIdIn]
      - in: query
        name: filter[rootEntryIdEqual]
      - in: query
        name: filter[rootEntryIdIn]
      - in: query
        name: filter[searchTextMatchAnd]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within all of the following metadata
          attributes: name, description, tags, adminTags'
      - in: query
        name: filter[searchTextMatchOr]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within at least one of the following
          metadata attributes: name, description, tags, adminTags'
      - in: query
        name: filter[sourceTypeEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: filter[sourceTypeIn]
      - in: query
        name: filter[sourceTypeNotEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: filter[sourceTypeNotIn]
      - in: query
        name: filter[startDateGreaterThanOrEqualOrNull]
      - in: query
        name: filter[startDateGreaterThanOrEqual]
      - in: query
        name: filter[startDateLessThanOrEqualOrNull]
      - in: query
        name: filter[startDateLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, at a specific {'
      - in: query
        name: filter[statusIn]
        description: This filter should be in use for retrieving only entries, at
          few specific {
      - in: query
        name: filter[statusNotEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, not at a specific {'
      - in: query
        name: filter[statusNotIn]
        description: This filter should be in use for retrieving only entries, not
          at few specific {
      - in: query
        name: filter[tagsAdminTagsMultiLikeAnd]
      - in: query
        name: filter[tagsAdminTagsMultiLikeOr]
      - in: query
        name: filter[tagsAdminTagsNameMultiLikeAnd]
      - in: query
        name: filter[tagsAdminTagsNameMultiLikeOr]
      - in: query
        name: filter[tagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsNameMultiLikeAnd]
      - in: query
        name: filter[tagsNameMultiLikeOr]
      - in: query
        name: filter[totalRankGreaterThanOrEqual]
      - in: query
        name: filter[totalRankLessThanOrEqual]
      - in: query
        name: filter[typeEqual]
        description: 'Enum Type: `KalturaEntryType`'
      - in: query
        name: filter[typeIn]
        description: This filter should be in use for retrieving entries of few {
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdEqual]
        description: This filter parameter should be in use for retrieving only entries,
          uploaded by/assigned to a specific user (identified by user Id)
      - in: query
        name: filter[userIdIn]
      - in: query
        name: filter[userIdNotIn]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Count
  /service/baseentry/action/delete:
    get:
      summary: Get Service Baseentry Action Delete
      description: Delete an entry.
      operationId: baseEntry.delete
      x-api-path-slug: servicebaseentryactiondelete-get
      parameters:
      - in: query
        name: entryId
        description: Entry id to delete
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Delete
  /service/baseentry/action/export:
    get:
      summary: Get Service Baseentry Action Export
      description: ""
      operationId: baseEntry.export
      x-api-path-slug: servicebaseentryactionexport-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      - in: query
        name: storageProfileId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Export
  /service/baseentry/action/flag:
    get:
      summary: Get Service Baseentry Action Flag
      description: Flag inappropriate entry for moderation.
      operationId: baseEntry.flag
      x-api-path-slug: servicebaseentryactionflag-get
      parameters:
      - in: query
        name: moderationFlag[comments]
        description: The comment that was added to the flag
      - in: query
        name: moderationFlag[flaggedEntryId]
        description: If moderation flag is set for entry, this is the flagged entry
          id
      - in: query
        name: moderationFlag[flaggedUserId]
        description: If moderation flag is set for user, this is the flagged user
          id
      - in: query
        name: moderationFlag[flagType]
        description: 'Enum Type: `KalturaModerationFlagType`'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Flag
  /service/baseentry/action/get:
    get:
      summary: Get Service Baseentry Action Get
      description: Get base entry by ID.
      operationId: baseEntry.get
      x-api-path-slug: servicebaseentryactionget-get
      parameters:
      - in: query
        name: entryId
        description: Entry id
      - in: query
        name: No Name
      - in: query
        name: version
        description: Desired version of the data
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Get
  /service/baseentry/action/getByIds:
    get:
      summary: Get Service Baseentry Action Getbyids
      description: Get an array of KalturaBaseEntry objects by a comma-separated list
        of ids.
      operationId: baseEntry.getByIds
      x-api-path-slug: servicebaseentryactiongetbyids-get
      parameters:
      - in: query
        name: entryIds
        description: Comma separated string of entry ids
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - GetByIds
  /service/baseentry/action/getContextData:
    get:
      summary: Get Service Baseentry Action Getcontextdata
      description: 'This action delivers entry-related data, based on the user''s
        context: access control, restriction, playback format and storage information.'
      operationId: baseEntry.getContextData
      x-api-path-slug: servicebaseentryactiongetcontextdata-get
      parameters:
      - in: query
        name: contextDataParams[contexts]
      - in: query
        name: contextDataParams[flavorAssetId]
        description: Id of the current flavor
      - in: query
        name: contextDataParams[flavorTags]
        description: The tags of the flavors that should be used for playback
      - in: query
        name: contextDataParams[hashes]
      - in: query
        name: contextDataParams[ip]
        description: IP to be used to test geographic location conditions
      - in: query
        name: contextDataParams[ks]
        description: Kaltura session to be used to test session and user conditions
      - in: query
        name: contextDataParams[mediaProtocol]
        description: Protocol of the specific media object
      - in: query
        name: contextDataParams[objectType]
      - in: query
        name: contextDataParams[referrer]
        description: URL to be used to test domain conditions
      - in: query
        name: contextDataParams[streamerType]
        description: 'Playback streamer type: RTMP, HTTP, appleHttps, rtsp, sl'
      - in: query
        name: contextDataParams[time]
        description: Unix timestamp (In seconds) to be used to test entry scheduling,
          keep null to use now
      - in: query
        name: contextDataParams[userAgent]
        description: Browser or client application to be used to test agent conditions
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - GetContextData
  /service/baseentry/action/getPlaybackContext:
    get:
      summary: Get Service Baseentry Action Getplaybackcontext
      description: This action delivers all data relevant for player
      operationId: baseEntry.getPlaybackContext
      x-api-path-slug: servicebaseentryactiongetplaybackcontext-get
      parameters:
      - in: query
        name: contextDataParams[contexts]
      - in: query
        name: contextDataParams[flavorAssetId]
        description: Id of the current flavor
      - in: query
        name: contextDataParams[flavorTags]
        description: The tags of the flavors that should be used for playback
      - in: query
        name: contextDataParams[hashes]
      - in: query
        name: contextDataParams[ip]
        description: IP to be used to test geographic location conditions
      - in: query
        name: contextDataParams[ks]
        description: Kaltura session to be used to test session and user conditions
      - in: query
        name: contextDataParams[mediaProtocol]
        description: Protocol of the specific media object
      - in: query
        name: contextDataParams[referrer]
        description: URL to be used to test domain conditions
      - in: query
        name: contextDataParams[streamerType]
        description: 'Playback streamer type: RTMP, HTTP, appleHttps, rtsp, sl'
      - in: query
        name: contextDataParams[time]
        description: Unix timestamp (In seconds) to be used to test entry scheduling,
          keep null to use now
      - in: query
        name: contextDataParams[userAgent]
        description: Browser or client application to be used to test agent conditions
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - GetPlaybackContext
  /service/baseentry/action/getRemotePaths:
    get:
      summary: Get Service Baseentry Action Getremotepaths
      description: Get remote storage existing paths for the asset.
      operationId: baseEntry.getRemotePaths
      x-api-path-slug: servicebaseentryactiongetremotepaths-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - GetRemotePaths
  /service/baseentry/action/index:
    get:
      summary: Get Service Baseentry Action Index
      description: Index an entry by id.
      operationId: baseEntry.index
      x-api-path-slug: servicebaseentryactionindex-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: shouldUpdate
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Index
  /service/baseentry/action/list:
    get:
      summary: Get Service Baseentry Action List
      description: List base entries by filter with paging support.
      operationId: baseEntry.list
      x-api-path-slug: servicebaseentryactionlist-get
      parameters:
      - in: query
        name: filter[accessControlIdEqual]
      - in: query
        name: filter[accessControlIdIn]
      - in: query
        name: filter[adminTagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[adminTagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[adminTagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[assetParamsIdsMatchAnd]
      - in: query
        name: filter[assetParamsIdsMatchOr]
      - in: query
        name: filter[categoriesFullNameIn]
      - in: query
        name: filter[categoriesIdsEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[categoriesIdsMatchAnd]
      - in: query
        name: filter[categoriesIdsMatchOr]
        description: All entries of the categories, excluding their child categories
      - in: query
        name: filter[categoriesIdsNotContains]
      - in: query
        name: filter[categoriesMatchAnd]
      - in: query
        name: filter[categoriesMatchOr]
        description: All entries within these categories or their child categories
      - in: query
        name: filter[categoriesNotContains]
      - in: query
        name: filter[categoryAncestorIdIn]
        description: All entries within this categoy or in child categories
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system after a specific time/date (standard
          timestamp format)
      - in: query
        name: filter[createdAtLessThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system before a specific time/date (standard
          timestamp format)
      - in: query
        name: filter[creatorIdEqual]
      - in: query
        name: filter[documentTypeEqual]
        description: 'Enum Type: `KalturaDocumentType`'
      - in: query
        name: filter[documentTypeIn]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationGreaterThan]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[durationLessThan]
      - in: query
        name: filter[durationTypeMatchOr]
      - in: query
        name: filter[endDateGreaterThanOrEqualOrNull]
      - in: query
        name: filter[endDateGreaterThanOrEqual]
      - in: query
        name: filter[endDateLessThanOrEqualOrNull]
      - in: query
        name: filter[endDateLessThanOrEqual]
      - in: query
        name: filter[entitledUsersEditMatchAnd]
      - in: query
        name: filter[entitledUsersEditMatchOr]
      - in: query
        name: filter[entitledUsersPublishMatchAnd]
      - in: query
        name: filter[entitledUsersPublishMatchOr]
      - in: query
        name: filter[externalSourceTypeEqual]
        description: 'Enum Type: `KalturaExternalMediaSourceType`'
      - in: query
        name: filter[externalSourceTypeIn]
      - in: query
        name: filter[flavorParamsIdsMatchAnd]
      - in: query
        name: filter[flavorParamsIdsMatchOr]
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[groupIdEqual]
      - in: query
        name: filter[hasMediaServerHostname]
      - in: query
        name: filter[idEqual]
        description: This filter should be in use for retrieving only a specific entry
          (identified by its entryId)
      - in: query
        name: filter[idIn]
        description: This filter should be in use for retrieving few specific entries
          (string should include comma separated list of entryId strings)
      - in: query
        name: filter[idNotIn]
      - in: query
        name: filter[isLive]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[isRecordedEntryIdEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[isRoot]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[lastPlayedAtGreaterThanOrEqual]
      - in: query
        name: filter[lastPlayedAtLessThanOrEqual]
      - in: query
        name: filter[limit]
      - in: query
        name: filter[mediaDateGreaterThanOrEqual]
      - in: query
        name: filter[mediaDateLessThanOrEqual]
      - in: query
        name: filter[mediaTypeEqual]
        description: 'Enum Type: `KalturaMediaType`'
      - in: query
        name: filter[mediaTypeIn]
      - in: query
        name: filter[moderationStatusEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: filter[moderationStatusIn]
      - in: query
        name: filter[moderationStatusNotEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: filter[moderationStatusNotIn]
      - in: query
        name: filter[nameEqual]
        description: This filter should be in use for retrieving entries with a specific
          name
      - in: query
        name: filter[nameLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[nameMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[nameMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentEntryIdEqual]
      - in: query
        name: filter[partnerIdEqual]
        description: This filter should be in use for retrieving only entries which
          were uploaded by/assigned to users of a specific Kaltura Partner (identified
          by Partner ID)
      - in: query
        name: filter[partnerIdIn]
        description: This filter should be in use for retrieving only entries within
          Kaltura network which were uploaded by/assigned to users of few Kaltura
          Partners  (string should include comma separated list of PartnerIDs)
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[redirectFromEntryId]
        description: The id of the original entry
      - in: query
        name: filter[referenceIdEqual]
      - in: query
        name: filter[referenceIdIn]
      - in: query
        name: filter[replacedEntryIdEqual]
      - in: query
        name: filter[replacedEntryIdIn]
      - in: query
        name: filter[replacementStatusEqual]
        description: 'Enum Type: `KalturaEntryReplacementStatus`'
      - in: query
        name: filter[replacementStatusIn]
      - in: query
        name: filter[replacingEntryIdEqual]
      - in: query
        name: filter[replacingEntryIdIn]
      - in: query
        name: filter[rootEntryIdEqual]
      - in: query
        name: filter[rootEntryIdIn]
      - in: query
        name: filter[searchTextMatchAnd]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within all of the following metadata
          attributes: name, description, tags, adminTags'
      - in: query
        name: filter[searchTextMatchOr]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within at least one of the following
          metadata attributes: name, description, tags, adminTags'
      - in: query
        name: filter[sourceTypeEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: filter[sourceTypeIn]
      - in: query
        name: filter[sourceTypeNotEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: filter[sourceTypeNotIn]
      - in: query
        name: filter[startDateGreaterThanOrEqualOrNull]
      - in: query
        name: filter[startDateGreaterThanOrEqual]
      - in: query
        name: filter[startDateLessThanOrEqualOrNull]
      - in: query
        name: filter[startDateLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, at a specific {'
      - in: query
        name: filter[statusIn]
        description: This filter should be in use for retrieving only entries, at
          few specific {
      - in: query
        name: filter[statusNotEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, not at a specific {'
      - in: query
        name: filter[statusNotIn]
        description: This filter should be in use for retrieving only entries, not
          at few specific {
      - in: query
        name: filter[tagsAdminTagsMultiLikeAnd]
      - in: query
        name: filter[tagsAdminTagsMultiLikeOr]
      - in: query
        name: filter[tagsAdminTagsNameMultiLikeAnd]
      - in: query
        name: filter[tagsAdminTagsNameMultiLikeOr]
      - in: query
        name: filter[tagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsNameMultiLikeAnd]
      - in: query
        name: filter[tagsNameMultiLikeOr]
      - in: query
        name: filter[totalRankGreaterThanOrEqual]
      - in: query
        name: filter[totalRankLessThanOrEqual]
      - in: query
        name: filter[typeEqual]
        description: 'Enum Type: `KalturaEntryType`'
      - in: query
        name: filter[typeIn]
        description: This filter should be in use for retrieving entries of few {
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdEqual]
        description: This filter parameter should be in use for retrieving only entries,
          uploaded by/assigned to a specific user (identified by user Id)
      - in: query
        name: filter[userIdIn]
      - in: query
        name: filter[userIdNotIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - List
  /service/baseentry/action/listByReferenceId:
    get:
      summary: Get Service Baseentry Action Listbyreferenceid
      description: List base entries by filter according to reference id
      operationId: baseEntry.listByReferenceId
      x-api-path-slug: servicebaseentryactionlistbyreferenceid-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      - in: query
        name: refId
        description: Entry Reference ID
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - ListByReferenceId
  /service/baseentry/action/listFlags:
    get:
      summary: Get Service Baseentry Action Listflags
      description: List all pending flags for the entry.
      operationId: baseEntry.listFlags
      x-api-path-slug: servicebaseentryactionlistflags-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - ListFlags
  /service/baseentry/action/reject:
    get:
      summary: Get Service Baseentry Action Reject
      description: Reject the entry and mark the pending flags (if any) as moderated
        (this will make the entry non-playable).
      operationId: baseEntry.reject
      x-api-path-slug: servicebaseentryactionreject-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Reject
  /service/baseentry/action/update:
    get:
      summary: Get Service Baseentry Action Update
      description: Update base entry. Only the properties that were set will be updated.
      operationId: baseEntry.update
      x-api-path-slug: servicebaseentryactionupdate-get
      parameters:
      - in: query
        name: baseEntry[accessControlId]
        description: The Access Control ID assigned to this entry (null when not set,
          send -1 to remove)
      - in: query
        name: baseEntry[adminTags]
        description: Entry admin tags can be updated only by administrators
      - in: query
        name: baseEntry[bitrates]
      - in: query
        name: baseEntry[categoriesIds]
        description: Comma separated list of ids of categories to which this entry
          belongs
      - in: query
        name: baseEntry[categories]
        description: Comma separated list of full names of categories to which this
          entry belongs
      - in: query
        name: baseEntry[conversionProfileId]
        description: Override the default ingestion profile
      - in: query
        name: baseEntry[conversionQuality]
        description: '`insertOnly`Override the default conversion quality'
      - in: query
        name: baseEntry[creatorId]
        description: '`insertOnly`The ID of the user who created this entry'
      - in: query
        name: baseEntry[creditUrl]
        description: The URL for credits
      - in: query
        name: baseEntry[creditUserName]
        description: The user name used for credits
      - in: query
        name: baseEntry[currentBroadcastStartTime]
        description: The time (unix timestamp in milliseconds) in which the entry
          broadcast started or 0 when the entry is off the air
      - in: query
        name: baseEntry[dataContent]
        description: The data of the entry
      - in: query
        name: baseEntry[description]
        description: Entry description
      - in: query
        name: baseEntry[displayInSearch]
        description: 'Enum Type: `KalturaEntryDisplayInSearchType`should we display
          this entry in search'
      - in: query
        name: baseEntry[documentType]
        description: '`insertOnly`Enum Type: `KalturaDocumentType`The type of the
          document'
      - in: query
        name: baseEntry[dvrStatus]
        description: 'Enum Type: `KalturaDVRStatus`DVR Status Enabled/Disabled'
      - in: query
        name: baseEntry[dvrWindow]
        description: Window of time which the DVR allows for backwards scrubbing (in
          minutes)
      - in: query
        name: baseEntry[editorType]
        description: 'Enum Type: `KalturaEditorType`The editor type used to edit the
          metadata'
      - in: query
        name: baseEntry[encodingIP1]
        description: The broadcast primary ip
      - in: query
        name: baseEntry[encodingIP2]
        description: The broadcast secondary ip
      - in: query
        name: baseEntry[endDate]
        description: Entry scheduling end date (null when not set, send -1 to remove)
      - in: query
        name: baseEntry[entitledUsersEdit]
        description: list of user ids that are entitled to edit the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: baseEntry[entitledUsersPublish]
        description: list of user ids that are entitled to publish the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: baseEntry[externalSourceType]
        description: '`insertOnly`Enum Type: `KalturaExternalMediaSourceType`The source
          type of the external media'
      - in: query
        name: baseEntry[filters]
      - in: query
        name: baseEntry[groupId]
      - in: query
        name: baseEntry[hlsStreamUrl]
        description: HLS URL - URL for live stream playback on mobile device
      - in: query
        name: baseEntry[lastElapsedRecordingTime]
        description: Elapsed recording time (in msec) up to the point where the live
          stream was last stopped (unpublished)
      - in: query
        name: baseEntry[licenseType]
        description: 'Enum Type: `KalturaLicenseType`License type used for this entry'
      - in: query
        name: baseEntry[liveStreamConfigurations]
      - in: query
        name: baseEntry[mediaType]
        description: '`insertOnly`Enum Type: `KalturaMediaType`The media type of the
          entry'
      - in: query
        name: baseEntry[msDuration]
        description: The duration in miliseconds
      - in: query
        name: baseEntry[name]
        description: Entry name (Min 1 chars)
      - in: query
        name: baseEntry[objectType]
      - in: query
        name: baseEntry[offlineMessage]
        description: The message to be presented when the stream is offline
      - in: query
        name: baseEntry[operationAttributes]
      - in: query
        name: baseEntry[parentEntryId]
        description: ID of source root entry, used for defining entires association
      - in: query
        name: baseEntry[partnerData]
        description: Can be used to store various partner related data as a string
      - in: query
        name: baseEntry[partnerSortValue]
        description: Can be used to store various partner related data as a numeric
          value
      - in: query
        name: baseEntry[playlistContent]
        description: Content of the playlist - XML if the playlistType is dynamic
          text if the playlistType is static url if the playlistType is mRss
      - in: query
        name: baseEntry[playlistId]
        description: Playlist id to be played
      - in: query
        name: baseEntry[playlistType]
        description: 'Enum Type: `KalturaPlaylistType`Type of playlist'
      - in: query
        name: baseEntry[primaryBroadcastingUrl]
      - in: query
        name: baseEntry[primaryRtspBroadcastingUrl]
      - in: query
        name: baseEntry[publishConfigurations]
      - in: query
        name: baseEntry[pushPublishEnabled]
        description: 'Enum Type: `KalturaLivePublishStatus`Flag denoting whether entry
          should be published by the media server'
      - in: query
        name: baseEntry[recordedEntryId]
        description: Recorded entry id
      - in: query
        name: baseEntry[recordingOptions][shouldCopyEntitlement]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: baseEntry[recordingOptions][shouldCopyScheduling]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: baseEntry[recordingOptions][shouldCopyThumbnail]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: baseEntry[recordingOptions][shouldMakeHidden]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: baseEntry[recordStatus]
        description: 'Enum Type: `KalturaRecordStatus`Recording Status Enabled/Disabled'
      - in: query
        name: baseEntry[redirectEntryId]
        description: IF not empty, points to an entry ID the should replace this current
          entrys id
      - in: query
        name: baseEntry[referenceId]
        description: Entry external reference id
      - in: query
        name: baseEntry[repeat]
        description: 'Enum Type: `KalturaNullableBoolean`Indicates that the segments
          should be repeated for ever'
      - in: query
        name: baseEntry[retrieveDataContentByGet]
        description: '`insertOnly`indicator whether to return the object for get action
          with the dataContent field'
      - in: query
        name: baseEntry[searchProviderId]
        description: '`insertOnly`The ID of the media in the importing site'
      - in: query
        name: baseEntry[searchProviderType]
        description: '`insertOnly`Enum Type: `KalturaSearchProviderType`The search
          provider type used to import this entry'
      - in: query
        name: baseEntry[secondaryBroadcastingUrl]
      - in: query
        name: baseEntry[secondaryRtspBroadcastingUrl]
      - in: query
        name: baseEntry[sourceType]
        description: '`insertOnly`Enum Type: `KalturaSourceType`The source type of
          the entry'
      - in: query
        name: baseEntry[startDate]
        description: Entry scheduling start date (null when not set, send -1 to remove)
      - in: query
        name: baseEntry[streamName]
      - in: query
        name: baseEntry[streamPassword]
        description: The broadcast password
      - in: query
        name: baseEntry[streams]
      - in: query
        name: baseEntry[streamUrl]
        description: The stream url
      - in: query
        name: baseEntry[tags]
        description: Entry tags
      - in: query
        name: baseEntry[templateEntryId]
        description: '`insertOnly`Template entry id'
      - in: query
        name: baseEntry[totalResults]
        description: Maximum count of results to be returned in playlist execution
      - in: query
        name: baseEntry[type]
        description: 'Enum Type: `KalturaEntryType`The type of the entry, this is
          auto filled by the derived entry object'
      - in: query
        name: baseEntry[urlManager]
        description: URL Manager to handle the live stream URL (for instance, add
          token)
      - in: query
        name: baseEntry[userId]
        description: The ID of the user who is the owner of this entry
      - in: query
        name: entryId
        description: Entry id to update
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Update
  /service/baseentry/action/updateContent:
    post:
      summary: Post Service Baseentry Action Updatecontent
      description: Update the content resource associated with the entry.
      operationId: baseEntry.updateContent
      x-api-path-slug: servicebaseentryactionupdatecontent-post
      parameters:
      - in: query
        name: advancedOptions[keepManualThumbnails]
        description: If true manually created thumbnails will not be deleted on entry
          replacement
      - in: query
        name: advancedOptions[pluginOptionItems]
      - in: query
        name: conversionProfileId
        description: The conversion profile id to be used on the entry
      - in: query
        name: entryId
        description: Entry id to update
      - in: query
        name: No Name
      - in: query
        name: resource[assetId]
        description: ID of the source asset
      - in: query
        name: resource[content]
        description: Textual content
      - in: query
        name: resource[dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[entryId]
        description: ID of the source entry
      - in: formData
        name: resource[fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[objectType]
      - in: query
        name: resource[privateKey]
        description: SSH private key
      - in: query
        name: resource[publicKey]
        description: SSH public key
      - in: query
        name: resource[resources]
      - in: query
        name: resource[resource][assetId]
        description: ID of the source asset
      - in: query
        name: resource[resource][content]
        description: Textual content
      - in: query
        name: resource[resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[resource][entryId]
        description: ID of the source entry
      - in: formData
        name: resource[resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[resource][objectType]
      - in: query
        name: resource[resource][privateKey]
        description: SSH private key
      - in: query
        name: resource[resource][publicKey]
        description: SSH public key
      - in: query
        name: resource[resource][resources]
      - in: query
        name: resource[resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: resource[resource][resource][content]
        description: Textual content
      - in: query
        name: resource[resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: resource[resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[resource][resource][objectType]
      - in: query
        name: resource[resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: resource[resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: resource[resource][resource][resources]
      - in: query
        name: resource[resource][resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: resource[resource][resource][resource][content]
        description: Textual content
      - in: query
        name: resource[resource][resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[resource][resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: resource[resource][resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[resource][resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[resource][resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[resource][resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[resource][resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[resource][resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[resource][resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[resource][resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[resource][resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[resource][resource][resource][objectType]
      - in: query
        name: resource[resource][resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: resource[resource][resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: resource[resource][resource][resource][resources]
      - in: query
        name: resource[resource][resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[resource][resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: resource[resource][resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[resource][resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: resource[resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: resource[resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: resource[resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[resource][token]
        description: Token that returned from upload
      - in: query
        name: resource[resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[resource][version]
        description: The version of the file sync object
      - in: query
        name: resource[storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[token]
        description: Token that returned from upload
      - in: query
        name: resource[url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[version]
        description: The version of the file sync object
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - UpdateContent
  /service/baseentry/action/updateThumbnailFromSourceEntry:
    get:
      summary: Get Service Baseentry Action Updatethumbnailfromsourceentry
      description: Update entry thumbnail from a different entry by a specified time
        offset (in seconds).
      operationId: baseEntry.updateThumbnailFromSourceEntry
      x-api-path-slug: servicebaseentryactionupdatethumbnailfromsourceentry-get
      parameters:
      - in: query
        name: entryId
        description: Media entry id
      - in: query
        name: No Name
      - in: query
        name: sourceEntryId
        description: Media entry id
      - in: query
        name: timeOffset
        description: Time offset (in seconds)
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - UpdateThumbnailFromSourceEntry
  /service/baseentry/action/updateThumbnailFromUrl:
    get:
      summary: Get Service Baseentry Action Updatethumbnailfromurl
      description: Update entry thumbnail using url.
      operationId: baseEntry.updateThumbnailFromUrl
      x-api-path-slug: servicebaseentryactionupdatethumbnailfromurl-get
      parameters:
      - in: query
        name: entryId
        description: Media entry id
      - in: query
        name: No Name
      - in: query
        name: url
        description: file url
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - UpdateThumbnailFromUrl
  /service/baseentry/action/updateThumbnailJpeg:
    post:
      summary: Post Service Baseentry Action Updatethumbnailjpeg
      description: Update entry thumbnail using a raw jpeg file.
      operationId: baseEntry.updateThumbnailJpeg
      x-api-path-slug: servicebaseentryactionupdatethumbnailjpeg-post
      parameters:
      - in: query
        name: entryId
        description: Media entry id
      - in: formData
        name: fileData
        description: Jpeg file data
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - UpdateThumbnailJpeg
  /service/baseentry/action/upload:
    post:
      summary: Post Service Baseentry Action Upload
      description: Upload a file to Kaltura, that can be used to create an entry.
      operationId: baseEntry.upload
      x-api-path-slug: servicebaseentryactionupload-post
      parameters:
      - in: formData
        name: fileData
        description: The file data
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Upload
  /service/batch/action/addBulkUploadResult:
    get:
      summary: Get Service Batch Action Addbulkuploadresult
      description: batch addBulkUploadResultAction action adds KalturaBulkUploadResult
        to the DB
      operationId: batch.addBulkUploadResult
      x-api-path-slug: servicebatchactionaddbulkuploadresult-get
      parameters:
      - in: query
        name: bulkUploadResult[accessControlProfileId]
      - in: query
        name: bulkUploadResult[action]
        description: 'Enum Type: `KalturaBulkUploadAction`'
      - in: query
        name: bulkUploadResult[appearInList]
      - in: query
        name: bulkUploadResult[bulkUploadJobId]
        description: The id of the parent job
      - in: query
        name: bulkUploadResult[bulkUploadResultObjectType]
        description: 'Enum Type: `KalturaBulkUploadObjectType`'
      - in: query
        name: bulkUploadResult[categoryId]
      - in: query
        name: bulkUploadResult[categoryReferenceId]
      - in: query
        name: bulkUploadResult[category]
      - in: query
        name: bulkUploadResult[city]
      - in: query
        name: bulkUploadResult[contentType]
      - in: query
        name: bulkUploadResult[contributionPolicy]
      - in: query
        name: bulkUploadResult[conversionProfileId]
      - in: query
        name: bulkUploadResult[country]
      - in: query
        name: bulkUploadResult[creatorId]
      - in: query
        name: bulkUploadResult[dateOfBirth]
      - in: query
        name: bulkUploadResult[defaultPermissionLevel]
      - in: query
        name: bulkUploadResult[description]
      - in: query
        name: bulkUploadResult[email]
      - in: query
        name: bulkUploadResult[entitledUsersEdit]
      - in: query
        name: bulkUploadResult[entitledUsersPublish]
      - in: query
        name: bulkUploadResult[entryId]
      - in: query
        name: bulkUploadResult[entryStatus]
      - in: query
        name: bulkUploadResult[errorCode]
      - in: query
        name: bulkUploadResult[errorDescription]
      - in: query
        name: bulkUploadResult[errorType]
      - in: query
        name: bulkUploadResult[firstName]
      - in: query
        name: bulkUploadResult[gender]
      - in: query
        name: bulkUploadResult[group]
      - in: query
        name: bulkUploadResult[inheritanceType]
      - in: query
        name: bulkUploadResult[lastName]
      - in: query
        name: bulkUploadResult[lineIndex]
        description: The index of the line in the CSV
      - in: query
        name: bulkUploadResult[moderation]
      - in: query
        name: bulkUploadResult[name]
      - in: query
        name: bulkUploadResult[objectErrorDescription]
      - in: query
        name: bulkUploadResult[objectId]
      - in: query
        name: bulkUploadResult[objectStatus]
      - in: query
        name: bulkUploadResult[objectType]
      - in: query
        name: bulkUploadResult[ownerId]
      - in: query
        name: bulkUploadResult[owner]
      - in: query
        name: bulkUploadResult[parentSystemName]
      - in: query
        name: bulkUploadResult[parentType]
      - in: query
        name: bulkUploadResult[partnerData]
      - in: query
        name: bulkUploadResult[partnerId]
      - in: query
        name: bulkUploadResult[partnerSortValue]
      - in: query
        name: bulkUploadResult[permissionLevel]
      - in: query
        name: bulkUploadResult[pluginsData]
      - in: query
        name: bulkUploadResult[privacy]
      - in: query
        name: bulkUploadResult[referenceId]
      - in: query
        name: bulkUploadResult[relativePath]
      - in: query
        name: bulkUploadResult[requiredObjectStatus]
      - in: query
        name: bulkUploadResult[resourceId]
      - in: query
        name: bulkUploadResult[rowData]
        description: The data as recieved in the csv
      - in: query
        name: bulkUploadResult[scheduleEndDate]
      - in: query
        name: bulkUploadResult[scheduleStartDate]
      - in: query
        name: bulkUploadResult[screenName]
      - in: query
        name: bulkUploadResult[sshKeyPassphrase]
      - in: query
        name: bulkUploadResult[sshPrivateKey]
      - in: query
        name: bulkUploadResult[sshPublicKey]
      - in: query
        name: bulkUploadResult[state]
      - in: query
        name: bulkUploadResult[status]
        description: 'Enum Type: `KalturaBulkUploadResultStatus`'
      - in: query
        name: bulkUploadResult[systemName]
      - in: query
        name: bulkUploadResult[tags]
      - in: query
        name: bulkUploadResult[templateEntryId]
      - in: query
        name: bulkUploadResult[thumbnailSaved]
      - in: query
        name: bulkUploadResult[thumbnailUrl]
      - in: query
        name: bulkUploadResult[title]
      - in: query
        name: bulkUploadResult[type]
      - in: query
        name: bulkUploadResult[updateMethod]
      - in: query
        name: bulkUploadResult[url]
      - in: query
        name: bulkUploadResult[userId]
      - in: query
        name: bulkUploadResult[userJoinPolicy]
      - in: query
        name: bulkUploadResult[zip]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - AddBulkUploadResult
  /service/batch/action/addMediaInfo:
    get:
      summary: Get Service Batch Action Addmediainfo
      description: batch addMediaInfoAction action saves a media info object
      operationId: batch.addMediaInfo
      x-api-path-slug: servicebatchactionaddmediainfo-get
      parameters:
      - in: query
        name: mediaInfo[audioBitRateMode]
        description: 'Enum Type: `KalturaBitRateMode`The audio bit rate mode'
      - in: query
        name: mediaInfo[audioBitRate]
        description: The audio bit rate
      - in: query
        name: mediaInfo[audioChannels]
        description: The number of audio channels
      - in: query
        name: mediaInfo[audioCodecId]
        description: The audio codec id
      - in: query
        name: mediaInfo[audioDuration]
        description: The audio duration
      - in: query
        name: mediaInfo[audioFormat]
        description: The audio format
      - in: query
        name: mediaInfo[audioResolution]
        description: The audio resolution
      - in: query
        name: mediaInfo[audioSamplingRate]
        description: The audio sampling rate
      - in: query
        name: mediaInfo[complexityValue]
      - in: query
        name: mediaInfo[containerBitRate]
        description: The container bit rate
      - in: query
        name: mediaInfo[containerDuration]
        description: The container duration
      - in: query
        name: mediaInfo[containerFormat]
        description: The container format
      - in: query
        name: mediaInfo[containerId]
        description: The container id
      - in: query
        name: mediaInfo[containerProfile]
        description: The container profile
      - in: query
        name: mediaInfo[contentStreams]
      - in: query
        name: mediaInfo[fileSize]
        description: The file size
      - in: query
        name: mediaInfo[flavorAssetId]
        description: The id of the related flavor asset
      - in: query
        name: mediaInfo[isFastStart]
      - in: query
        name: mediaInfo[maxGOP]
      - in: query
        name: mediaInfo[multiStreamInfo]
      - in: query
        name: mediaInfo[multiStream]
      - in: query
        name: mediaInfo[rawData]
        description: The data as returned by the mediainfo command line
      - in: query
        name: mediaInfo[scanType]
      - in: query
        name: mediaInfo[videoBitRateMode]
        description: 'Enum Type: `KalturaBitRateMode`The video bit rate mode'
      - in: query
        name: mediaInfo[videoBitRate]
        description: The video bit rate
      - in: query
        name: mediaInfo[videoCodecId]
        description: The video codec id
      - in: query
        name: mediaInfo[videoDar]
        description: The video display aspect ratio (dar)
      - in: query
        name: mediaInfo[videoDuration]
        description: The video duration
      - in: query
        name: mediaInfo[videoFormat]
        description: The video format
      - in: query
        name: mediaInfo[videoFrameRate]
        description: The video frame rate
      - in: query
        name: mediaInfo[videoHeight]
        description: The video height
      - in: query
        name: mediaInfo[videoRotation]
      - in: query
        name: mediaInfo[videoWidth]
        description: The video width
      - in: query
        name: mediaInfo[writingLib]
        description: The writing library
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - AddMediaInfo
  /service/batch/action/checkEntryIsDone:
    get:
      summary: Get Service Batch Action Checkentryisdone
      description: batch checkEntryIsDone Check weather a specified entry is done
        converting and changes it to ready.
      operationId: batch.checkEntryIsDone
      x-api-path-slug: servicebatchactioncheckentryisdone-get
      parameters:
      - in: query
        name: batchJobId
        description: The entry to check
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - CheckEntryIsDone
  /service/batch/action/checkFileExists:
    get:
      summary: Get Service Batch Action Checkfileexists
      description: batch checkFileExists action check if the file exists
      operationId: batch.checkFileExists
      x-api-path-slug: servicebatchactioncheckfileexists-get
      parameters:
      - in: query
        name: localPath
      - in: query
        name: No Name
      - in: query
        name: size
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - CheckFileExists
  /service/batch/action/cleanExclusiveJobs:
    get:
      summary: Get Service Batch Action Cleanexclusivejobs
      description: batch cleanExclusiveJobs action mark as fatal error all expired
        jobs
      operationId: batch.cleanExclusiveJobs
      x-api-path-slug: servicebatchactioncleanexclusivejobs-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - CleanExclusiveJobs
  /service/batch/action/countBulkUploadEntries:
    get:
      summary: Get Service Batch Action Countbulkuploadentries
      description: Returns total created entries count and total error entries count
      operationId: batch.countBulkUploadEntries
      x-api-path-slug: servicebatchactioncountbulkuploadentries-get
      parameters:
      - in: query
        name: bulkUploadJobId
        description: The id of the bulk upload job
      - in: query
        name: bulkUploadObjectType
        description: 'Enum Type: `KalturaBulkUploadObjectType`'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - CountBulkUploadEntries
  /service/batch/action/freeExclusiveJob:
    get:
      summary: Get Service Batch Action Freeexclusivejob
      description: batch freeExclusiveJobAction action allows to get a generic BatchJob
      operationId: batch.freeExclusiveJob
      x-api-path-slug: servicebatchactionfreeexclusivejob-get
      parameters:
      - in: query
        name: id
        description: The id of the job
      - in: query
        name: jobType
        description: 'Enum Type: `KalturaBatchJobType`The type of the job'
      - in: query
        name: lockKey[batchIndex]
      - in: query
        name: lockKey[schedulerId]
      - in: query
        name: lockKey[workerId]
      - in: query
        name: No Name
      - in: query
        name: resetExecutionAttempts
        description: Resets the job execution attampts to zero
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - FreeExclusiveJob
  /service/batch/action/getBulkUploadLastResult:
    get:
      summary: Get Service Batch Action Getbulkuploadlastresult
      description: batch getBulkUploadLastResultAction action returns the last result
        of the bulk upload
      operationId: batch.getBulkUploadLastResult
      x-api-path-slug: servicebatchactiongetbulkuploadlastresult-get
      parameters:
      - in: query
        name: bulkUploadJobId
        description: The id of the bulk upload job
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - GetBulkUploadLastResult
  /service/batch/action/getExclusiveAlmostDone:
    get:
      summary: Get Service Batch Action Getexclusivealmostdone
      description: batch getExclusiveAlmostDone action allows to get a BatchJob that
        wait for remote closure
      operationId: batch.getExclusiveAlmostDone
      x-api-path-slug: servicebatchactiongetexclusivealmostdone-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[batchVersionEqual]
      - in: query
        name: filter[batchVersionGreaterThanOrEqual]
      - in: query
        name: filter[batchVersionLessThanOrEqual]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[errNumberEqual]
      - in: query
        name: filter[errNumberIn]
      - in: query
        name: filter[errNumberNotIn]
      - in: query
        name: filter[errTypeEqual]
        description: 'Enum Type: `KalturaBatchJobErrorTypes`'
      - in: query
        name: filter[errTypeIn]
      - in: query
        name: filter[errTypeNotIn]
      - in: query
        name: filter[estimatedEffortGreaterThan]
      - in: query
        name: filter[estimatedEffortLessThan]
      - in: query
        name: filter[executionAttemptsGreaterThanOrEqual]
      - in: query
        name: filter[executionAttemptsLessThanOrEqual]
      - in: query
        name: filter[finishTimeGreaterThanOrEqual]
      - in: query
        name: filter[finishTimeLessThanOrEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idGreaterThanOrEqual]
      - in: query
        name: filter[jobSubTypeEqual]
      - in: query
        name: filter[jobSubTypeIn]
      - in: query
        name: filter[jobSubTypeNotIn]
      - in: query
        name: filter[jobTypeAndSubTypeIn]
      - in: query
        name: filter[jobTypeEqual]
        description: 'Enum Type: `KalturaBatchJobType`'
      - in: query
        name: filter[jobTypeIn]
      - in: query
        name: filter[jobTypeNotIn]
      - in: query
        name: filter[lockVersionGreaterThanOrEqual]
      - in: query
        name: filter[lockVersionLessThanOrEqual]
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[partnerIdNotIn]
      - in: query
        name: filter[priorityEqual]
      - in: query
        name: filter[priorityGreaterThanOrEqual]
      - in: query
        name: filter[priorityIn]
      - in: query
        name: filter[priorityLessThanOrEqual]
      - in: query
        name: filter[priorityNotIn]
      - in: query
        name: filter[queueTimeGreaterThanOrEqual]
      - in: query
        name: filter[queueTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaBatchJobStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[statusNotIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[urgencyGreaterThanOrEqual]
      - in: query
        name: filter[urgencyLessThanOrEqual]
      - in: query
        name: jobType
        description: 'Enum Type: `KalturaBatchJobType`The type of the job - could
          be a custom extended type'
      - in: query
        name: lockKey[batchIndex]
      - in: query
        name: lockKey[schedulerId]
      - in: query
        name: lockKey[workerId]
      - in: query
        name: maxExecutionTime
        description: The maximum time in seconds the job reguarly take
      - in: query
        name: No Name
      - in: query
        name: numberOfJobs
        description: The maximum number of jobs to return
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - GetExclusiveAlmostDone
  /service/batch/action/getExclusiveJobs:
    get:
      summary: Get Service Batch Action Getexclusivejobs
      description: batch getExclusiveJobsAction action allows to get a BatchJob
      operationId: batch.getExclusiveJobs
      x-api-path-slug: servicebatchactiongetexclusivejobs-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[batchVersionEqual]
      - in: query
        name: filter[batchVersionGreaterThanOrEqual]
      - in: query
        name: filter[batchVersionLessThanOrEqual]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[errNumberEqual]
      - in: query
        name: filter[errNumberIn]
      - in: query
        name: filter[errNumberNotIn]
      - in: query
        name: filter[errTypeEqual]
        description: 'Enum Type: `KalturaBatchJobErrorTypes`'
      - in: query
        name: filter[errTypeIn]
      - in: query
        name: filter[errTypeNotIn]
      - in: query
        name: filter[estimatedEffortGreaterThan]
      - in: query
        name: filter[estimatedEffortLessThan]
      - in: query
        name: filter[executionAttemptsGreaterThanOrEqual]
      - in: query
        name: filter[executionAttemptsLessThanOrEqual]
      - in: query
        name: filter[finishTimeGreaterThanOrEqual]
      - in: query
        name: filter[finishTimeLessThanOrEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idGreaterThanOrEqual]
      - in: query
        name: filter[jobSubTypeEqual]
      - in: query
        name: filter[jobSubTypeIn]
      - in: query
        name: filter[jobSubTypeNotIn]
      - in: query
        name: filter[jobTypeAndSubTypeIn]
      - in: query
        name: filter[jobTypeEqual]
        description: 'Enum Type: `KalturaBatchJobType`'
      - in: query
        name: filter[jobTypeIn]
      - in: query
        name: filter[jobTypeNotIn]
      - in: query
        name: filter[lockVersionGreaterThanOrEqual]
      - in: query
        name: filter[lockVersionLessThanOrEqual]
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[partnerIdNotIn]
      - in: query
        name: filter[priorityEqual]
      - in: query
        name: filter[priorityGreaterThanOrEqual]
      - in: query
        name: filter[priorityIn]
      - in: query
        name: filter[priorityLessThanOrEqual]
      - in: query
        name: filter[priorityNotIn]
      - in: query
        name: filter[queueTimeGreaterThanOrEqual]
      - in: query
        name: filter[queueTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaBatchJobStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[statusNotIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[urgencyGreaterThanOrEqual]
      - in: query
        name: filter[urgencyLessThanOrEqual]
      - in: query
        name: jobType
        description: 'Enum Type: `KalturaBatchJobType`The type of the job - could
          be a custom extended type'
      - in: query
        name: lockKey[batchIndex]
      - in: query
        name: lockKey[schedulerId]
      - in: query
        name: lockKey[workerId]
      - in: query
        name: maxExecutionTime
        description: The maximum time in seconds the job reguarly take
      - in: query
        name: maxJobToPullForCache
        description: The number of job to pull to cache
      - in: query
        name: No Name
      - in: query
        name: numberOfJobs
        description: The maximum number of jobs to return
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - GetExclusiveJobs
  /service/batch/action/getExclusiveNotificationJobs:
    get:
      summary: Get Service Batch Action Getexclusivenotificationjobs
      description: batch getExclusiveNotificationJob action allows to get a BatchJob
        of type NOTIFICATION
      operationId: batch.getExclusiveNotificationJobs
      x-api-path-slug: servicebatchactiongetexclusivenotificationjobs-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[batchVersionEqual]
      - in: query
        name: filter[batchVersionGreaterThanOrEqual]
      - in: query
        name: filter[batchVersionLessThanOrEqual]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[errNumberEqual]
      - in: query
        name: filter[errNumberIn]
      - in: query
        name: filter[errNumberNotIn]
      - in: query
        name: filter[errTypeEqual]
        description: 'Enum Type: `KalturaBatchJobErrorTypes`'
      - in: query
        name: filter[errTypeIn]
      - in: query
        name: filter[errTypeNotIn]
      - in: query
        name: filter[estimatedEffortGreaterThan]
      - in: query
        name: filter[estimatedEffortLessThan]
      - in: query
        name: filter[executionAttemptsGreaterThanOrEqual]
      - in: query
        name: filter[executionAttemptsLessThanOrEqual]
      - in: query
        name: filter[finishTimeGreaterThanOrEqual]
      - in: query
        name: filter[finishTimeLessThanOrEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idGreaterThanOrEqual]
      - in: query
        name: filter[jobSubTypeEqual]
      - in: query
        name: filter[jobSubTypeIn]
      - in: query
        name: filter[jobSubTypeNotIn]
      - in: query
        name: filter[jobTypeAndSubTypeIn]
      - in: query
        name: filter[jobTypeEqual]
        description: 'Enum Type: `KalturaBatchJobType`'
      - in: query
        name: filter[jobTypeIn]
      - in: query
        name: filter[jobTypeNotIn]
      - in: query
        name: filter[lockVersionGreaterThanOrEqual]
      - in: query
        name: filter[lockVersionLessThanOrEqual]
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[partnerIdNotIn]
      - in: query
        name: filter[priorityEqual]
      - in: query
        name: filter[priorityGreaterThanOrEqual]
      - in: query
        name: filter[priorityIn]
      - in: query
        name: filter[priorityLessThanOrEqual]
      - in: query
        name: filter[priorityNotIn]
      - in: query
        name: filter[queueTimeGreaterThanOrEqual]
      - in: query
        name: filter[queueTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaBatchJobStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[statusNotIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[urgencyGreaterThanOrEqual]
      - in: query
        name: filter[urgencyLessThanOrEqual]
      - in: query
        name: lockKey[batchIndex]
      - in: query
        name: lockKey[schedulerId]
      - in: query
        name: lockKey[workerId]
      - in: query
        name: maxExecutionTime
        description: The maximum time in seconds the job reguarly take
      - in: query
        name: No Name
      - in: query
        name: numberOfJobs
        description: The maximum number of jobs to return
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - GetExclusiveNotificationJobs
  /service/batch/action/getQueueSize:
    get:
      summary: Get Service Batch Action Getqueuesize
      description: batch getQueueSize action get the queue size for job type
      operationId: batch.getQueueSize
      x-api-path-slug: servicebatchactiongetqueuesize-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: workerQueueFilter[filter][advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][categoriesMatchOr]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][categoryEntryStatusIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][categoryIdEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][contentLike]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][contentMultiLikeAnd]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][contentMultiLikeOr]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][cuePointsFreeText]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][cuePointTypeIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][depthGreaterThanEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][distributionProfileId]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: workerQueueFilter[filter][advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][extendedStatusIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][field]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][idEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][idIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][indexIdGreaterThan]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][items]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][memberIdEq]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][memberIdIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][metadataProfileId]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][noDistributionProfiles]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][not]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][objectType]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][userIdEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][userIdIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][value]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][watermarkId]
      - in: query
        name: workerQueueFilter[filter][batchVersionEqual]
      - in: query
        name: workerQueueFilter[filter][batchVersionGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][batchVersionLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][createdAtGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][createdAtLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][entryIdEqual]
      - in: query
        name: workerQueueFilter[filter][errNumberEqual]
      - in: query
        name: workerQueueFilter[filter][errNumberIn]
      - in: query
        name: workerQueueFilter[filter][errNumberNotIn]
      - in: query
        name: workerQueueFilter[filter][errTypeEqual]
        description: 'Enum Type: `KalturaBatchJobErrorTypes`'
      - in: query
        name: workerQueueFilter[filter][errTypeIn]
      - in: query
        name: workerQueueFilter[filter][errTypeNotIn]
      - in: query
        name: workerQueueFilter[filter][estimatedEffortGreaterThan]
      - in: query
        name: workerQueueFilter[filter][estimatedEffortLessThan]
      - in: query
        name: workerQueueFilter[filter][executionAttemptsGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][executionAttemptsLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][finishTimeGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][finishTimeLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][idEqual]
      - in: query
        name: workerQueueFilter[filter][idGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][jobSubTypeEqual]
      - in: query
        name: workerQueueFilter[filter][jobSubTypeIn]
      - in: query
        name: workerQueueFilter[filter][jobSubTypeNotIn]
      - in: query
        name: workerQueueFilter[filter][jobTypeAndSubTypeIn]
      - in: query
        name: workerQueueFilter[filter][jobTypeEqual]
        description: 'Enum Type: `KalturaBatchJobType`'
      - in: query
        name: workerQueueFilter[filter][jobTypeIn]
      - in: query
        name: workerQueueFilter[filter][jobTypeNotIn]
      - in: query
        name: workerQueueFilter[filter][lockVersionGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][lockVersionLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][objectType]
      - in: query
        name: workerQueueFilter[filter][orderBy]
      - in: query
        name: workerQueueFilter[filter][partnerIdEqual]
      - in: query
        name: workerQueueFilter[filter][partnerIdIn]
      - in: query
        name: workerQueueFilter[filter][partnerIdNotIn]
      - in: query
        name: workerQueueFilter[filter][priorityEqual]
      - in: query
        name: workerQueueFilter[filter][priorityGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][priorityIn]
      - in: query
        name: workerQueueFilter[filter][priorityLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][priorityNotIn]
      - in: query
        name: workerQueueFilter[filter][queueTimeGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][queueTimeLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][statusEqual]
        description: 'Enum Type: `KalturaBatchJobStatus`'
      - in: query
        name: workerQueueFilter[filter][statusIn]
      - in: query
        name: workerQueueFilter[filter][statusNotIn]
      - in: query
        name: workerQueueFilter[filter][updatedAtGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][updatedAtLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][urgencyGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][urgencyLessThanOrEqual]
      - in: query
        name: workerQueueFilter[jobType]
        description: 'Enum Type: `KalturaBatchJobType`'
      - in: query
        name: workerQueueFilter[schedulerId]
      - in: query
        name: workerQueueFilter[workerId]
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - GetQueueSize
  /service/batch/action/logConversion:
    get:
      summary: Get Service Batch Action Logconversion
      description: Add the data to the flavor asset conversion log, creates it if
        doesn't exists
      operationId: batch.logConversion
      x-api-path-slug: servicebatchactionlogconversion-get
      parameters:
      - in: query
        name: data
      - in: query
        name: flavorAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - LogConversion
  /service/batch/action/resetJobExecutionAttempts:
    get:
      summary: Get Service Batch Action Resetjobexecutionattempts
      description: batch resetJobExecutionAttempts action resets the execution attempts
        of the job
      operationId: batch.resetJobExecutionAttempts
      x-api-path-slug: servicebatchactionresetjobexecutionattempts-get
      parameters:
      - in: query
        name: id
        description: The id of the job
      - in: query
        name: jobType
        description: 'Enum Type: `KalturaBatchJobType`The type of the job'
      - in: query
        name: lockKey[batchIndex]
      - in: query
        name: lockKey[schedulerId]
      - in: query
        name: lockKey[workerId]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - ResetJobExecutionAttempts
  /service/batch/action/suspendJobs:
    get:
      summary: Get Service Batch Action Suspendjobs
      description: batch suspendJobs action suspends jobs from running.
      operationId: batch.suspendJobs
      x-api-path-slug: servicebatchactionsuspendjobs-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - SuspendJobs
  /service/batch/action/updateBulkUploadResults:
    get:
      summary: Get Service Batch Action Updatebulkuploadresults
      description: batch updateBulkUploadResults action adds KalturaBulkUploadResult
        to the DB
      operationId: batch.updateBulkUploadResults
      x-api-path-slug: servicebatchactionupdatebulkuploadresults-get
      parameters:
      - in: query
        name: bulkUploadJobId
        description: The id of the bulk upload job
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - UpdateBulkUploadResults
  /service/batch/action/updateExclusiveConvertCollectionJob:
    get:
      summary: Get Service Batch Action Updateexclusiveconvertcollectionjob
      description: batch updateExclusiveConvertCollectionJobAction action updates
        a BatchJob of type CONVERT_PROFILE that was claimed using the getExclusiveConvertJobs
      operationId: batch.updateExclusiveConvertCollectionJob
      x-api-path-slug: servicebatchactionupdateexclusiveconvertcollectionjob-get
      parameters:
      - in: query
        name: id
        description: The id of the job to free
      - in: query
        name: job[data][actualSrcFileSyncLocalPath]
        description: The translated path as used by the scheduler
      - in: query
        name: job[data][addedPrivacyContexts]
      - in: query
        name: job[data][amfArray]
        description: amf Array File Path
      - in: query
        name: job[data][assetId]
      - in: query
        name: job[data][authenticationMethod]
        description: 'Enum Type: `KalturaHttpNotificationAuthenticationMethod`The
          HTTP authentication method to use'
      - in: query
        name: job[data][backupEncoderIP]
      - in: query
        name: job[data][backupStreamID]
      - in: query
        name: job[data][bodyParams]
      - in: query
        name: job[data][cachedObjectType]
        description: Class name
      - in: query
        name: job[data][calculateComplexity]
      - in: query
        name: job[data][campaignId]
      - in: query
        name: job[data][captionAssetId]
      - in: query
        name: job[data][categoryId]
        description: category id
      - in: query
        name: job[data][changedCategoryId]
      - in: query
        name: job[data][columns]
      - in: query
        name: job[data][commandLinesStr]
      - in: query
        name: job[data][concatenatedDuration]
        description: duration of the concated video
      - in: query
        name: job[data][connectTimeout]
        description: The number of seconds to wait while trying to connect
      - in: query
        name: job[data][contentMatchPolicy]
        description: 'Enum Type: `KalturaDropFolderContentFileHandlerMatchPolicy`'
      - in: query
        name: job[data][contentMoid]
        description: Unique Kontiki MOID for the content uploaded to Kontiki
      - in: query
        name: job[data][contentParameters]
      - in: query
        name: job[data][conversionProfileId]
      - in: query
        name: job[data][cpcode]
      - in: query
        name: job[data][createLink]
      - in: query
        name: job[data][createThumb]
        description: Indicates if a thumbnail should be created
      - in: query
        name: job[data][customData]
      - in: query
        name: job[data][customHeaders]
      - in: query
        name: job[data][data]
      - in: query
        name: job[data][deletedPrivacyContexts]
      - in: query
        name: job[data][description]
      - in: query
        name: job[data][destCategoryFullIds]
        description: Destination categories fallback ids
      - in: query
        name: job[data][destCategoryId]
        description: Destination category id
      - in: query
        name: job[data][destDataFilePath]
        description: The data output file
      - in: query
        name: job[data][destDirLocalPath]
      - in: query
        name: job[data][destDirRemoteUrl]
      - in: query
        name: job[data][destFileLocalPath]
      - in: query
        name: job[data][destFileName]
      - in: query
        name: job[data][destFilePath]
        description: Output file
      - in: query
        name: job[data][destFileSyncLocalPath]
      - in: query
        name: job[data][destFileSyncRemoteUrl]
      - in: query
        name: job[data][destFileSyncStoredPath]
      - in: query
        name: job[data][destVersion]
      - in: query
        name: job[data][destXsdPath]
      - in: query
        name: job[data][detectGOP]
      - in: query
        name: job[data][distributionProfileId]
      - in: query
        name: job[data][distributionProfile][accountId]
      - in: query
        name: job[data][distributionProfile][adFreeApplicationGuid]
        description: The GUID for the application in which to record metrics and enforce
          business rules obtained through your Unicorn representative
      - in: query
        name: job[data][distributionProfile][adServerPartnerId]
      - in: query
        name: job[data][distributionProfile][allowAdsenseForVideo]
      - in: query
        name: job[data][distributionProfile][allowComments]
      - in: query
        name: job[data][distributionProfile][allowDownload]
      - in: query
        name: job[data][distributionProfile][allowEmbedding]
      - in: query
        name: job[data][distributionProfile][allowInvideo]
      - in: query
        name: job[data][distributionProfile][allowMidRollAds]
      - in: query
        name: job[data][distributionProfile][allowPostRollAds]
      - in: query
        name: job[data][distributionProfile][allowPreRollAds]
      - in: query
        name: job[data][distributionProfile][allowRatings]
      - in: query
        name: job[data][distributionProfile][allowResponses]
      - in: query
        name: job[data][distributionProfile][allowStreaming]
      - in: query
        name: job[data][distributionProfile][allowSyndication]
      - in: query
        name: job[data][distributionProfile][apiAuthorizeUrl]
      - in: query
        name: job[data][distributionProfile][apiHostUrl]
        description: The API host URL that the Upload User should have access to,
          Used for HTTP content submission
      - in: query
        name: job[data][distributionProfile][apikey]
      - in: query
        name: job[data][distributionProfile][asperaHost]
      - in: query
        name: job[data][distributionProfile][asperaLogin]
      - in: query
        name: job[data][distributionProfile][asperaPass]
      - in: query
        name: job[data][distributionProfile][asperaPrivateKey]
      - in: query
        name: job[data][distributionProfile][asperaPublicKey]
      - in: query
        name: job[data][distributionProfile][assetFilenameXslt]
      - in: query
        name: job[data][distributionProfile][assumeSuccess]
      - in: query
        name: job[data][distributionProfile][autoCreateFlavors]
        description: Comma separated flavor params ids that should be auto converted
      - in: query
        name: job[data][distributionProfile][autoCreateThumb]
        description: Comma separated thumbnail params ids that should be auto generated
      - in: query
        name: job[data][distributionProfile][backgroundImageStandard]
      - in: query
        name: job[data][distributionProfile][backgroundImageWide]
      - in: query
        name: job[data][distributionProfile][basePath]
      - in: query
        name: job[data][distributionProfile][blockOutsideOwnership]
      - in: query
        name: job[data][distributionProfile][bodyXslt]
      - in: query
        name: job[data][distributionProfile][captionAutosync]
      - in: query
        name: job[data][distributionProfile][categoryId]
      - in: query
        name: job[data][distributionProfile][certificateKey]
      - in: query
        name: job[data][distributionProfile][channelCopyright]
      - in: query
        name: job[data][distributionProfile][channelDescription]
      - in: query
        name: job[data][distributionProfile][channelGenerator]
      - in: query
        name: job[data][distributionProfile][channelGuid]
        description: The Channel GUID assigned to this Publication Rule
      - in: query
        name: job[data][distributionProfile][channelImageHeight]
      - in: query
        name: job[data][distributionProfile][channelImageLink]
      - in: query
        name: job[data][distributionProfile][channelImageTitle]
      - in: query
        name: job[data][distributionProfile][channelImageUrl]
      - in: query
        name: job[data][distributionProfile][channelImageWidth]
      - in: query
        name: job[data][distributionProfile][channelLanguage]
      - in: query
        name: job[data][distributionProfile][channelLink]
      - in: query
        name: job[data][distributionProfile][channelManagingEditor]
      - in: query
        name: job[data][distributionProfile][channelRating]
      - in: query
        name: job[data][distributionProfile][channelTitle]
      - in: query
        name: job[data][distributionProfile][claimType]
      - in: query
        name: job[data][distributionProfile][commercialPolicy]
      - in: query
        name: job[data][distributionProfile][contactEmail]
      - in: query
        name: job[data][distributionProfile][contactTelephone]
      - in: query
        name: job[data][distributionProfile][contentOwner]
      - in: query
        name: job[data][distributionProfile][copyright]
      - in: query
        name: job[data][distributionProfile][cPlatformTvSeriesField]
      - in: query
        name: job[data][distributionProfile][cPlatformTvSeries]
      - in: query
        name: job[data][distributionProfile][csId]
      - in: query
        name: job[data][distributionProfile][cuePointsProvider]
      - in: query
        name: job[data][distributionProfile][defaultCategory]
      - in: query
        name: job[data][distributionProfile][deleteEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: job[data][distributionProfile][deleteReference]
      - in: query
        name: job[data][distributionProfile][disableEpisodeNumberCustomValidation]
      - in: query
        name: job[data][distributionProfile][disableMetadata]
      - in: query
        name: job[data][distributionProfile][distributeCaptions]
      - in: query
        name: job[data][distributionProfile][distributeCuePoints]
      - in: query
        name: job[data][distributionProfile][distributeRemoteCaptionAssetContent]
      - in: query
        name: job[data][distributionProfile][distributeRemoteFlavorAssetContent]
      - in: query
        name: job[data][distributionProfile][distributeRemoteThumbAssetContent]
      - in: query
        name: job[data][distributionProfile][domainGuid]
        description: The GUID of the Customer Domain in the Unicorn system obtained
          by contacting your Unicorn representative
      - in: query
        name: job[data][distributionProfile][domainName]
        description: The name of the Domain that the Upload User should have access
          to, Used for authentication
      - in: query
        name: job[data][distributionProfile][domain]
      - in: query
        name: job[data][distributionProfile][downloadPriceCode]
      - in: query
        name: job[data][distributionProfile][email]
      - in: query
        name: job[data][distributionProfile][enableAdServer]
      - in: query
        name: job[data][distributionProfile][entitlements]
      - in: query
        name: job[data][distributionProfile][entitlement]
      - in: query
        name: job[data][distributionProfile][feedAuthorName]
      - in: query
        name: job[data][distributionProfile][feedCopyright]
      - in: query
        name: job[data][distributionProfile][feedDescription]
      - in: query
        name: job[data][distributionProfile][feedImageHeight]
      - in: query
        name: job[data][distributionProfile][feedImageLink]
      - in: query
        name: job[data][distributionProfile][feedImageTitle]
      - in: query
        name: job[data][distributionProfile][feedImageUrl]
      - in: query
        name: job[data][distributionProfile][feedImageWidth]
      - in: query
        name: job[data][distributionProfile][feedLanguage]
      - in: query
        name: job[data][distributionProfile][feedLastBuildDate]
      - in: query
        name: job[data][distributionProfile][feedLink]
      - in: query
        name: job[data][distributionProfile][feedSpecVersion]
        description: 'Enum Type: `KalturaYouTubeDistributionFeedSpecVersion`'
      - in: query
        name: job[data][distributionProfile][feedSubtitle]
      - in: query
        name: job[data][distributionProfile][feedTitle]
      - in: query
        name: job[data][distributionProfile][fieldConfigArray]
      - in: query
        name: job[data][distributionProfile][flavorAssetFilenameXslt]
      - in: query
        name: job[data][distributionProfile][flvFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][ftpHost]
      - in: query
        name: job[data][distributionProfile][ftpLogin]
      - in: query
        name: job[data][distributionProfile][ftpPassword]
      - in: query
        name: job[data][distributionProfile][ftpPass]
      - in: query
        name: job[data][distributionProfile][ftpPath]
      - in: query
        name: job[data][distributionProfile][ftpUsername]
      - in: query
        name: job[data][distributionProfile][genericProviderId]
        description: '`insertOnly`'
      - in: query
        name: job[data][distributionProfile][geoBlockingMapping]
        description: 'Enum Type: `KalturaDailymotionGeoBlockingMapping`'
      - in: query
        name: job[data][distributionProfile][googleClientId]
      - in: query
        name: job[data][distributionProfile][googleClientSecret]
      - in: query
        name: job[data][distributionProfile][googleTokenData]
      - in: query
        name: job[data][distributionProfile][hideViewCount]
      - in: query
        name: job[data][distributionProfile][host]
      - in: query
        name: job[data][distributionProfile][ignoreSchedulingInFeed]
      - in: query
        name: job[data][distributionProfile][ingestUrl]
      - in: query
        name: job[data][distributionProfile][instreamStandard]
      - in: query
        name: job[data][distributionProfile][instreamTrueview]
      - in: query
        name: job[data][distributionProfile][ips]
      - in: query
        name: job[data][distributionProfile][itemLink]
      - in: query
        name: job[data][distributionProfile][itemMediaRating]
      - in: query
        name: job[data][distributionProfile][itemsPerPage]
      - in: query
        name: job[data][distributionProfile][itemType]
      - in: query
        name: job[data][distributionProfile][itemXpathsToExtend]
      - in: query
        name: job[data][distributionProfile][mapAccessControlProfileIds]
      - in: query
        name: job[data][distributionProfile][mapCaptionParamsIds]
      - in: query
        name: job[data][distributionProfile][mapConversionProfileIds]
      - in: query
        name: job[data][distributionProfile][mapFlavorParamsIds]
      - in: query
        name: job[data][distributionProfile][mapMetadataProfileIds]
      - in: query
        name: job[data][distributionProfile][mapStorageProfileIds]
      - in: query
        name: job[data][distributionProfile][mapThumbParamsIds]
      - in: query
        name: job[data][distributionProfile][metadataFilenameXslt]
      - in: query
        name: job[data][distributionProfile][metadataProfileId]
      - in: query
        name: job[data][distributionProfile][metadataXpathsTriggerUpdate]
      - in: query
        name: job[data][distributionProfile][metadataXslt]
      - in: query
        name: job[data][distributionProfile][msnvideoCat]
      - in: query
        name: job[data][distributionProfile][msnvideoTopCat]
      - in: query
        name: job[data][distributionProfile][msnvideoTop]
      - in: query
        name: job[data][distributionProfile][name]
      - in: query
        name: job[data][distributionProfile][notificationEmail]
      - in: query
        name: job[data][distributionProfile][objectType]
      - in: query
        name: job[data][distributionProfile][optionalAssetDistributionRules]
      - in: query
        name: job[data][distributionProfile][optionalFlavorParamsIds]
        description: Comma separated flavor params ids that should be submitted if
          ready
      - in: query
        name: job[data][distributionProfile][optionalThumbDimensions]
      - in: query
        name: job[data][distributionProfile][overrideManualEdits]
      - in: query
        name: job[data][distributionProfile][ownerName]
      - in: query
        name: job[data][distributionProfile][pageAccessToken]
      - in: query
        name: job[data][distributionProfile][pageGroup]
      - in: query
        name: job[data][distributionProfile][pageId]
      - in: query
        name: job[data][distributionProfile][passphrase]
      - in: query
        name: job[data][distributionProfile][password]
      - in: query
        name: job[data][distributionProfile][permissions]
      - in: query
        name: job[data][distributionProfile][port]
      - in: query
        name: job[data][distributionProfile][priority]
      - in: query
        name: job[data][distributionProfile][privacyStatus]
      - in: query
        name: job[data][distributionProfile][processFeed]
        description: 'Enum Type: `KalturaYahooDistributionProcessFeedActionStatus`'
      - in: query
        name: job[data][distributionProfile][protocol]
        description: '`insertOnly`Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: job[data][distributionProfile][providerId]
      - in: query
        name: job[data][distributionProfile][providerName]
      - in: query
        name: job[data][distributionProfile][providerType]
        description: '`insertOnly`Enum Type: `KalturaDistributionProviderType`'
      - in: query
        name: job[data][distributionProfile][rating]
      - in: query
        name: job[data][distributionProfile][recommendedDcForDownload]
        description: The best Kaltura data center to be used to download the asset
          files to
      - in: query
        name: job[data][distributionProfile][recommendedDcForExecute]
        description: The best Kaltura data center to be used to execute the distribution
          job
      - in: query
        name: job[data][distributionProfile][recommendedStorageProfileForDownload]
        description: The best external storage to be used to download the asset files
          from
      - in: query
        name: job[data][distributionProfile][releaseClaims]
      - in: query
        name: job[data][distributionProfile][remoteAssetParamsId]
        description: The flavor-params that will be used for the remote asset
      - in: query
        name: job[data][distributionProfile][replaceAirDates]
      - in: query
        name: job[data][distributionProfile][replaceGroup]
      - in: query
        name: job[data][distributionProfile][reportEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: job[data][distributionProfile][requiredAssetDistributionRules]
      - in: query
        name: job[data][distributionProfile][requiredFlavorParamsIds]
        description: Comma separated flavor params ids that required to be ready before
          submission
      - in: query
        name: job[data][distributionProfile][requiredThumbDimensions]
      - in: query
        name: job[data][distributionProfile][reRequestPermissions]
      - in: query
        name: job[data][distributionProfile][seasonNumber]
      - in: query
        name: job[data][distributionProfile][seasonSynopsis]
      - in: query
        name: job[data][distributionProfile][seasonTuneInInformation]
      - in: query
        name: job[data][distributionProfile][sendMetadataAfterAssets]
      - in: query
        name: job[data][distributionProfile][seriesAdditionalCategories]
      - in: query
        name: job[data][distributionProfile][seriesChannel]
      - in: query
        name: job[data][distributionProfile][seriesPrimaryCategory]
      - in: query
        name: job[data][distributionProfile][sftpBaseDir]
      - in: query
        name: job[data][distributionProfile][sftpBasePath]
      - in: query
        name: job[data][distributionProfile][sftpHost]
      - in: query
        name: job[data][distributionProfile][sftpLogin]
      - in: query
        name: job[data][distributionProfile][sftpPass]
      - in: query
        name: job[data][distributionProfile][sftpPort]
      - in: query
        name: job[data][distributionProfile][sftpPrivateKey]
      - in: query
        name: job[data][distributionProfile][sftpPublicKey]
      - in: query
        name: job[data][distributionProfile][shouldAddThumbExtension]
      - in: query
        name: job[data][distributionProfile][shouldIncludeCaptions]
      - in: query
        name: job[data][distributionProfile][shouldIncludeCuePoints]
      - in: query
        name: job[data][distributionProfile][slFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][slHdFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][sourceFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][sourceFriendlyName]
      - in: query
        name: job[data][distributionProfile][source]
      - in: query
        name: job[data][distributionProfile][state]
      - in: query
        name: job[data][distributionProfile][status]
        description: 'Enum Type: `KalturaDistributionProfileStatus`'
      - in: query
        name: job[data][distributionProfile][storageProfileId]
        description: The remote storage that should be used for the remote asset
      - in: query
        name: job[data][distributionProfile][streamingPriceCode]
      - in: query
        name: job[data][distributionProfile][strict]
      - in: query
        name: job[data][distributionProfile][submitAction][ftpPassiveMode]
      - in: query
        name: job[data][distributionProfile][submitAction][httpFieldName]
      - in: query
        name: job[data][distributionProfile][submitAction][httpFileName]
      - in: query
        name: job[data][distributionProfile][submitAction][password]
      - in: query
        name: job[data][distributionProfile][submitAction][protocol]
        description: 'Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: job[data][distributionProfile][submitAction][serverPath]
      - in: query
        name: job[data][distributionProfile][submitAction][serverUrl]
      - in: query
        name: job[data][distributionProfile][submitAction][username]
      - in: query
        name: job[data][distributionProfile][submitEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: job[data][distributionProfile][sunriseDefaultOffset]
        description: If entry distribution sunrise not specified that will be the
          default since entry creation time, in seconds
      - in: query
        name: job[data][distributionProfile][sunsetDefaultOffset]
        description: If entry distribution sunset not specified that will be the default
          since entry creation time, in seconds
      - in: query
        name: job[data][distributionProfile][tags]
      - in: query
        name: job[data][distributionProfile][targetAccountId]
      - in: query
        name: job[data][distributionProfile][targetLoginId]
      - in: query
        name: job[data][distributionProfile][targetLoginPassword]
      - in: query
        name: job[data][distributionProfile][targetServiceUrl]
      - in: query
        name: job[data][distributionProfile][target]
      - in: query
        name: job[data][distributionProfile][thumbnailAssetFilenameXslt]
      - in: query
        name: job[data][distributionProfile][ugcPolicy]
      - in: query
        name: job[data][distributionProfile][updateEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: job[data][distributionProfile][upstreamNetworkId]
      - in: query
        name: job[data][distributionProfile][upstreamNetworkName]
      - in: query
        name: job[data][distributionProfile][upstreamVideoId]
      - in: query
        name: job[data][distributionProfile][urgentReference]
      - in: query
        name: job[data][distributionProfile][useCategoryEntries]
        description: When checking custom XSLT conditions using the fieldConfigArray
          - address only categories associated with the entry via the categoryEntry
          object
      - in: query
        name: job[data][distributionProfile][userAccessToken]
      - in: query
        name: job[data][distributionProfile][username]
      - in: query
        name: job[data][distributionProfile][user]
      - in: query
        name: job[data][distributionProfile][videoMediaType]
      - in: query
        name: job[data][distributionProfile][wmvFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][xsltFile]
      - in: query
        name: job[data][distributionProfile][xsl]
      - in: query
        name: job[data][domainName]
      - in: query
        name: job[data][dropFolderFileIds]
      - in: query
        name: job[data][dropFolderFileId]
      - in: query
        name: job[data][dropFolderId]
      - in: query
        name: job[data][duration]
        description: Clipping duration in seconds
      - in: query
        name: job[data][dvrEnabled]
        description: 'Enum Type: `KalturaDVRStatus`'
      - in: query
        name: job[data][dvrWindow]
      - in: query
        name: job[data][emailId]
      - in: query
        name: job[data][encoderIP]
      - in: query
        name: job[data][encoderPassword]
      - in: query
        name: job[data][encoderUsername]
      - in: query
        name: job[data][endDate]
      - in: query
        name: job[data][endObjectKey]
      - in: query
        name: job[data][endPoint]
      - in: query
        name: job[data][endTime]
        description: Duration of the live entry including all recorded segments including
          the current
      - in: query
        name: job[data][engineMessage]
      - in: query
        name: job[data][engineVersion]
      - in: query
        name: job[data][entryIds]
        description: Comma separated list of entry ids
      - in: query
        name: job[data][entryId]
        description: Live stream entry id
      - in: query
        name: job[data][eventsType]
        description: 'Enum Type: `KalturaScheduleEventType`The type of the events
          that ill be created by this upload'
      - in: query
        name: job[data][extractId3Tags]
      - in: query
        name: job[data][extraDestFileSyncs]
      - in: query
        name: job[data][fileIndex]
        description: The index of the file within the entry
      - in: query
        name: job[data][fileLocation]
      - in: query
        name: job[data][fileName]
        description: Friendly name of the file, used to be recognized later in the
          logs
      - in: query
        name: job[data][fileSize]
      - in: query
        name: job[data][filesPermissionInS3]
        description: 'Enum Type: `KalturaAmazonS3StorageProfileFilesPermissionLevel`'
      - in: query
        name: job[data][filter][advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: job[data][filter][advancedSearch][categoriesMatchOr]
      - in: query
        name: job[data][filter][advancedSearch][categoryEntryStatusIn]
      - in: query
        name: job[data][filter][advancedSearch][categoryIdEqual]
      - in: query
        name: job[data][filter][advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: job[data][filter][advancedSearch][contentLike]
      - in: query
        name: job[data][filter][advancedSearch][contentMultiLikeAnd]
      - in: query
        name: job[data][filter][advancedSearch][contentMultiLikeOr]
      - in: query
        name: job[data][filter][advancedSearch][cuePointsFreeText]
      - in: query
        name: job[data][filter][advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: job[data][filter][advancedSearch][cuePointTypeIn]
      - in: query
        name: job[data][filter][advancedSearch][depthGreaterThanEqual]
      - in: query
        name: job[data][filter][advancedSearch][distributionProfileId]
      - in: query
        name: job[data][filter][advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: job[data][filter][advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: job[data][filter][advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: job[data][filter][advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: job[data][filter][advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: job[data][filter][advancedSearch][extendedStatusIn]
      - in: query
        name: job[data][filter][advancedSearch][field]
      - in: query
        name: job[data][filter][advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: job[data][filter][advancedSearch][idEqual]
      - in: query
        name: job[data][filter][advancedSearch][idIn]
      - in: query
        name: job[data][filter][advancedSearch][indexIdGreaterThan]
      - in: query
        name: job[data][filter][advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: job[data][filter][advancedSearch][items]
      - in: query
        name: job[data][filter][advancedSearch][memberIdEq]
      - in: query
        name: job[data][filter][advancedSearch][memberIdIn]
      - in: query
        name: job[data][filter][advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: job[data][filter][advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: job[data][filter][advancedSearch][metadataProfileId]
      - in: query
        name: job[data][filter][advancedSearch][noDistributionProfiles]
      - in: query
        name: job[data][filter][advancedSearch][not]
      - in: query
        name: job[data][filter][advancedSearch][objectType]
      - in: query
        name: job[data][filter][advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: job[data][filter][advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: job[data][filter][advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: job[data][filter][advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: job[data][filter][advancedSearch][userIdEqual]
      - in: query
        name: job[data][filter][advancedSearch][userIdIn]
      - in: query
        name: job[data][filter][advancedSearch][value]
      - in: query
        name: job[data][filter][advancedSearch][watermarkId]
      - in: query
        name: job[data][filter][orderBy]
      - in: query
        name: job[data][flavorAssetId]
        description: Flavor asset to be ingested with the output
      - in: query
        name: job[data][flavorParamsId]
        description: Flavor params id to use for conversion
      - in: query
        name: job[data][flavorParamsOutputId]
      - in: query
        name: job[data][flavorParamsOutput][anamorphicPixels]
      - in: query
        name: job[data][flavorParamsOutput][aspectRatioProcessingMode]
      - in: query
        name: job[data][flavorParamsOutput][audioBitrate]
        description: The audio bitrate (in KBits) of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][audioChannels]
        description: The number of audio channels for downmixing
      - in: query
        name: job[data][flavorParamsOutput][audioCodec]
        description: 'Enum Type: `KalturaAudioCodec`The audio codec of the Flavor
          Params'
      - in: query
        name: job[data][flavorParamsOutput][audioSampleRate]
        description: The audio sample rate of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][clipDuration]
      - in: query
        name: job[data][flavorParamsOutput][clipOffset]
      - in: query
        name: job[data][flavorParamsOutput][commandLinesStr]
      - in: query
        name: job[data][flavorParamsOutput][contentAwareness]
      - in: query
        name: job[data][flavorParamsOutput][conversionEnginesExtraParams]
        description: The list of conversion engines extra params (separated with |)
      - in: query
        name: job[data][flavorParamsOutput][conversionEngines]
        description: The list of conversion engines (comma separated)
      - in: query
        name: job[data][flavorParamsOutput][deinterlice]
      - in: query
        name: job[data][flavorParamsOutput][densityHeight]
      - in: query
        name: job[data][flavorParamsOutput][densityWidth]
      - in: query
        name: job[data][flavorParamsOutput][depth]
      - in: query
        name: job[data][flavorParamsOutput][description]
        description: The description of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][engineVersion]
      - in: query
        name: job[data][flavorParamsOutput][flashVersion]
      - in: query
        name: job[data][flavorParamsOutput][flavorAssetId]
      - in: query
        name: job[data][flavorParamsOutput][flavorAssetVersion]
      - in: query
        name: job[data][flavorParamsOutput][flavorParamsId]
      - in: query
        name: job[data][flavorParamsOutput][flavorParamsVersion]
      - in: query
        name: job[data][flavorParamsOutput][forcedKeyFramesMode]
      - in: query
        name: job[data][flavorParamsOutput][forceFrameToMultiplication16]
      - in: query
        name: job[data][flavorParamsOutput][format]
        description: 'Enum Type: `KalturaContainerFormat`The container format of the
          Flavor Params'
      - in: query
        name: job[data][flavorParamsOutput][frameRate]
        description: The frame rate of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][gopSize]
        description: The gop size of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][height]
        description: The desired height of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][isAvoidForcedKeyFrames]
      - in: query
        name: job[data][flavorParamsOutput][isAvoidVideoShrinkBitrateToSource]
      - in: query
        name: job[data][flavorParamsOutput][isAvoidVideoShrinkFramesizeToSource]
      - in: query
        name: job[data][flavorParamsOutput][isCropIMX]
      - in: query
        name: job[data][flavorParamsOutput][isEncrypted]
      - in: query
        name: job[data][flavorParamsOutput][isGopInSec]
      - in: query
        name: job[data][flavorParamsOutput][isVideoFrameRateForLowBrAppleHls]
      - in: query
        name: job[data][flavorParamsOutput][maxFrameRate]
      - in: query
        name: job[data][flavorParamsOutput][mediaParserType]
        description: 'Enum Type: `KalturaMediaParserType`Media parser type to be used
          for post-conversion validation'
      - in: query
        name: job[data][flavorParamsOutput][multiStream]
      - in: query
        name: job[data][flavorParamsOutput][name]
        description: The name of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][objectType]
      - in: query
        name: job[data][flavorParamsOutput][operators]
      - in: query
        name: job[data][flavorParamsOutput][optimizationPolicy]
      - in: query
        name: job[data][flavorParamsOutput][partnerId]
      - in: query
        name: job[data][flavorParamsOutput][poly2Bitmap]
      - in: query
        name: job[data][flavorParamsOutput][readonly]
      - in: query
        name: job[data][flavorParamsOutput][readyBehavior]
      - in: query
        name: job[data][flavorParamsOutput][remoteStorageProfileIds]
        description: Comma seperated ids of remote storage profiles that the flavor
          distributed to, the distribution done by the conversion engine
      - in: query
        name: job[data][flavorParamsOutput][requiredPermissions]
      - in: query
        name: job[data][flavorParamsOutput][rotate]
      - in: query
        name: job[data][flavorParamsOutput][sizeHeight]
      - in: query
        name: job[data][flavorParamsOutput][sizeWidth]
      - in: query
        name: job[data][flavorParamsOutput][sourceAssetParamsIds]
        description: Comma seperated ids of source flavor params this flavor is created
          from
      - in: query
        name: job[data][flavorParamsOutput][sourceRemoteStorageProfileId]
        description: Id of remote storage profile that used to get the source, zero
          indicates Kaltura data center
      - in: query
        name: job[data][flavorParamsOutput][subtitlesData]
      - in: query
        name: job[data][flavorParamsOutput][systemName]
        description: System name of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][tags]
        description: The Flavor Params tags are used to identify the flavor for different
          usage (e
      - in: query
        name: job[data][flavorParamsOutput][twoPass]
      - in: query
        name: job[data][flavorParamsOutput][videoBitrateTolerance]
      - in: query
        name: job[data][flavorParamsOutput][videoBitrate]
        description: The video bitrate (in KBits) of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][videoCodec]
        description: 'Enum Type: `KalturaVideoCodec`The video codec of the Flavor
          Params'
      - in: query
        name: job[data][flavorParamsOutput][videoConstantBitrate]
      - in: query
        name: job[data][flavorParamsOutput][watermarkData]
      - in: query
        name: job[data][flavorParamsOutput][widevineDistributionEndDate]
        description: License distribution window end date
      - in: query
        name: job[data][flavorParamsOutput][widevineDistributionStartDate]
        description: License distribution window start date
      - in: query
        name: job[data][flavorParamsOutput][width]
        description: The desired width of the Flavor Params
      - in: query
        name: job[data][flavors]
      - in: query
        name: job[data][force]
      - in: query
        name: job[data][fromEmail]
      - in: query
        name: job[data][fromName]
      - in: query
        name: job[data][fromPartnerId]
        description: Id of the partner to copy from
      - in: query
        name: job[data][ftpPassiveMode]
      - in: query
        name: job[data][inputFileSyncLocalPath]
      - in: query
        name: job[data][inputXmlLocalPath]
      - in: query
        name: job[data][inputXmlRemoteUrl]
      - in: query
        name: job[data][isHtml]
      - in: query
        name: job[data][keepDistributionItem]
        description: Flag signifying that the associated distribution item should
          not be moved to removed status
      - in: query
        name: job[data][ksType]
        description: 'Enum Type: `KalturaSessionType`'
      - in: query
        name: job[data][language]
        description: 'Enum Type: `KalturaLanguageCode`'
      - in: query
        name: job[data][lastCuePointSyncTime]
        description: last live to vod sync time
      - in: query
        name: job[data][lastMovedCategoryEntryPageIndex]
        description: Saves the last page index of the category entries filter pager     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][lastMovedCategoryId]
        description: Saves the last category id that its entries moved completely     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][lastMovedCategoryPageIndex]
        description: Saves the last page index of the child categories filter pager     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][lastSegmentDrift]
        description: last segment drift
      - in: query
        name: job[data][lastSegmentDuration]
        description: last Segment Duration
      - in: query
        name: job[data][lastUpdatedCategoryCreatedAt]
        description: Saves the last sub category creation date that was updated     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][lastUpdatedCategoryEntryCreatedAt]
        description: Saves the last category entry creation date that was updated     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][liveEntryId]
        description: live Entry Id
      - in: query
        name: job[data][localFileSyncPath]
      - in: query
        name: job[data][logFileSyncLocalPath]
      - in: query
        name: job[data][logFileSyncRemoteUrl]
      - in: query
        name: job[data][mailPriority]
      - in: query
        name: job[data][mailType]
        description: 'Enum Type: `KalturaMailType`'
      - in: query
        name: job[data][maxResults]
      - in: query
        name: job[data][mediaServerIndex]
        description: 'Enum Type: `KalturaEntryServerNodeType`Primary or secondary
          media server'
      - in: query
        name: job[data][mediaType]
      - in: query
        name: job[data][metadataId]
      - in: query
        name: job[data][metadataProfileId]
      - in: query
        name: job[data][method]
        description: 'Enum Type: `KalturaHttpNotificationMethod`Request method'
      - in: query
        name: job[data][minSendDate]
      - in: query
        name: job[data][modifiedAttributes]
      - in: query
        name: job[data][monitorSyncCompletion]
      - in: query
        name: job[data][moveFromChildren]
        description: All entries from all child categories will be moved as well
      - in: query
        name: job[data][multiLanaguageCaptionAssetId]
      - in: query
        name: job[data][notificationEmail]
      - in: query
        name: job[data][notificationResult]
      - in: query
        name: job[data][numberOfAttempts]
      - in: query
        name: job[data][objectData][conversionProfileId]
        description: Selected profile id for all bulk entries
      - in: query
        name: job[data][objectData][objectType]
      - in: query
        name: job[data][objectId]
      - in: query
        name: job[data][objectType]
      - in: query
        name: job[data][objType]
        description: 'Enum Type: `KalturaNotificationObjectType`'
      - in: query
        name: job[data][offset]
        description: Clipping offset in seconds
      - in: query
        name: job[data][outputPath]
      - in: query
        name: job[data][parsedSlug]
      - in: query
        name: job[data][parsedUserId]
      - in: query
        name: job[data][passPhrase]
      - in: query
        name: job[data][password]
        description: A password to use for the connection
      - in: query
        name: job[data][plays]
      - in: query
        name: job[data][primaryBroadcastingUrl]
      - in: query
        name: job[data][primaryContact]
      - in: query
        name: job[data][privateKey]
      - in: query
        name: job[data][protocol]
        description: http / https
      - in: query
        name: job[data][providerData][additionalParameters]
        description: additional parameters to send to Cielo24
      - in: query
        name: job[data][providerData][captionAssetFormats]
        description: Caption formats
      - in: query
        name: job[data][providerData][entryId]
        description: Entry ID
      - in: query
        name: job[data][providerData][exampleUrl]
        description: Just an example
      - in: query
        name: job[data][providerData][fidelity]
        description: 'Enum Type: `KalturaCielo24Fidelity`'
      - in: query
        name: job[data][providerData][flavorAssetId]
        description: Flavor ID
      - in: query
        name: job[data][providerData][metadataProfileId]
        description: ID of the metadata profile for the extracted term metadata
      - in: query
        name: job[data][providerData][objectType]
      - in: query
        name: job[data][providerData][priority]
        description: 'Enum Type: `KalturaCielo24Priority`'
      - in: query
        name: job[data][providerData][replaceMediaContent]
        description: should replace remote media content
      - in: query
        name: job[data][providerData][spokenLanguage]
        description: 'Enum Type: `KalturaLanguage`Transcript content language'
      - in: query
        name: job[data][providerData][transcriptAssetId]
        description: ID of the transcript asset
      - in: query
        name: job[data][providerData][transcriptId]
        description: input Transcript-asset ID
      - in: query
        name: job[data][providerData][voicebaseApiKey]
        description: Voicebase API key to fetch transcript tokens
      - in: query
        name: job[data][providerData][voicebaseApiPassword]
        description: Voicebase API password to fetch transcript tokens
      - in: query
        name: job[data][providerType]
        description: 'Enum Type: `KalturaIntegrationProviderType`'
      - in: query
        name: job[data][provisioningParams]
      - in: query
        name: job[data][publicKey]
      - in: query
        name: job[data][puserId]
        description: The id of the requesting user
      - in: query
        name: job[data][recipientEmail]
      - in: query
        name: job[data][recipientId]
        description: kuserId
      - in: query
        name: job[data][recipientName]
      - in: query
        name: job[data][referenceTime]
      - in: query
        name: job[data][remoteMediaId]
      - in: query
        name: job[data][resultsFilePath]
      - in: query
        name: job[data][returnVal]
      - in: query
        name: job[data][rtmp]
      - in: query
        name: job[data][s3Region]
      - in: query
        name: job[data][scanResult]
        description: 'Enum Type: `KalturaVirusScanJobResult`'
      - in: query
        name: job[data][secondaryBroadcastingUrl]
      - in: query
        name: job[data][secondaryContact]
      - in: query
        name: job[data][separator]
      - in: query
        name: job[data][serverPassPhrase]
      - in: query
        name: job[data][serverPassword]
      - in: query
        name: job[data][serverPrivateKey]
      - in: query
        name: job[data][serverPublicKey]
      - in: query
        name: job[data][serverUrl]
      - in: query
        name: job[data][serverUsername]
      - in: query
        name: job[data][server][dc]
        description: The dc of the server
      - in: query
        name: job[data][server][description]
      - in: query
        name: job[data][server][host]
      - in: query
        name: job[data][server][name]
      - in: query
        name: job[data][server][objectType]
      - in: query
        name: job[data][server][password]
      - in: query
        name: job[data][server][port]
      - in: query
        name: job[data][server][protocol]
        description: 'Enum Type: `KalturaActivitiBusinessProcessServerProtocol`'
      - in: query
        name: job[data][server][systemName]
      - in: query
        name: job[data][server][username]
      - in: query
        name: job[data][serviceToken]
      - in: query
        name: job[data][signatureType]
      - in: query
        name: job[data][signSecret]
        description: The secret to sign the notification with
      - in: query
        name: job[data][srcAssetId]
      - in: query
        name: job[data][srcAssetType]
        description: 'Enum Type: `KalturaAssetType`'
      - in: query
        name: job[data][srcCategoryId]
        description: Source category id
      - in: query
        name: job[data][srcFilePath]
        description: The recorded live media
      - in: query
        name: job[data][srcFileSyncId]
      - in: query
        name: job[data][srcFileSyncLocalPath]
      - in: query
        name: job[data][srcFileSyncRemoteUrl]
      - in: query
        name: job[data][srcFileSyncs]
      - in: query
        name: job[data][srcFiles]
      - in: query
        name: job[data][srcFileUrl]
      - in: query
        name: job[data][srcVersion]
      - in: query
        name: job[data][srcXslPath]
      - in: query
        name: job[data][sseKmsKeyId]
      - in: query
        name: job[data][sseType]
      - in: query
        name: job[data][sslCertificatePassword]
        description: The password required to use the certificate
      - in: query
        name: job[data][sslCertificateType]
        description: 'Enum Type: `KalturaHttpNotificationCertificateType`The format
          of the certificate'
      - in: query
        name: job[data][sslCertificate]
        description: SSL certificate to verify the peer with
      - in: query
        name: job[data][sslEngineDefault]
        description: The identifier for the crypto engine used for asymmetric crypto
          operations
      - in: query
        name: job[data][sslEngine]
        description: The identifier for the crypto engine of the private SSL key specified
          in ssl key
      - in: query
        name: job[data][sslKeyPassword]
        description: The secret password needed to use the private SSL key specified
          in ssl key
      - in: query
        name: job[data][sslKeyType]
        description: 'Enum Type: `KalturaHttpNotificationSslKeyType`The key type of
          the private SSL key specified in ssl key - PEM / DER / ENG'
      - in: query
        name: job[data][sslKey]
        description: Private SSL key
      - in: query
        name: job[data][sslVersion]
        description: 'Enum Type: `KalturaHttpNotificationSslVersion`The SSL version
          (2 or 3) to use'
      - in: query
        name: job[data][startObjectKey]
      - in: query
        name: job[data][status]
        description: 'Enum Type: `KalturaMailJobStatus`'
      - in: query
        name: job[data][streamID]
      - in: query
        name: job[data][streamName]
      - in: query
        name: job[data][streamType]
        description: 'Enum Type: `KalturaAkamaiUniversalStreamType`'
      - in: query
        name: job[data][subjectParams]
      - in: query
        name: job[data][syncMode]
        description: 'Enum Type: `KalturaWidevineRepositorySyncMode`'
      - in: query
        name: job[data][systemPassword]
      - in: query
        name: job[data][systemUserName]
      - in: query
        name: job[data][templateId]
      - in: query
        name: job[data][templatePath]
      - in: query
        name: job[data][thumbAssetId]
      - in: query
        name: job[data][thumbBitrate]
        description: The bit rate of last created thumbnail, will be used to comapare
          if this thumbnail is the best we can have
      - in: query
        name: job[data][thumbHeight]
        description: The height of last created thumbnail, will be used to comapare
          if this thumbnail is the best we can have
      - in: query
        name: job[data][thumbOffset]
        description: The position of the thumbnail in the media file
      - in: query
        name: job[data][thumbParamsOutputId]
      - in: query
        name: job[data][thumbPath]
      - in: query
        name: job[data][timeout]
        description: The maximum number of seconds to allow cURL functions to execute
      - in: query
        name: job[data][timeReference]
      - in: query
        name: job[data][timeZoneOffset]
      - in: query
        name: job[data][toPartnerId]
        description: Id of the partner to copy to
      - in: query
        name: job[data][totalVodDuration]
        description: total VOD Duration
      - in: query
        name: job[data][to][categoryUserFilter][categoryDirectMembers]
        description: Return the list of categoryUser that are not inherited from parent
          category - only the direct categoryUsers
      - in: query
        name: job[data][to][categoryUserFilter][categoryFullIdsEqual]
      - in: query
        name: job[data][to][categoryUserFilter][categoryFullIdsStartsWith]
      - in: query
        name: job[data][to][categoryUserFilter][categoryIdEqual]
      - in: query
        name: job[data][to][categoryUserFilter][categoryIdIn]
      - in: query
        name: job[data][to][categoryUserFilter][createdAtGreaterThanOrEqual]
      - in: query
        name: job[data][to][categoryUserFilter][createdAtLessThanOrEqual]
      - in: query
        name: job[data][to][categoryUserFilter][freeText]
        description: Free text search on user id or screen name
      - in: query
        name: job[data][to][categoryUserFilter][orderBy]
      - in: query
        name: job[data][to][categoryUserFilter][permissionLevelEqual]
        description: 'Enum Type: `KalturaCategoryUserPermissionLevel`'
      - in: query
        name: job[data][to][categoryUserFilter][permissionLevelIn]
      - in: query
        name: job[data][to][categoryUserFilter][permissionNamesMatchAnd]
      - in: query
        name: job[data][to][categoryUserFilter][permissionNamesMatchOr]
      - in: query
        name: job[data][to][categoryUserFilter][permissionNamesNotContains]
      - in: query
        name: job[data][to][categoryUserFilter][relatedGroupsByUserId]
        description: Return a list of categoryUser that related to the userId in this
          field by groups
      - in: query
        name: job[data][to][categoryUserFilter][statusEqual]
        description: 'Enum Type: `KalturaCategoryUserStatus`'
      - in: query
        name: job[data][to][categoryUserFilter][statusIn]
      - in: query
        name: job[data][to][categoryUserFilter][updatedAtGreaterThanOrEqual]
      - in: query
        name: job[data][to][categoryUserFilter][updatedAtLessThanOrEqual]
      - in: query
        name: job[data][to][categoryUserFilter][updateMethodEqual]
        description: 'Enum Type: `KalturaUpdateMethodType`'
      - in: query
        name: job[data][to][categoryUserFilter][updateMethodIn]
      - in: query
        name: job[data][to][categoryUserFilter][userIdEqual]
      - in: query
        name: job[data][to][categoryUserFilter][userIdIn]
      - in: query
        name: job[data][to][emailRecipients]
      - in: query
        name: job[data][to][filter][createdAtGreaterThanOrEqual]
      - in: query
        name: job[data][to][filter][createdAtLessThanOrEqual]
      - in: query
        name: job[data][to][filter][emailLike]
      - in: query
        name: job[data][to][filter][emailStartsWith]
      - in: query
        name: job[data][to][filter][firstNameOrLastNameStartsWith]
      - in: query
        name: job[data][to][filter][firstNameStartsWith]
      - in: query
        name: job[data][to][filter][idEqual]
      - in: query
        name: job[data][to][filter][idIn]
      - in: query
        name: job[data][to][filter][idOrScreenNameStartsWith]
      - in: query
        name: job[data][to][filter][isAdminEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: job[data][to][filter][lastNameStartsWith]
      - in: query
        name: job[data][to][filter][loginEnabledEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: job[data][to][filter][objectType]
      - in: query
        name: job[data][to][filter][orderBy]
      - in: query
        name: job[data][to][filter][partnerIdEqual]
      - in: query
        name: job[data][to][filter][permissionNamesMultiLikeAnd]
        description: Permission names filter expression
      - in: query
        name: job[data][to][filter][permissionNamesMultiLikeOr]
        description: Permission names filter expression
      - in: query
        name: job[data][to][filter][roleIdEqual]
      - in: query
        name: job[data][to][filter][roleIdsEqual]
      - in: query
        name: job[data][to][filter][roleIdsIn]
      - in: query
        name: job[data][to][filter][screenNameLike]
      - in: query
        name: job[data][to][filter][screenNameStartsWith]
      - in: query
        name: job[data][to][filter][statusEqual]
        description: 'Enum Type: `KalturaUserStatus`'
      - in: query
        name: job[data][to][filter][statusIn]
      - in: query
        name: job[data][to][filter][tagsMultiLikeAnd]
      - in: query
        name: job[data][to][filter][tagsMultiLikeOr]
      - in: query
        name: job[data][to][filter][typeEqual]
        description: 'Enum Type: `KalturaUserType`'
      - in: query
        name: job[data][to][filter][typeIn]
      - in: query
        name: job[data][to][objectType]
      - in: query
        name: job[data][typeAsString]
      - in: query
        name: job[data][type]
        description: 'Enum Type: `KalturaNotificationType`'
      - in: query
        name: job[data][url]
        description: Remote server URL
      - in: query
        name: job[data][userId]
      - in: query
        name: job[data][username]
        description: A username to use for the connection
      - in: query
        name: job[data][userRoles]
      - in: query
        name: job[data][views]
      - in: query
        name: job[data][virusFoundAction]
        description: 'Enum Type: `KalturaVirusFoundAction`'
      - in: query
        name: job[data][vodEntryId]
        description: $vod Entry Id
      - in: query
        name: job[data][webexHostId]
      - in: query
        name: job[data][wsdlPassword]
      - in: query
        name: job[data][wsdlUsername]
      - in: query
        name: job[data][wvAssetIds]
      - in: query
        name: job[entryId]
      - in: query
        name: job[entryName]
      - in: query
        name: job[jobSubType]
      - in: query
        name: lockKey[batchIndex]
      - in: query
        name: lockKey[schedulerId]
      - in: query
        name: lockKey[workerId]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - UpdateExclusiveConvertCollectionJob
  /service/batch/action/updateExclusiveJob:
    get:
      summary: Get Service Batch Action Updateexclusivejob
      description: batch updateExclusiveJobAction action updates a BatchJob of extended
        type that was claimed using the getExclusiveJobs
      operationId: batch.updateExclusiveJob
      x-api-path-slug: servicebatchactionupdateexclusivejob-get
      parameters:
      - in: query
        name: id
        description: The id of the job to free
      - in: query
        name: job[data][actualSrcFileSyncLocalPath]
        description: The translated path as used by the scheduler
      - in: query
        name: job[data][addedPrivacyContexts]
      - in: query
        name: job[data][amfArray]
        description: amf Array File Path
      - in: query
        name: job[data][assetId]
      - in: query
        name: job[data][authenticationMethod]
        description: 'Enum Type: `KalturaHttpNotificationAuthenticationMethod`The
          HTTP authentication method to use'
      - in: query
        name: job[data][backupEncoderIP]
      - in: query
        name: job[data][backupStreamID]
      - in: query
        name: job[data][bodyParams]
      - in: query
        name: job[data][cachedObjectType]
        description: Class name
      - in: query
        name: job[data][calculateComplexity]
      - in: query
        name: job[data][campaignId]
      - in: query
        name: job[data][captionAssetId]
      - in: query
        name: job[data][categoryId]
        description: category id
      - in: query
        name: job[data][changedCategoryId]
      - in: query
        name: job[data][columns]
      - in: query
        name: job[data][commandLinesStr]
      - in: query
        name: job[data][concatenatedDuration]
        description: duration of the concated video
      - in: query
        name: job[data][connectTimeout]
        description: The number of seconds to wait while trying to connect
      - in: query
        name: job[data][contentMatchPolicy]
        description: 'Enum Type: `KalturaDropFolderContentFileHandlerMatchPolicy`'
      - in: query
        name: job[data][contentMoid]
        description: Unique Kontiki MOID for the content uploaded to Kontiki
      - in: query
        name: job[data][contentParameters]
      - in: query
        name: job[data][conversionProfileId]
      - in: query
        name: job[data][cpcode]
      - in: query
        name: job[data][createLink]
      - in: query
        name: job[data][createThumb]
        description: Indicates if a thumbnail should be created
      - in: query
        name: job[data][customData]
      - in: query
        name: job[data][customHeaders]
      - in: query
        name: job[data][data]
      - in: query
        name: job[data][deletedPrivacyContexts]
      - in: query
        name: job[data][description]
      - in: query
        name: job[data][destCategoryFullIds]
        description: Destination categories fallback ids
      - in: query
        name: job[data][destCategoryId]
        description: Destination category id
      - in: query
        name: job[data][destDataFilePath]
        description: The data output file
      - in: query
        name: job[data][destDirLocalPath]
      - in: query
        name: job[data][destDirRemoteUrl]
      - in: query
        name: job[data][destFileLocalPath]
      - in: query
        name: job[data][destFileName]
      - in: query
        name: job[data][destFilePath]
        description: Output file
      - in: query
        name: job[data][destFileSyncLocalPath]
      - in: query
        name: job[data][destFileSyncRemoteUrl]
      - in: query
        name: job[data][destFileSyncStoredPath]
      - in: query
        name: job[data][destVersion]
      - in: query
        name: job[data][destXsdPath]
      - in: query
        name: job[data][detectGOP]
      - in: query
        name: job[data][distributionProfileId]
      - in: query
        name: job[data][distributionProfile][accountId]
      - in: query
        name: job[data][distributionProfile][adFreeApplicationGuid]
        description: The GUID for the application in which to record metrics and enforce
          business rules obtained through your Unicorn representative
      - in: query
        name: job[data][distributionProfile][adServerPartnerId]
      - in: query
        name: job[data][distributionProfile][allowAdsenseForVideo]
      - in: query
        name: job[data][distributionProfile][allowComments]
      - in: query
        name: job[data][distributionProfile][allowDownload]
      - in: query
        name: job[data][distributionProfile][allowEmbedding]
      - in: query
        name: job[data][distributionProfile][allowInvideo]
      - in: query
        name: job[data][distributionProfile][allowMidRollAds]
      - in: query
        name: job[data][distributionProfile][allowPostRollAds]
      - in: query
        name: job[data][distributionProfile][allowPreRollAds]
      - in: query
        name: job[data][distributionProfile][allowRatings]
      - in: query
        name: job[data][distributionProfile][allowResponses]
      - in: query
        name: job[data][distributionProfile][allowStreaming]
      - in: query
        name: job[data][distributionProfile][allowSyndication]
      - in: query
        name: job[data][distributionProfile][apiAuthorizeUrl]
      - in: query
        name: job[data][distributionProfile][apiHostUrl]
        description: The API host URL that the Upload User should have access to,
          Used for HTTP content submission
      - in: query
        name: job[data][distributionProfile][apikey]
      - in: query
        name: job[data][distributionProfile][asperaHost]
      - in: query
        name: job[data][distributionProfile][asperaLogin]
      - in: query
        name: job[data][distributionProfile][asperaPass]
      - in: query
        name: job[data][distributionProfile][asperaPrivateKey]
      - in: query
        name: job[data][distributionProfile][asperaPublicKey]
      - in: query
        name: job[data][distributionProfile][assetFilenameXslt]
      - in: query
        name: job[data][distributionProfile][assumeSuccess]
      - in: query
        name: job[data][distributionProfile][autoCreateFlavors]
        description: Comma separated flavor params ids that should be auto converted
      - in: query
        name: job[data][distributionProfile][autoCreateThumb]
        description: Comma separated thumbnail params ids that should be auto generated
      - in: query
        name: job[data][distributionProfile][backgroundImageStandard]
      - in: query
        name: job[data][distributionProfile][backgroundImageWide]
      - in: query
        name: job[data][distributionProfile][basePath]
      - in: query
        name: job[data][distributionProfile][blockOutsideOwnership]
      - in: query
        name: job[data][distributionProfile][bodyXslt]
      - in: query
        name: job[data][distributionProfile][captionAutosync]
      - in: query
        name: job[data][distributionProfile][categoryId]
      - in: query
        name: job[data][distributionProfile][certificateKey]
      - in: query
        name: job[data][distributionProfile][channelCopyright]
      - in: query
        name: job[data][distributionProfile][channelDescription]
      - in: query
        name: job[data][distributionProfile][channelGenerator]
      - in: query
        name: job[data][distributionProfile][channelGuid]
        description: The Channel GUID assigned to this Publication Rule
      - in: query
        name: job[data][distributionProfile][channelImageHeight]
      - in: query
        name: job[data][distributionProfile][channelImageLink]
      - in: query
        name: job[data][distributionProfile][channelImageTitle]
      - in: query
        name: job[data][distributionProfile][channelImageUrl]
      - in: query
        name: job[data][distributionProfile][channelImageWidth]
      - in: query
        name: job[data][distributionProfile][channelLanguage]
      - in: query
        name: job[data][distributionProfile][channelLink]
      - in: query
        name: job[data][distributionProfile][channelManagingEditor]
      - in: query
        name: job[data][distributionProfile][channelRating]
      - in: query
        name: job[data][distributionProfile][channelTitle]
      - in: query
        name: job[data][distributionProfile][claimType]
      - in: query
        name: job[data][distributionProfile][commercialPolicy]
      - in: query
        name: job[data][distributionProfile][contactEmail]
      - in: query
        name: job[data][distributionProfile][contactTelephone]
      - in: query
        name: job[data][distributionProfile][contentOwner]
      - in: query
        name: job[data][distributionProfile][copyright]
      - in: query
        name: job[data][distributionProfile][cPlatformTvSeriesField]
      - in: query
        name: job[data][distributionProfile][cPlatformTvSeries]
      - in: query
        name: job[data][distributionProfile][csId]
      - in: query
        name: job[data][distributionProfile][cuePointsProvider]
      - in: query
        name: job[data][distributionProfile][defaultCategory]
      - in: query
        name: job[data][distributionProfile][deleteEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: job[data][distributionProfile][deleteReference]
      - in: query
        name: job[data][distributionProfile][disableEpisodeNumberCustomValidation]
      - in: query
        name: job[data][distributionProfile][disableMetadata]
      - in: query
        name: job[data][distributionProfile][distributeCaptions]
      - in: query
        name: job[data][distributionProfile][distributeCuePoints]
      - in: query
        name: job[data][distributionProfile][distributeRemoteCaptionAssetContent]
      - in: query
        name: job[data][distributionProfile][distributeRemoteFlavorAssetContent]
      - in: query
        name: job[data][distributionProfile][distributeRemoteThumbAssetContent]
      - in: query
        name: job[data][distributionProfile][domainGuid]
        description: The GUID of the Customer Domain in the Unicorn system obtained
          by contacting your Unicorn representative
      - in: query
        name: job[data][distributionProfile][domainName]
        description: The name of the Domain that the Upload User should have access
          to, Used for authentication
      - in: query
        name: job[data][distributionProfile][domain]
      - in: query
        name: job[data][distributionProfile][downloadPriceCode]
      - in: query
        name: job[data][distributionProfile][email]
      - in: query
        name: job[data][distributionProfile][enableAdServer]
      - in: query
        name: job[data][distributionProfile][entitlements]
      - in: query
        name: job[data][distributionProfile][entitlement]
      - in: query
        name: job[data][distributionProfile][feedAuthorName]
      - in: query
        name: job[data][distributionProfile][feedCopyright]
      - in: query
        name: job[data][distributionProfile][feedDescription]
      - in: query
        name: job[data][distributionProfile][feedImageHeight]
      - in: query
        name: job[data][distributionProfile][feedImageLink]
      - in: query
        name: job[data][distributionProfile][feedImageTitle]
      - in: query
        name: job[data][distributionProfile][feedImageUrl]
      - in: query
        name: job[data][distributionProfile][feedImageWidth]
      - in: query
        name: job[data][distributionProfile][feedLanguage]
      - in: query
        name: job[data][distributionProfile][feedLastBuildDate]
      - in: query
        name: job[data][distributionProfile][feedLink]
      - in: query
        name: job[data][distributionProfile][feedSpecVersion]
        description: 'Enum Type: `KalturaYouTubeDistributionFeedSpecVersion`'
      - in: query
        name: job[data][distributionProfile][feedSubtitle]
      - in: query
        name: job[data][distributionProfile][feedTitle]
      - in: query
        name: job[data][distributionProfile][fieldConfigArray]
      - in: query
        name: job[data][distributionProfile][flavorAssetFilenameXslt]
      - in: query
        name: job[data][distributionProfile][flvFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][ftpHost]
      - in: query
        name: job[data][distributionProfile][ftpLogin]
      - in: query
        name: job[data][distributionProfile][ftpPassword]
      - in: query
        name: job[data][distributionProfile][ftpPass]
      - in: query
        name: job[data][distributionProfile][ftpPath]
      - in: query
        name: job[data][distributionProfile][ftpUsername]
      - in: query
        name: job[data][distributionProfile][genericProviderId]
        description: '`insertOnly`'
      - in: query
        name: job[data][distributionProfile][geoBlockingMapping]
        description: 'Enum Type: `KalturaDailymotionGeoBlockingMapping`'
      - in: query
        name: job[data][distributionProfile][googleClientId]
      - in: query
        name: job[data][distributionProfile][googleClientSecret]
      - in: query
        name: job[data][distributionProfile][googleTokenData]
      - in: query
        name: job[data][distributionProfile][hideViewCount]
      - in: query
        name: job[data][distributionProfile][host]
      - in: query
        name: job[data][distributionProfile][ignoreSchedulingInFeed]
      - in: query
        name: job[data][distributionProfile][ingestUrl]
      - in: query
        name: job[data][distributionProfile][instreamStandard]
      - in: query
        name: job[data][distributionProfile][instreamTrueview]
      - in: query
        name: job[data][distributionProfile][ips]
      - in: query
        name: job[data][distributionProfile][itemLink]
      - in: query
        name: job[data][distributionProfile][itemMediaRating]
      - in: query
        name: job[data][distributionProfile][itemsPerPage]
      - in: query
        name: job[data][distributionProfile][itemType]
      - in: query
        name: job[data][distributionProfile][itemXpathsToExtend]
      - in: query
        name: job[data][distributionProfile][mapAccessControlProfileIds]
      - in: query
        name: job[data][distributionProfile][mapCaptionParamsIds]
      - in: query
        name: job[data][distributionProfile][mapConversionProfileIds]
      - in: query
        name: job[data][distributionProfile][mapFlavorParamsIds]
      - in: query
        name: job[data][distributionProfile][mapMetadataProfileIds]
      - in: query
        name: job[data][distributionProfile][mapStorageProfileIds]
      - in: query
        name: job[data][distributionProfile][mapThumbParamsIds]
      - in: query
        name: job[data][distributionProfile][metadataFilenameXslt]
      - in: query
        name: job[data][distributionProfile][metadataProfileId]
      - in: query
        name: job[data][distributionProfile][metadataXpathsTriggerUpdate]
      - in: query
        name: job[data][distributionProfile][metadataXslt]
      - in: query
        name: job[data][distributionProfile][msnvideoCat]
      - in: query
        name: job[data][distributionProfile][msnvideoTopCat]
      - in: query
        name: job[data][distributionProfile][msnvideoTop]
      - in: query
        name: job[data][distributionProfile][name]
      - in: query
        name: job[data][distributionProfile][notificationEmail]
      - in: query
        name: job[data][distributionProfile][objectType]
      - in: query
        name: job[data][distributionProfile][optionalAssetDistributionRules]
      - in: query
        name: job[data][distributionProfile][optionalFlavorParamsIds]
        description: Comma separated flavor params ids that should be submitted if
          ready
      - in: query
        name: job[data][distributionProfile][optionalThumbDimensions]
      - in: query
        name: job[data][distributionProfile][overrideManualEdits]
      - in: query
        name: job[data][distributionProfile][ownerName]
      - in: query
        name: job[data][distributionProfile][pageAccessToken]
      - in: query
        name: job[data][distributionProfile][pageGroup]
      - in: query
        name: job[data][distributionProfile][pageId]
      - in: query
        name: job[data][distributionProfile][passphrase]
      - in: query
        name: job[data][distributionProfile][password]
      - in: query
        name: job[data][distributionProfile][permissions]
      - in: query
        name: job[data][distributionProfile][port]
      - in: query
        name: job[data][distributionProfile][priority]
      - in: query
        name: job[data][distributionProfile][privacyStatus]
      - in: query
        name: job[data][distributionProfile][processFeed]
        description: 'Enum Type: `KalturaYahooDistributionProcessFeedActionStatus`'
      - in: query
        name: job[data][distributionProfile][protocol]
        description: '`insertOnly`Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: job[data][distributionProfile][providerId]
      - in: query
        name: job[data][distributionProfile][providerName]
      - in: query
        name: job[data][distributionProfile][providerType]
        description: '`insertOnly`Enum Type: `KalturaDistributionProviderType`'
      - in: query
        name: job[data][distributionProfile][rating]
      - in: query
        name: job[data][distributionProfile][recommendedDcForDownload]
        description: The best Kaltura data center to be used to download the asset
          files to
      - in: query
        name: job[data][distributionProfile][recommendedDcForExecute]
        description: The best Kaltura data center to be used to execute the distribution
          job
      - in: query
        name: job[data][distributionProfile][recommendedStorageProfileForDownload]
        description: The best external storage to be used to download the asset files
          from
      - in: query
        name: job[data][distributionProfile][releaseClaims]
      - in: query
        name: job[data][distributionProfile][remoteAssetParamsId]
        description: The flavor-params that will be used for the remote asset
      - in: query
        name: job[data][distributionProfile][replaceAirDates]
      - in: query
        name: job[data][distributionProfile][replaceGroup]
      - in: query
        name: job[data][distributionProfile][reportEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: job[data][distributionProfile][requiredAssetDistributionRules]
      - in: query
        name: job[data][distributionProfile][requiredFlavorParamsIds]
        description: Comma separated flavor params ids that required to be ready before
          submission
      - in: query
        name: job[data][distributionProfile][requiredThumbDimensions]
      - in: query
        name: job[data][distributionProfile][reRequestPermissions]
      - in: query
        name: job[data][distributionProfile][seasonNumber]
      - in: query
        name: job[data][distributionProfile][seasonSynopsis]
      - in: query
        name: job[data][distributionProfile][seasonTuneInInformation]
      - in: query
        name: job[data][distributionProfile][sendMetadataAfterAssets]
      - in: query
        name: job[data][distributionProfile][seriesAdditionalCategories]
      - in: query
        name: job[data][distributionProfile][seriesChannel]
      - in: query
        name: job[data][distributionProfile][seriesPrimaryCategory]
      - in: query
        name: job[data][distributionProfile][sftpBaseDir]
      - in: query
        name: job[data][distributionProfile][sftpBasePath]
      - in: query
        name: job[data][distributionProfile][sftpHost]
      - in: query
        name: job[data][distributionProfile][sftpLogin]
      - in: query
        name: job[data][distributionProfile][sftpPass]
      - in: query
        name: job[data][distributionProfile][sftpPort]
      - in: query
        name: job[data][distributionProfile][sftpPrivateKey]
      - in: query
        name: job[data][distributionProfile][sftpPublicKey]
      - in: query
        name: job[data][distributionProfile][shouldAddThumbExtension]
      - in: query
        name: job[data][distributionProfile][shouldIncludeCaptions]
      - in: query
        name: job[data][distributionProfile][shouldIncludeCuePoints]
      - in: query
        name: job[data][distributionProfile][slFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][slHdFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][sourceFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][sourceFriendlyName]
      - in: query
        name: job[data][distributionProfile][source]
      - in: query
        name: job[data][distributionProfile][state]
      - in: query
        name: job[data][distributionProfile][status]
        description: 'Enum Type: `KalturaDistributionProfileStatus`'
      - in: query
        name: job[data][distributionProfile][storageProfileId]
        description: The remote storage that should be used for the remote asset
      - in: query
        name: job[data][distributionProfile][streamingPriceCode]
      - in: query
        name: job[data][distributionProfile][strict]
      - in: query
        name: job[data][distributionProfile][submitAction][ftpPassiveMode]
      - in: query
        name: job[data][distributionProfile][submitAction][httpFieldName]
      - in: query
        name: job[data][distributionProfile][submitAction][httpFileName]
      - in: query
        name: job[data][distributionProfile][submitAction][password]
      - in: query
        name: job[data][distributionProfile][submitAction][protocol]
        description: 'Enum Type: `KalturaDistributionProtocol`'
      - in: query
        name: job[data][distributionProfile][submitAction][serverPath]
      - in: query
        name: job[data][distributionProfile][submitAction][serverUrl]
      - in: query
        name: job[data][distributionProfile][submitAction][username]
      - in: query
        name: job[data][distributionProfile][submitEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: job[data][distributionProfile][sunriseDefaultOffset]
        description: If entry distribution sunrise not specified that will be the
          default since entry creation time, in seconds
      - in: query
        name: job[data][distributionProfile][sunsetDefaultOffset]
        description: If entry distribution sunset not specified that will be the default
          since entry creation time, in seconds
      - in: query
        name: job[data][distributionProfile][tags]
      - in: query
        name: job[data][distributionProfile][targetAccountId]
      - in: query
        name: job[data][distributionProfile][targetLoginId]
      - in: query
        name: job[data][distributionProfile][targetLoginPassword]
      - in: query
        name: job[data][distributionProfile][targetServiceUrl]
      - in: query
        name: job[data][distributionProfile][target]
      - in: query
        name: job[data][distributionProfile][thumbnailAssetFilenameXslt]
      - in: query
        name: job[data][distributionProfile][ugcPolicy]
      - in: query
        name: job[data][distributionProfile][updateEnabled]
        description: 'Enum Type: `KalturaDistributionProfileActionStatus`'
      - in: query
        name: job[data][distributionProfile][upstreamNetworkId]
      - in: query
        name: job[data][distributionProfile][upstreamNetworkName]
      - in: query
        name: job[data][distributionProfile][upstreamVideoId]
      - in: query
        name: job[data][distributionProfile][urgentReference]
      - in: query
        name: job[data][distributionProfile][useCategoryEntries]
        description: When checking custom XSLT conditions using the fieldConfigArray
          - address only categories associated with the entry via the categoryEntry
          object
      - in: query
        name: job[data][distributionProfile][userAccessToken]
      - in: query
        name: job[data][distributionProfile][username]
      - in: query
        name: job[data][distributionProfile][user]
      - in: query
        name: job[data][distributionProfile][videoMediaType]
      - in: query
        name: job[data][distributionProfile][wmvFlavorParamsId]
      - in: query
        name: job[data][distributionProfile][xsltFile]
      - in: query
        name: job[data][distributionProfile][xsl]
      - in: query
        name: job[data][domainName]
      - in: query
        name: job[data][dropFolderFileIds]
      - in: query
        name: job[data][dropFolderFileId]
      - in: query
        name: job[data][dropFolderId]
      - in: query
        name: job[data][duration]
        description: Clipping duration in seconds
      - in: query
        name: job[data][dvrEnabled]
        description: 'Enum Type: `KalturaDVRStatus`'
      - in: query
        name: job[data][dvrWindow]
      - in: query
        name: job[data][emailId]
      - in: query
        name: job[data][encoderIP]
      - in: query
        name: job[data][encoderPassword]
      - in: query
        name: job[data][encoderUsername]
      - in: query
        name: job[data][endDate]
      - in: query
        name: job[data][endObjectKey]
      - in: query
        name: job[data][endPoint]
      - in: query
        name: job[data][endTime]
        description: Duration of the live entry including all recorded segments including
          the current
      - in: query
        name: job[data][engineMessage]
      - in: query
        name: job[data][engineVersion]
      - in: query
        name: job[data][entryIds]
        description: Comma separated list of entry ids
      - in: query
        name: job[data][entryId]
        description: Live stream entry id
      - in: query
        name: job[data][eventsType]
        description: 'Enum Type: `KalturaScheduleEventType`The type of the events
          that ill be created by this upload'
      - in: query
        name: job[data][extractId3Tags]
      - in: query
        name: job[data][extraDestFileSyncs]
      - in: query
        name: job[data][fileIndex]
        description: The index of the file within the entry
      - in: query
        name: job[data][fileLocation]
      - in: query
        name: job[data][fileName]
        description: Friendly name of the file, used to be recognized later in the
          logs
      - in: query
        name: job[data][fileSize]
      - in: query
        name: job[data][filesPermissionInS3]
        description: 'Enum Type: `KalturaAmazonS3StorageProfileFilesPermissionLevel`'
      - in: query
        name: job[data][filter][advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: job[data][filter][advancedSearch][categoriesMatchOr]
      - in: query
        name: job[data][filter][advancedSearch][categoryEntryStatusIn]
      - in: query
        name: job[data][filter][advancedSearch][categoryIdEqual]
      - in: query
        name: job[data][filter][advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: job[data][filter][advancedSearch][contentLike]
      - in: query
        name: job[data][filter][advancedSearch][contentMultiLikeAnd]
      - in: query
        name: job[data][filter][advancedSearch][contentMultiLikeOr]
      - in: query
        name: job[data][filter][advancedSearch][cuePointsFreeText]
      - in: query
        name: job[data][filter][advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: job[data][filter][advancedSearch][cuePointTypeIn]
      - in: query
        name: job[data][filter][advancedSearch][depthGreaterThanEqual]
      - in: query
        name: job[data][filter][advancedSearch][distributionProfileId]
      - in: query
        name: job[data][filter][advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: job[data][filter][advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: job[data][filter][advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: job[data][filter][advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: job[data][filter][advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: job[data][filter][advancedSearch][extendedStatusIn]
      - in: query
        name: job[data][filter][advancedSearch][field]
      - in: query
        name: job[data][filter][advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: job[data][filter][advancedSearch][idEqual]
      - in: query
        name: job[data][filter][advancedSearch][idIn]
      - in: query
        name: job[data][filter][advancedSearch][indexIdGreaterThan]
      - in: query
        name: job[data][filter][advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: job[data][filter][advancedSearch][items]
      - in: query
        name: job[data][filter][advancedSearch][memberIdEq]
      - in: query
        name: job[data][filter][advancedSearch][memberIdIn]
      - in: query
        name: job[data][filter][advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: job[data][filter][advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: job[data][filter][advancedSearch][metadataProfileId]
      - in: query
        name: job[data][filter][advancedSearch][noDistributionProfiles]
      - in: query
        name: job[data][filter][advancedSearch][not]
      - in: query
        name: job[data][filter][advancedSearch][objectType]
      - in: query
        name: job[data][filter][advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: job[data][filter][advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: job[data][filter][advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: job[data][filter][advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: job[data][filter][advancedSearch][userIdEqual]
      - in: query
        name: job[data][filter][advancedSearch][userIdIn]
      - in: query
        name: job[data][filter][advancedSearch][value]
      - in: query
        name: job[data][filter][advancedSearch][watermarkId]
      - in: query
        name: job[data][filter][orderBy]
      - in: query
        name: job[data][flavorAssetId]
        description: Flavor asset to be ingested with the output
      - in: query
        name: job[data][flavorParamsId]
        description: Flavor params id to use for conversion
      - in: query
        name: job[data][flavorParamsOutputId]
      - in: query
        name: job[data][flavorParamsOutput][anamorphicPixels]
      - in: query
        name: job[data][flavorParamsOutput][aspectRatioProcessingMode]
      - in: query
        name: job[data][flavorParamsOutput][audioBitrate]
        description: The audio bitrate (in KBits) of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][audioChannels]
        description: The number of audio channels for downmixing
      - in: query
        name: job[data][flavorParamsOutput][audioCodec]
        description: 'Enum Type: `KalturaAudioCodec`The audio codec of the Flavor
          Params'
      - in: query
        name: job[data][flavorParamsOutput][audioSampleRate]
        description: The audio sample rate of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][clipDuration]
      - in: query
        name: job[data][flavorParamsOutput][clipOffset]
      - in: query
        name: job[data][flavorParamsOutput][commandLinesStr]
      - in: query
        name: job[data][flavorParamsOutput][contentAwareness]
      - in: query
        name: job[data][flavorParamsOutput][conversionEnginesExtraParams]
        description: The list of conversion engines extra params (separated with |)
      - in: query
        name: job[data][flavorParamsOutput][conversionEngines]
        description: The list of conversion engines (comma separated)
      - in: query
        name: job[data][flavorParamsOutput][deinterlice]
      - in: query
        name: job[data][flavorParamsOutput][densityHeight]
      - in: query
        name: job[data][flavorParamsOutput][densityWidth]
      - in: query
        name: job[data][flavorParamsOutput][depth]
      - in: query
        name: job[data][flavorParamsOutput][description]
        description: The description of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][engineVersion]
      - in: query
        name: job[data][flavorParamsOutput][flashVersion]
      - in: query
        name: job[data][flavorParamsOutput][flavorAssetId]
      - in: query
        name: job[data][flavorParamsOutput][flavorAssetVersion]
      - in: query
        name: job[data][flavorParamsOutput][flavorParamsId]
      - in: query
        name: job[data][flavorParamsOutput][flavorParamsVersion]
      - in: query
        name: job[data][flavorParamsOutput][forcedKeyFramesMode]
      - in: query
        name: job[data][flavorParamsOutput][forceFrameToMultiplication16]
      - in: query
        name: job[data][flavorParamsOutput][format]
        description: 'Enum Type: `KalturaContainerFormat`The container format of the
          Flavor Params'
      - in: query
        name: job[data][flavorParamsOutput][frameRate]
        description: The frame rate of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][gopSize]
        description: The gop size of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][height]
        description: The desired height of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][isAvoidForcedKeyFrames]
      - in: query
        name: job[data][flavorParamsOutput][isAvoidVideoShrinkBitrateToSource]
      - in: query
        name: job[data][flavorParamsOutput][isAvoidVideoShrinkFramesizeToSource]
      - in: query
        name: job[data][flavorParamsOutput][isCropIMX]
      - in: query
        name: job[data][flavorParamsOutput][isEncrypted]
      - in: query
        name: job[data][flavorParamsOutput][isGopInSec]
      - in: query
        name: job[data][flavorParamsOutput][isVideoFrameRateForLowBrAppleHls]
      - in: query
        name: job[data][flavorParamsOutput][maxFrameRate]
      - in: query
        name: job[data][flavorParamsOutput][mediaParserType]
        description: 'Enum Type: `KalturaMediaParserType`Media parser type to be used
          for post-conversion validation'
      - in: query
        name: job[data][flavorParamsOutput][multiStream]
      - in: query
        name: job[data][flavorParamsOutput][name]
        description: The name of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][objectType]
      - in: query
        name: job[data][flavorParamsOutput][operators]
      - in: query
        name: job[data][flavorParamsOutput][optimizationPolicy]
      - in: query
        name: job[data][flavorParamsOutput][partnerId]
      - in: query
        name: job[data][flavorParamsOutput][poly2Bitmap]
      - in: query
        name: job[data][flavorParamsOutput][readonly]
      - in: query
        name: job[data][flavorParamsOutput][readyBehavior]
      - in: query
        name: job[data][flavorParamsOutput][remoteStorageProfileIds]
        description: Comma seperated ids of remote storage profiles that the flavor
          distributed to, the distribution done by the conversion engine
      - in: query
        name: job[data][flavorParamsOutput][requiredPermissions]
      - in: query
        name: job[data][flavorParamsOutput][rotate]
      - in: query
        name: job[data][flavorParamsOutput][sizeHeight]
      - in: query
        name: job[data][flavorParamsOutput][sizeWidth]
      - in: query
        name: job[data][flavorParamsOutput][sourceAssetParamsIds]
        description: Comma seperated ids of source flavor params this flavor is created
          from
      - in: query
        name: job[data][flavorParamsOutput][sourceRemoteStorageProfileId]
        description: Id of remote storage profile that used to get the source, zero
          indicates Kaltura data center
      - in: query
        name: job[data][flavorParamsOutput][subtitlesData]
      - in: query
        name: job[data][flavorParamsOutput][systemName]
        description: System name of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][tags]
        description: The Flavor Params tags are used to identify the flavor for different
          usage (e
      - in: query
        name: job[data][flavorParamsOutput][twoPass]
      - in: query
        name: job[data][flavorParamsOutput][videoBitrateTolerance]
      - in: query
        name: job[data][flavorParamsOutput][videoBitrate]
        description: The video bitrate (in KBits) of the Flavor Params
      - in: query
        name: job[data][flavorParamsOutput][videoCodec]
        description: 'Enum Type: `KalturaVideoCodec`The video codec of the Flavor
          Params'
      - in: query
        name: job[data][flavorParamsOutput][videoConstantBitrate]
      - in: query
        name: job[data][flavorParamsOutput][watermarkData]
      - in: query
        name: job[data][flavorParamsOutput][widevineDistributionEndDate]
        description: License distribution window end date
      - in: query
        name: job[data][flavorParamsOutput][widevineDistributionStartDate]
        description: License distribution window start date
      - in: query
        name: job[data][flavorParamsOutput][width]
        description: The desired width of the Flavor Params
      - in: query
        name: job[data][flavors]
      - in: query
        name: job[data][force]
      - in: query
        name: job[data][fromEmail]
      - in: query
        name: job[data][fromName]
      - in: query
        name: job[data][fromPartnerId]
        description: Id of the partner to copy from
      - in: query
        name: job[data][ftpPassiveMode]
      - in: query
        name: job[data][inputFileSyncLocalPath]
      - in: query
        name: job[data][inputXmlLocalPath]
      - in: query
        name: job[data][inputXmlRemoteUrl]
      - in: query
        name: job[data][isHtml]
      - in: query
        name: job[data][keepDistributionItem]
        description: Flag signifying that the associated distribution item should
          not be moved to removed status
      - in: query
        name: job[data][ksType]
        description: 'Enum Type: `KalturaSessionType`'
      - in: query
        name: job[data][language]
        description: 'Enum Type: `KalturaLanguageCode`'
      - in: query
        name: job[data][lastCuePointSyncTime]
        description: last live to vod sync time
      - in: query
        name: job[data][lastMovedCategoryEntryPageIndex]
        description: Saves the last page index of the category entries filter pager     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][lastMovedCategoryId]
        description: Saves the last category id that its entries moved completely     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][lastMovedCategoryPageIndex]
        description: Saves the last page index of the child categories filter pager     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][lastSegmentDrift]
        description: last segment drift
      - in: query
        name: job[data][lastSegmentDuration]
        description: last Segment Duration
      - in: query
        name: job[data][lastUpdatedCategoryCreatedAt]
        description: Saves the last sub category creation date that was updated     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][lastUpdatedCategoryEntryCreatedAt]
        description: Saves the last category entry creation date that was updated     In
          case of crash the batch will restart from that point
      - in: query
        name: job[data][liveEntryId]
        description: live Entry Id
      - in: query
        name: job[data][localFileSyncPath]
      - in: query
        name: job[data][logFileSyncLocalPath]
      - in: query
        name: job[data][logFileSyncRemoteUrl]
      - in: query
        name: job[data][mailPriority]
      - in: query
        name: job[data][mailType]
        description: 'Enum Type: `KalturaMailType`'
      - in: query
        name: job[data][maxResults]
      - in: query
        name: job[data][mediaServerIndex]
        description: 'Enum Type: `KalturaEntryServerNodeType`Primary or secondary
          media server'
      - in: query
        name: job[data][mediaType]
      - in: query
        name: job[data][metadataId]
      - in: query
        name: job[data][metadataProfileId]
      - in: query
        name: job[data][method]
        description: 'Enum Type: `KalturaHttpNotificationMethod`Request method'
      - in: query
        name: job[data][minSendDate]
      - in: query
        name: job[data][modifiedAttributes]
      - in: query
        name: job[data][monitorSyncCompletion]
      - in: query
        name: job[data][moveFromChildren]
        description: All entries from all child categories will be moved as well
      - in: query
        name: job[data][multiLanaguageCaptionAssetId]
      - in: query
        name: job[data][notificationEmail]
      - in: query
        name: job[data][notificationResult]
      - in: query
        name: job[data][numberOfAttempts]
      - in: query
        name: job[data][objectData][conversionProfileId]
        description: Selected profile id for all bulk entries
      - in: query
        name: job[data][objectData][objectType]
      - in: query
        name: job[data][objectId]
      - in: query
        name: job[data][objectType]
      - in: query
        name: job[data][objType]
        description: 'Enum Type: `KalturaNotificationObjectType`'
      - in: query
        name: job[data][offset]
        description: Clipping offset in seconds
      - in: query
        name: job[data][outputPath]
      - in: query
        name: job[data][parsedSlug]
      - in: query
        name: job[data][parsedUserId]
      - in: query
        name: job[data][passPhrase]
      - in: query
        name: job[data][password]
        description: A password to use for the connection
      - in: query
        name: job[data][plays]
      - in: query
        name: job[data][primaryBroadcastingUrl]
      - in: query
        name: job[data][primaryContact]
      - in: query
        name: job[data][privateKey]
      - in: query
        name: job[data][protocol]
        description: http / https
      - in: query
        name: job[data][providerData][additionalParameters]
        description: additional parameters to send to Cielo24
      - in: query
        name: job[data][providerData][captionAssetFormats]
        description: Caption formats
      - in: query
        name: job[data][providerData][entryId]
        description: Entry ID
      - in: query
        name: job[data][providerData][exampleUrl]
        description: Just an example
      - in: query
        name: job[data][providerData][fidelity]
        description: 'Enum Type: `KalturaCielo24Fidelity`'
      - in: query
        name: job[data][providerData][flavorAssetId]
        description: Flavor ID
      - in: query
        name: job[data][providerData][metadataProfileId]
        description: ID of the metadata profile for the extracted term metadata
      - in: query
        name: job[data][providerData][objectType]
      - in: query
        name: job[data][providerData][priority]
        description: 'Enum Type: `KalturaCielo24Priority`'
      - in: query
        name: job[data][providerData][replaceMediaContent]
        description: should replace remote media content
      - in: query
        name: job[data][providerData][spokenLanguage]
        description: 'Enum Type: `KalturaLanguage`Transcript content language'
      - in: query
        name: job[data][providerData][transcriptAssetId]
        description: ID of the transcript asset
      - in: query
        name: job[data][providerData][transcriptId]
        description: input Transcript-asset ID
      - in: query
        name: job[data][providerData][voicebaseApiKey]
        description: Voicebase API key to fetch transcript tokens
      - in: query
        name: job[data][providerData][voicebaseApiPassword]
        description: Voicebase API password to fetch transcript tokens
      - in: query
        name: job[data][providerType]
        description: 'Enum Type: `KalturaIntegrationProviderType`'
      - in: query
        name: job[data][provisioningParams]
      - in: query
        name: job[data][publicKey]
      - in: query
        name: job[data][puserId]
        description: The id of the requesting user
      - in: query
        name: job[data][recipientEmail]
      - in: query
        name: job[data][recipientId]
        description: kuserId
      - in: query
        name: job[data][recipientName]
      - in: query
        name: job[data][referenceTime]
      - in: query
        name: job[data][remoteMediaId]
      - in: query
        name: job[data][resultsFilePath]
      - in: query
        name: job[data][returnVal]
      - in: query
        name: job[data][rtmp]
      - in: query
        name: job[data][s3Region]
      - in: query
        name: job[data][scanResult]
        description: 'Enum Type: `KalturaVirusScanJobResult`'
      - in: query
        name: job[data][secondaryBroadcastingUrl]
      - in: query
        name: job[data][secondaryContact]
      - in: query
        name: job[data][separator]
      - in: query
        name: job[data][serverPassPhrase]
      - in: query
        name: job[data][serverPassword]
      - in: query
        name: job[data][serverPrivateKey]
      - in: query
        name: job[data][serverPublicKey]
      - in: query
        name: job[data][serverUrl]
      - in: query
        name: job[data][serverUsername]
      - in: query
        name: job[data][server][dc]
        description: The dc of the server
      - in: query
        name: job[data][server][description]
      - in: query
        name: job[data][server][host]
      - in: query
        name: job[data][server][name]
      - in: query
        name: job[data][server][objectType]
      - in: query
        name: job[data][server][password]
      - in: query
        name: job[data][server][port]
      - in: query
        name: job[data][server][protocol]
        description: 'Enum Type: `KalturaActivitiBusinessProcessServerProtocol`'
      - in: query
        name: job[data][server][systemName]
      - in: query
        name: job[data][server][username]
      - in: query
        name: job[data][serviceToken]
      - in: query
        name: job[data][signatureType]
      - in: query
        name: job[data][signSecret]
        description: The secret to sign the notification with
      - in: query
        name: job[data][srcAssetId]
      - in: query
        name: job[data][srcAssetType]
        description: 'Enum Type: `KalturaAssetType`'
      - in: query
        name: job[data][srcCategoryId]
        description: Source category id
      - in: query
        name: job[data][srcFilePath]
        description: The recorded live media
      - in: query
        name: job[data][srcFileSyncId]
      - in: query
        name: job[data][srcFileSyncLocalPath]
      - in: query
        name: job[data][srcFileSyncRemoteUrl]
      - in: query
        name: job[data][srcFileSyncs]
      - in: query
        name: job[data][srcFiles]
      - in: query
        name: job[data][srcFileUrl]
      - in: query
        name: job[data][srcVersion]
      - in: query
        name: job[data][srcXslPath]
      - in: query
        name: job[data][sseKmsKeyId]
      - in: query
        name: job[data][sseType]
      - in: query
        name: job[data][sslCertificatePassword]
        description: The password required to use the certificate
      - in: query
        name: job[data][sslCertificateType]
        description: 'Enum Type: `KalturaHttpNotificationCertificateType`The format
          of the certificate'
      - in: query
        name: job[data][sslCertificate]
        description: SSL certificate to verify the peer with
      - in: query
        name: job[data][sslEngineDefault]
        description: The identifier for the crypto engine used for asymmetric crypto
          operations
      - in: query
        name: job[data][sslEngine]
        description: The identifier for the crypto engine of the private SSL key specified
          in ssl key
      - in: query
        name: job[data][sslKeyPassword]
        description: The secret password needed to use the private SSL key specified
          in ssl key
      - in: query
        name: job[data][sslKeyType]
        description: 'Enum Type: `KalturaHttpNotificationSslKeyType`The key type of
          the private SSL key specified in ssl key - PEM / DER / ENG'
      - in: query
        name: job[data][sslKey]
        description: Private SSL key
      - in: query
        name: job[data][sslVersion]
        description: 'Enum Type: `KalturaHttpNotificationSslVersion`The SSL version
          (2 or 3) to use'
      - in: query
        name: job[data][startObjectKey]
      - in: query
        name: job[data][status]
        description: 'Enum Type: `KalturaMailJobStatus`'
      - in: query
        name: job[data][streamID]
      - in: query
        name: job[data][streamName]
      - in: query
        name: job[data][streamType]
        description: 'Enum Type: `KalturaAkamaiUniversalStreamType`'
      - in: query
        name: job[data][subjectParams]
      - in: query
        name: job[data][syncMode]
        description: 'Enum Type: `KalturaWidevineRepositorySyncMode`'
      - in: query
        name: job[data][systemPassword]
      - in: query
        name: job[data][systemUserName]
      - in: query
        name: job[data][templateId]
      - in: query
        name: job[data][templatePath]
      - in: query
        name: job[data][thumbAssetId]
      - in: query
        name: job[data][thumbBitrate]
        description: The bit rate of last created thumbnail, will be used to comapare
          if this thumbnail is the best we can have
      - in: query
        name: job[data][thumbHeight]
        description: The height of last created thumbnail, will be used to comapare
          if this thumbnail is the best we can have
      - in: query
        name: job[data][thumbOffset]
        description: The position of the thumbnail in the media file
      - in: query
        name: job[data][thumbParamsOutputId]
      - in: query
        name: job[data][thumbPath]
      - in: query
        name: job[data][timeout]
        description: The maximum number of seconds to allow cURL functions to execute
      - in: query
        name: job[data][timeReference]
      - in: query
        name: job[data][timeZoneOffset]
      - in: query
        name: job[data][toPartnerId]
        description: Id of the partner to copy to
      - in: query
        name: job[data][totalVodDuration]
        description: total VOD Duration
      - in: query
        name: job[data][to][categoryUserFilter][categoryDirectMembers]
        description: Return the list of categoryUser that are not inherited from parent
          category - only the direct categoryUsers
      - in: query
        name: job[data][to][categoryUserFilter][categoryFullIdsEqual]
      - in: query
        name: job[data][to][categoryUserFilter][categoryFullIdsStartsWith]
      - in: query
        name: job[data][to][categoryUserFilter][categoryIdEqual]
      - in: query
        name: job[data][to][categoryUserFilter][categoryIdIn]
      - in: query
        name: job[data][to][categoryUserFilter][createdAtGreaterThanOrEqual]
      - in: query
        name: job[data][to][categoryUserFilter][createdAtLessThanOrEqual]
      - in: query
        name: job[data][to][categoryUserFilter][freeText]
        description: Free text search on user id or screen name
      - in: query
        name: job[data][to][categoryUserFilter][orderBy]
      - in: query
        name: job[data][to][categoryUserFilter][permissionLevelEqual]
        description: 'Enum Type: `KalturaCategoryUserPermissionLevel`'
      - in: query
        name: job[data][to][categoryUserFilter][permissionLevelIn]
      - in: query
        name: job[data][to][categoryUserFilter][permissionNamesMatchAnd]
      - in: query
        name: job[data][to][categoryUserFilter][permissionNamesMatchOr]
      - in: query
        name: job[data][to][categoryUserFilter][permissionNamesNotContains]
      - in: query
        name: job[data][to][categoryUserFilter][relatedGroupsByUserId]
        description: Return a list of categoryUser that related to the userId in this
          field by groups
      - in: query
        name: job[data][to][categoryUserFilter][statusEqual]
        description: 'Enum Type: `KalturaCategoryUserStatus`'
      - in: query
        name: job[data][to][categoryUserFilter][statusIn]
      - in: query
        name: job[data][to][categoryUserFilter][updatedAtGreaterThanOrEqual]
      - in: query
        name: job[data][to][categoryUserFilter][updatedAtLessThanOrEqual]
      - in: query
        name: job[data][to][categoryUserFilter][updateMethodEqual]
        description: 'Enum Type: `KalturaUpdateMethodType`'
      - in: query
        name: job[data][to][categoryUserFilter][updateMethodIn]
      - in: query
        name: job[data][to][categoryUserFilter][userIdEqual]
      - in: query
        name: job[data][to][categoryUserFilter][userIdIn]
      - in: query
        name: job[data][to][emailRecipients]
      - in: query
        name: job[data][to][filter][createdAtGreaterThanOrEqual]
      - in: query
        name: job[data][to][filter][createdAtLessThanOrEqual]
      - in: query
        name: job[data][to][filter][emailLike]
      - in: query
        name: job[data][to][filter][emailStartsWith]
      - in: query
        name: job[data][to][filter][firstNameOrLastNameStartsWith]
      - in: query
        name: job[data][to][filter][firstNameStartsWith]
      - in: query
        name: job[data][to][filter][idEqual]
      - in: query
        name: job[data][to][filter][idIn]
      - in: query
        name: job[data][to][filter][idOrScreenNameStartsWith]
      - in: query
        name: job[data][to][filter][isAdminEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: job[data][to][filter][lastNameStartsWith]
      - in: query
        name: job[data][to][filter][loginEnabledEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: job[data][to][filter][objectType]
      - in: query
        name: job[data][to][filter][orderBy]
      - in: query
        name: job[data][to][filter][partnerIdEqual]
      - in: query
        name: job[data][to][filter][permissionNamesMultiLikeAnd]
        description: Permission names filter expression
      - in: query
        name: job[data][to][filter][permissionNamesMultiLikeOr]
        description: Permission names filter expression
      - in: query
        name: job[data][to][filter][roleIdEqual]
      - in: query
        name: job[data][to][filter][roleIdsEqual]
      - in: query
        name: job[data][to][filter][roleIdsIn]
      - in: query
        name: job[data][to][filter][screenNameLike]
      - in: query
        name: job[data][to][filter][screenNameStartsWith]
      - in: query
        name: job[data][to][filter][statusEqual]
        description: 'Enum Type: `KalturaUserStatus`'
      - in: query
        name: job[data][to][filter][statusIn]
      - in: query
        name: job[data][to][filter][tagsMultiLikeAnd]
      - in: query
        name: job[data][to][filter][tagsMultiLikeOr]
      - in: query
        name: job[data][to][filter][typeEqual]
        description: 'Enum Type: `KalturaUserType`'
      - in: query
        name: job[data][to][filter][typeIn]
      - in: query
        name: job[data][to][objectType]
      - in: query
        name: job[data][typeAsString]
      - in: query
        name: job[data][type]
        description: 'Enum Type: `KalturaNotificationType`'
      - in: query
        name: job[data][url]
        description: Remote server URL
      - in: query
        name: job[data][userId]
      - in: query
        name: job[data][username]
        description: A username to use for the connection
      - in: query
        name: job[data][userRoles]
      - in: query
        name: job[data][views]
      - in: query
        name: job[data][virusFoundAction]
        description: 'Enum Type: `KalturaVirusFoundAction`'
      - in: query
        name: job[data][vodEntryId]
        description: $vod Entry Id
      - in: query
        name: job[data][webexHostId]
      - in: query
        name: job[data][wsdlPassword]
      - in: query
        name: job[data][wsdlUsername]
      - in: query
        name: job[data][wvAssetIds]
      - in: query
        name: job[entryId]
      - in: query
        name: job[entryName]
      - in: query
        name: job[jobSubType]
      - in: query
        name: lockKey[batchIndex]
      - in: query
        name: lockKey[schedulerId]
      - in: query
        name: lockKey[workerId]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - UpdateExclusiveJob
  /service/batch/action/updatePartnerLoadTable:
    get:
      summary: Get Service Batch Action Updatepartnerloadtable
      description: batch updatePartnerLoadTable action cleans the partner load table
      operationId: batch.updatePartnerLoadTable
      x-api-path-slug: servicebatchactionupdatepartnerloadtable-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - UpdatePartnerLoadTable
  /service/batchcontrol/action/configLoaded:
    get:
      summary: Get Service Batchcontrol Action Configloaded
      description: batch configLoaded action saves the configuration as loaded by
        a remote scheduler
      operationId: batchcontrol.configLoaded
      x-api-path-slug: servicebatchcontrolactionconfigloaded-get
      parameters:
      - in: query
        name: configParam
        description: The parameter that was loaded
      - in: query
        name: configParamPart
        description: The parameter part that was loaded
      - in: query
        name: configValue
        description: The value that was loaded
      - in: query
        name: No Name
      - in: query
        name: scheduler[configs]
      - in: query
        name: scheduler[configuredId]
        description: The id as configured in the batch config
      - in: query
        name: scheduler[host]
        description: The host name
      - in: query
        name: scheduler[name]
        description: The scheduler name
      - in: query
        name: scheduler[statuses]
      - in: query
        name: scheduler[workers]
      - in: query
        name: workerConfigId
        description: The id of the job that the configuration refers to, not mandatory
          if the configuration refers to the scheduler
      - in: query
        name: workerName
        description: The name of the job that the configuration refers to, not mandatory
          if the configuration refers to the scheduler
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - ConfigLoaded
  /service/batchcontrol/action/getCommand:
    get:
      summary: Get Service Batchcontrol Action Getcommand
      description: batch getCommand action returns the command with its current status
      operationId: batchcontrol.getCommand
      x-api-path-slug: servicebatchcontrolactiongetcommand-get
      parameters:
      - in: query
        name: commandId
        description: The id of the command
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - GetCommand
  /service/batchcontrol/action/getFullStatus:
    get:
      summary: Get Service Batchcontrol Action Getfullstatus
      description: batch getFullStatus action returns the status of all schedulers
        and queues
      operationId: batchcontrol.getFullStatus
      x-api-path-slug: servicebatchcontrolactiongetfullstatus-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - GetFullStatus
  /service/batchcontrol/action/kill:
    get:
      summary: Get Service Batchcontrol Action Kill
      description: batch kill action forces stop og a batch on a remote scheduler
      operationId: batchcontrol.kill
      x-api-path-slug: servicebatchcontrolactionkill-get
      parameters:
      - in: query
        name: adminId
        description: The id of the admin that called the stop
      - in: query
        name: batchIndex
        description: The index of the batch job process to be stopped
      - in: query
        name: cause
        description: The reason it was stopped
      - in: query
        name: No Name
      - in: query
        name: workerId
        description: The id of the job to be stopped
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - Kill
  /service/batchcontrol/action/listCommands:
    get:
      summary: Get Service Batchcontrol Action Listcommands
      description: list batch control commands
      operationId: batchcontrol.listCommands
      x-api-path-slug: servicebatchcontrolactionlistcommands-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[createdByIdEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaControlPanelCommandStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[targetTypeEqual]
        description: 'Enum Type: `KalturaControlPanelCommandTargetType`'
      - in: query
        name: filter[targetTypeIn]
      - in: query
        name: filter[typeEqual]
        description: 'Enum Type: `KalturaControlPanelCommandType`'
      - in: query
        name: filter[typeIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - ListCommands
  /service/batchcontrol/action/listSchedulers:
    get:
      summary: Get Service Batchcontrol Action Listschedulers
      description: list all Schedulers
      operationId: batchcontrol.listSchedulers
      x-api-path-slug: servicebatchcontrolactionlistschedulers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - ListSchedulers
  /service/batchcontrol/action/listWorkers:
    get:
      summary: Get Service Batchcontrol Action Listworkers
      description: list all Workers
      operationId: batchcontrol.listWorkers
      x-api-path-slug: servicebatchcontrolactionlistworkers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - ListWorkers
  /service/batchcontrol/action/reportStatus:
    get:
      summary: Get Service Batchcontrol Action Reportstatus
      description: batch reportStatus action saves the a status attribute from a remote
        scheduler and returns pending commands for the scheduler
      operationId: batchcontrol.reportStatus
      x-api-path-slug: servicebatchcontrolactionreportstatus-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: scheduler[configs]
      - in: query
        name: scheduler[configuredId]
        description: The id as configured in the batch config
      - in: query
        name: scheduler[host]
        description: The host name
      - in: query
        name: scheduler[name]
        description: The scheduler name
      - in: query
        name: scheduler[statuses]
      - in: query
        name: scheduler[workers]
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - ReportStatus
  /service/batchcontrol/action/setCommandResult:
    get:
      summary: Get Service Batchcontrol Action Setcommandresult
      description: batch setCommandResult action saves the results of a command as
        recieved from a remote scheduler
      operationId: batchcontrol.setCommandResult
      x-api-path-slug: servicebatchcontrolactionsetcommandresult-get
      parameters:
      - in: query
        name: commandId
        description: The id of the command
      - in: query
        name: errorDescription
        description: The description, important for failed commands
      - in: query
        name: No Name
      - in: query
        name: status
        description: 'Enum Type: `KalturaControlPanelCommandStatus`The status of the
          command'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - SetCommandResult
  /service/batchcontrol/action/setSchedulerConfig:
    get:
      summary: Get Service Batchcontrol Action Setschedulerconfig
      description: batch sets a configuration parameter to be loaded by a scheduler
      operationId: batchcontrol.setSchedulerConfig
      x-api-path-slug: servicebatchcontrolactionsetschedulerconfig-get
      parameters:
      - in: query
        name: adminId
        description: The id of the admin that called the setConfig
      - in: query
        name: cause
        description: The reason it was changed
      - in: query
        name: configParam
        description: The parameter to be set
      - in: query
        name: configParamPart
        description: The parameter part to be set - for additional params
      - in: query
        name: configValue
        description: The value to be set
      - in: query
        name: No Name
      - in: query
        name: schedulerId
        description: The id of the remote scheduler location
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - SetSchedulerConfig
  /service/batchcontrol/action/setWorkerConfig:
    get:
      summary: Get Service Batchcontrol Action Setworkerconfig
      description: batch sets a configuration parameter to be loaded by a worker
      operationId: batchcontrol.setWorkerConfig
      x-api-path-slug: servicebatchcontrolactionsetworkerconfig-get
      parameters:
      - in: query
        name: adminId
        description: The id of the admin that called the setConfig
      - in: query
        name: cause
        description: The reason it was changed
      - in: query
        name: configParam
        description: The parameter to be set
      - in: query
        name: configParamPart
        description: The parameter part to be set - for additional params
      - in: query
        name: configValue
        description: The value to be set
      - in: query
        name: No Name
      - in: query
        name: workerId
        description: The id of the job to be configured
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - SetWorkerConfig
  /service/batchcontrol/action/startWorker:
    get:
      summary: Get Service Batchcontrol Action Startworker
      description: batch start action starts a job
      operationId: batchcontrol.startWorker
      x-api-path-slug: servicebatchcontrolactionstartworker-get
      parameters:
      - in: query
        name: adminId
        description: The id of the admin that called the start
      - in: query
        name: cause
        description: The reason it was started
      - in: query
        name: No Name
      - in: query
        name: workerId
        description: The id of the job to be started
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - StartWorker
  /service/batchcontrol/action/stopScheduler:
    get:
      summary: Get Service Batchcontrol Action Stopscheduler
      description: batch stop action stops a scheduler
      operationId: batchcontrol.stopScheduler
      x-api-path-slug: servicebatchcontrolactionstopscheduler-get
      parameters:
      - in: query
        name: adminId
        description: The id of the admin that called the stop
      - in: query
        name: cause
        description: The reason it was stopped
      - in: query
        name: No Name
      - in: query
        name: schedulerId
        description: The id of the remote scheduler location
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - StopScheduler
  /service/batchcontrol/action/stopWorker:
    get:
      summary: Get Service Batchcontrol Action Stopworker
      description: batch stop action stops a worker
      operationId: batchcontrol.stopWorker
      x-api-path-slug: servicebatchcontrolactionstopworker-get
      parameters:
      - in: query
        name: adminId
        description: The id of the admin that called the stop
      - in: query
        name: cause
        description: The reason it was stopped
      - in: query
        name: No Name
      - in: query
        name: workerId
        description: The id of the job to be stopped
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batchcontrol
      - Action
      - StopWorker
  /service/bulkupload/action/abort:
    get:
      summary: Get Service Bulkupload Action Abort
      description: Aborts the bulk upload and all its child jobs
      operationId: bulkUpload.abort
      x-api-path-slug: servicebulkuploadactionabort-get
      parameters:
      - in: query
        name: id
        description: job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Action
      - Abort
  /service/bulkupload/action/add:
    post:
      summary: Post Service Bulkupload Action Add
      description: |-
        Add new bulk upload batch job

        Conversion profile id can be specified in the API or in the CSV file, the one in the CSV file will be stronger.

        If no conversion profile was specified, partner's default will be used
      operationId: bulkUpload.add
      x-api-path-slug: servicebulkuploadactionadd-post
      parameters:
      - in: query
        name: bulkUploadType
        description: 'Enum Type: `KalturaBulkUploadType`'
      - in: query
        name: conversionProfileId
        description: Convertion profile id to use for converting the current bulk
          (-1 to use partners default)
      - in: formData
        name: csvFileData
        description: bulk upload file
      - in: query
        name: fileName
        description: Friendly name of the file, used to be recognized later in the
          logs
      - in: query
        name: No Name
      - in: query
        name: uploadedBy
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Action
      - Add
  /service/bulkupload/action/get:
    get:
      summary: Get Service Bulkupload Action Get
      description: Get bulk upload batch job by id
      operationId: bulkUpload.get
      x-api-path-slug: servicebulkuploadactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Action
      - Get
  /service/bulkupload/action/list:
    get:
      summary: Get Service Bulkupload Action List
      description: List bulk upload batch jobs
      operationId: bulkUpload.list
      x-api-path-slug: servicebulkuploadactionlist-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Action
      - List
  /service/bulkupload/action/serve:
    get:
      summary: Get Service Bulkupload Action Serve
      description: serve action returan the original file.
      operationId: bulkUpload.serve
      x-api-path-slug: servicebulkuploadactionserve-get
      parameters:
      - in: query
        name: id
        description: job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Action
      - Serve
  /service/bulkupload/action/serveLog:
    get:
      summary: Get Service Bulkupload Action Servelog
      description: serveLog action returan the original file.
      operationId: bulkUpload.serveLog
      x-api-path-slug: servicebulkuploadactionservelog-get
      parameters:
      - in: query
        name: id
        description: job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Action
      - ServeLog
  /service/bulkupload_bulk/action/abort:
    get:
      summary: Get Service Bulkupload Bulk Action Abort
      description: Aborts the bulk upload and all its child jobs
      operationId: bulk.abort
      x-api-path-slug: servicebulkupload-bulkactionabort-get
      parameters:
      - in: query
        name: id
        description: job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Bulk
      - Action
      - Abort
  /service/bulkupload_bulk/action/get:
    get:
      summary: Get Service Bulkupload Bulk Action Get
      description: Get bulk upload batch job by id
      operationId: bulk.get
      x-api-path-slug: servicebulkupload-bulkactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Bulk
      - Action
      - Get
  /service/bulkupload_bulk/action/list:
    get:
      summary: Get Service Bulkupload Bulk Action List
      description: List bulk upload batch jobs
      operationId: bulk.list
      x-api-path-slug: servicebulkupload-bulkactionlist-get
      parameters:
      - in: query
        name: bulkUploadFilter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: bulkUploadFilter[advancedSearch][categoriesMatchOr]
      - in: query
        name: bulkUploadFilter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: bulkUploadFilter[advancedSearch][categoryIdEqual]
      - in: query
        name: bulkUploadFilter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: bulkUploadFilter[advancedSearch][contentLike]
      - in: query
        name: bulkUploadFilter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: bulkUploadFilter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: bulkUploadFilter[advancedSearch][cuePointsFreeText]
      - in: query
        name: bulkUploadFilter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: bulkUploadFilter[advancedSearch][cuePointTypeIn]
      - in: query
        name: bulkUploadFilter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: bulkUploadFilter[advancedSearch][distributionProfileId]
      - in: query
        name: bulkUploadFilter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: bulkUploadFilter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: bulkUploadFilter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: bulkUploadFilter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: bulkUploadFilter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: bulkUploadFilter[advancedSearch][extendedStatusIn]
      - in: query
        name: bulkUploadFilter[advancedSearch][field]
      - in: query
        name: bulkUploadFilter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: bulkUploadFilter[advancedSearch][idEqual]
      - in: query
        name: bulkUploadFilter[advancedSearch][idIn]
      - in: query
        name: bulkUploadFilter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: bulkUploadFilter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: bulkUploadFilter[advancedSearch][items]
      - in: query
        name: bulkUploadFilter[advancedSearch][memberIdEq]
      - in: query
        name: bulkUploadFilter[advancedSearch][memberIdIn]
      - in: query
        name: bulkUploadFilter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: bulkUploadFilter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: bulkUploadFilter[advancedSearch][metadataProfileId]
      - in: query
        name: bulkUploadFilter[advancedSearch][noDistributionProfiles]
      - in: query
        name: bulkUploadFilter[advancedSearch][not]
      - in: query
        name: bulkUploadFilter[advancedSearch][objectType]
      - in: query
        name: bulkUploadFilter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: bulkUploadFilter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: bulkUploadFilter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: bulkUploadFilter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: bulkUploadFilter[advancedSearch][userIdEqual]
      - in: query
        name: bulkUploadFilter[advancedSearch][userIdIn]
      - in: query
        name: bulkUploadFilter[advancedSearch][value]
      - in: query
        name: bulkUploadFilter[advancedSearch][watermarkId]
      - in: query
        name: bulkUploadFilter[bulkUploadObjectTypeEqual]
        description: 'Enum Type: `KalturaBulkUploadObjectType`'
      - in: query
        name: bulkUploadFilter[bulkUploadObjectTypeIn]
      - in: query
        name: bulkUploadFilter[orderBy]
      - in: query
        name: bulkUploadFilter[statusEqual]
        description: 'Enum Type: `KalturaBatchJobStatus`'
      - in: query
        name: bulkUploadFilter[statusIn]
      - in: query
        name: bulkUploadFilter[uploadedOnEqual]
      - in: query
        name: bulkUploadFilter[uploadedOnGreaterThanOrEqual]
      - in: query
        name: bulkUploadFilter[uploadedOnLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Bulk
      - Action
      - List
  /service/bulkupload_bulk/action/serve:
    get:
      summary: Get Service Bulkupload Bulk Action Serve
      description: serve action returns the original file.
      operationId: bulk.serve
      x-api-path-slug: servicebulkupload-bulkactionserve-get
      parameters:
      - in: query
        name: id
        description: job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Bulk
      - Action
      - Serve
  /service/bulkupload_bulk/action/serveLog:
    get:
      summary: Get Service Bulkupload Bulk Action Servelog
      description: serveLog action returns the log file for the bulk-upload job.
      operationId: bulk.serveLog
      x-api-path-slug: servicebulkupload-bulkactionservelog-get
      parameters:
      - in: query
        name: id
        description: job id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Bulkupload
      - Bulk
      - Action
      - ServeLog
  /service/businessprocessnotification_businessprocesscase/action/abort:
    get:
      summary: Get Service Businessprocessnotification Businessprocesscase Action
        Abort
      description: Abort business-process case
      operationId: businessProcessCase.abort
      x-api-path-slug: servicebusinessprocessnotification-businessprocesscaseactionabort-get
      parameters:
      - in: query
        name: businessProcessStartNotificationTemplateId
      - in: query
        name: No Name
      - in: query
        name: objectId
      - in: query
        name: objectType
        description: 'Enum Type: `KalturaEventNotificationEventObjectType`'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocesscase
      - Action
      - Abort
  /service/businessprocessnotification_businessprocesscase/action/list:
    get:
      summary: Get Service Businessprocessnotification Businessprocesscase Action
        List
      description: list business-process cases
      operationId: businessProcessCase.list
      x-api-path-slug: servicebusinessprocessnotification-businessprocesscaseactionlist-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: objectId
      - in: query
        name: objectType
        description: 'Enum Type: `KalturaEventNotificationEventObjectType`'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocesscase
      - Action
      - List
  /service/businessprocessnotification_businessprocesscase/action/serveDiagram:
    get:
      summary: Get Service Businessprocessnotification Businessprocesscase Action
        Servediagram
      description: Server business-process case diagram
      operationId: businessProcessCase.serveDiagram
      x-api-path-slug: servicebusinessprocessnotification-businessprocesscaseactionservediagram-get
      parameters:
      - in: query
        name: businessProcessStartNotificationTemplateId
      - in: query
        name: No Name
      - in: query
        name: objectId
      - in: query
        name: objectType
        description: 'Enum Type: `KalturaEventNotificationEventObjectType`'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocesscase
      - Action
      - ServeDiagram
  /service/businessprocessnotification_businessprocessserver/action/add:
    get:
      summary: Get Service Businessprocessnotification Businessprocessserver Action
        Add
      description: Allows you to add a new Business-Process server object
      operationId: businessProcessServer.add
      x-api-path-slug: servicebusinessprocessnotification-businessprocessserveractionadd-get
      parameters:
      - in: query
        name: businessProcessServer[dc]
        description: The dc of the server
      - in: query
        name: businessProcessServer[description]
      - in: query
        name: businessProcessServer[host]
      - in: query
        name: businessProcessServer[name]
      - in: query
        name: businessProcessServer[objectType]
      - in: query
        name: businessProcessServer[password]
      - in: query
        name: businessProcessServer[port]
      - in: query
        name: businessProcessServer[protocol]
        description: 'Enum Type: `KalturaActivitiBusinessProcessServerProtocol`'
      - in: query
        name: businessProcessServer[systemName]
      - in: query
        name: businessProcessServer[username]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocessserver
      - Action
      - Add
  /service/businessprocessnotification_businessprocessserver/action/delete:
    get:
      summary: Get Service Businessprocessnotification Businessprocessserver Action
        Delete
      description: Delete an Business-Process server object
      operationId: businessProcessServer.delete
      x-api-path-slug: servicebusinessprocessnotification-businessprocessserveractiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocessserver
      - Action
      - Delete
  /service/businessprocessnotification_businessprocessserver/action/get:
    get:
      summary: Get Service Businessprocessnotification Businessprocessserver Action
        Get
      description: Retrieve an Business-Process server object by id
      operationId: businessProcessServer.get
      x-api-path-slug: servicebusinessprocessnotification-businessprocessserveractionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocessserver
      - Action
      - Get
  /service/businessprocessnotification_businessprocessserver/action/list:
    get:
      summary: Get Service Businessprocessnotification Businessprocessserver Action
        List
      description: list Business-Process server objects
      operationId: businessProcessServer.list
      x-api-path-slug: servicebusinessprocessnotification-businessprocessserveractionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[currentDcOrExternal]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[currentDc]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[dcEqOrNull]
      - in: query
        name: filter[dcEqual]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[idNotIn]
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaBusinessProcessServerStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[statusNotEqual]
        description: 'Enum Type: `KalturaBusinessProcessServerStatus`'
      - in: query
        name: filter[statusNotIn]
      - in: query
        name: filter[typeEqual]
        description: 'Enum Type: `KalturaBusinessProcessProvider`'
      - in: query
        name: filter[typeIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocessserver
      - Action
      - List
  /service/businessprocessnotification_businessprocessserver/action/update:
    get:
      summary: Get Service Businessprocessnotification Businessprocessserver Action
        Update
      description: Update an existing Business-Process server object
      operationId: businessProcessServer.update
      x-api-path-slug: servicebusinessprocessnotification-businessprocessserveractionupdate-get
      parameters:
      - in: query
        name: businessProcessServer[dc]
        description: The dc of the server
      - in: query
        name: businessProcessServer[description]
      - in: query
        name: businessProcessServer[host]
      - in: query
        name: businessProcessServer[name]
      - in: query
        name: businessProcessServer[objectType]
      - in: query
        name: businessProcessServer[password]
      - in: query
        name: businessProcessServer[port]
      - in: query
        name: businessProcessServer[protocol]
        description: 'Enum Type: `KalturaActivitiBusinessProcessServerProtocol`'
      - in: query
        name: businessProcessServer[systemName]
      - in: query
        name: businessProcessServer[username]
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocessserver
      - Action
      - Update
  /service/businessprocessnotification_businessprocessserver/action/updateStatus:
    get:
      summary: Get Service Businessprocessnotification Businessprocessserver Action
        Updatestatus
      description: Update Business-Process server status by id
      operationId: businessProcessServer.updateStatus
      x-api-path-slug: servicebusinessprocessnotification-businessprocessserveractionupdatestatus-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: status
        description: 'Enum Type: `KalturaBusinessProcessServerStatus`'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Businessprocessnotification
      - Businessprocessserver
      - Action
      - UpdateStatus
  /service/caption_captionasset/action/add:
    get:
      summary: Get Service Caption Captionasset Action Add
      description: Add caption asset
      operationId: captionAsset.add
      x-api-path-slug: servicecaption-captionassetactionadd-get
      parameters:
      - in: query
        name: captionAsset[accuracy]
        description: The Accuracy of the caption content
      - in: query
        name: captionAsset[actualSourceAssetParamsIds]
        description: Comma separated list of source flavor params ids
      - in: query
        name: captionAsset[captionParamsId]
        description: '`insertOnly`The Caption Params used to create this Caption Asset'
      - in: query
        name: captionAsset[fileExt]
        description: '`insertOnly`The file extension'
      - in: query
        name: captionAsset[format]
        description: '`insertOnly`Enum Type: `KalturaCaptionType`The caption format'
      - in: query
        name: captionAsset[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`Is default caption asset
          of the entry'
      - in: query
        name: captionAsset[label]
        description: Friendly label
      - in: query
        name: captionAsset[language]
        description: 'Enum Type: `KalturaLanguage`The language of the caption asset
          content'
      - in: query
        name: captionAsset[parentId]
        description: '`insertOnly`The parent id of the asset'
      - in: query
        name: captionAsset[partnerData]
        description: Partner private data
      - in: query
        name: captionAsset[partnerDescription]
        description: Partner friendly description
      - in: query
        name: captionAsset[tags]
        description: Tags used to identify the Flavor Asset in various scenarios
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - Add
  /service/caption_captionasset/action/delete:
    get:
      summary: Get Service Caption Captionasset Action Delete
      description: ""
      operationId: captionAsset.delete
      x-api-path-slug: servicecaption-captionassetactiondelete-get
      parameters:
      - in: query
        name: captionAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - Delete
  /service/caption_captionasset/action/get:
    get:
      summary: Get Service Caption Captionasset Action Get
      description: ""
      operationId: captionAsset.get
      x-api-path-slug: servicecaption-captionassetactionget-get
      parameters:
      - in: query
        name: captionAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - Get
  /service/caption_captionasset/action/getRemotePaths:
    get:
      summary: Get Service Caption Captionasset Action Getremotepaths
      description: Get remote storage existing paths for the asset
      operationId: captionAsset.getRemotePaths
      x-api-path-slug: servicecaption-captionassetactiongetremotepaths-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - GetRemotePaths
  /service/caption_captionasset/action/getUrl:
    get:
      summary: Get Service Caption Captionasset Action Geturl
      description: Get download URL for the asset
      operationId: captionAsset.getUrl
      x-api-path-slug: servicecaption-captionassetactiongeturl-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: storageId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - GetUrl
  /service/caption_captionasset/action/list:
    get:
      summary: Get Service Caption Captionasset Action List
      description: List caption Assets by filter and pager
      operationId: captionAsset.list
      x-api-path-slug: servicecaption-captionassetactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[captionParamsIdEqual]
      - in: query
        name: filter[captionParamsIdIn]
      - in: query
        name: filter[contentLike]
      - in: query
        name: filter[contentMultiLikeAnd]
      - in: query
        name: filter[contentMultiLikeOr]
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[deletedAtGreaterThanOrEqual]
      - in: query
        name: filter[deletedAtLessThanOrEqual]
      - in: query
        name: filter[endTimeGreaterThanOrEqual]
      - in: query
        name: filter[endTimeLessThanOrEqual]
      - in: query
        name: filter[entryIdEqual]
      - in: query
        name: filter[entryIdIn]
      - in: query
        name: filter[flavorParamsIdEqual]
      - in: query
        name: filter[flavorParamsIdIn]
      - in: query
        name: filter[formatEqual]
        description: 'Enum Type: `KalturaAttachmentType`'
      - in: query
        name: filter[formatIn]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[labelEqual]
      - in: query
        name: filter[labelIn]
      - in: query
        name: filter[languageEqual]
        description: 'Enum Type: `KalturaLanguage`'
      - in: query
        name: filter[languageIn]
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[partnerDescriptionLike]
      - in: query
        name: filter[partnerDescriptionMultiLikeAnd]
      - in: query
        name: filter[partnerDescriptionMultiLikeOr]
      - in: query
        name: filter[partnerIdEqual]
      - in: query
        name: filter[partnerIdIn]
      - in: query
        name: filter[sizeGreaterThanOrEqual]
      - in: query
        name: filter[sizeLessThanOrEqual]
      - in: query
        name: filter[startTimeGreaterThanOrEqual]
      - in: query
        name: filter[startTimeLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaAttachmentAssetStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[statusNotIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[thumbParamsIdEqual]
      - in: query
        name: filter[thumbParamsIdIn]
      - in: query
        name: filter[typeIn]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - List
  /service/caption_captionasset/action/serve:
    get:
      summary: Get Service Caption Captionasset Action Serve
      description: Serves caption by its id
      operationId: captionAsset.serve
      x-api-path-slug: servicecaption-captionassetactionserve-get
      parameters:
      - in: query
        name: captionAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - Serve
  /service/caption_captionasset/action/serveByEntryId:
    get:
      summary: Get Service Caption Captionasset Action Servebyentryid
      description: Serves caption by entry id and thumnail params id
      operationId: captionAsset.serveByEntryId
      x-api-path-slug: servicecaption-captionassetactionservebyentryid-get
      parameters:
      - in: query
        name: captionParamId
        description: if not set, default caption will be used
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - ServeByEntryId
  /service/caption_captionasset/action/serveWebVTT:
    get:
      summary: Get Service Caption Captionasset Action Servewebvtt
      description: Serves caption by its id converting it to segmented WebVTT
      operationId: captionAsset.serveWebVTT
      x-api-path-slug: servicecaption-captionassetactionservewebvtt-get
      parameters:
      - in: query
        name: captionAssetId
      - in: query
        name: localTimestamp
      - in: query
        name: No Name
      - in: query
        name: segmentDuration
      - in: query
        name: segmentIndex
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - ServeWebVTT
  /service/caption_captionasset/action/setAsDefault:
    get:
      summary: Get Service Caption Captionasset Action Setasdefault
      description: Markss the caption as default and removes that mark from all other
        caption assets of the entry.
      operationId: captionAsset.setAsDefault
      x-api-path-slug: servicecaption-captionassetactionsetasdefault-get
      parameters:
      - in: query
        name: captionAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - SetAsDefault
  /service/caption_captionasset/action/setContent:
    post:
      summary: Post Service Caption Captionasset Action Setcontent
      description: Update content of caption asset
      operationId: captionAsset.setContent
      x-api-path-slug: servicecaption-captionassetactionsetcontent-post
      parameters:
      - in: query
        name: contentResource[assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[content]
        description: Textual content
      - in: query
        name: contentResource[dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[objectType]
      - in: query
        name: contentResource[privateKey]
        description: SSH private key
      - in: query
        name: contentResource[publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resources]
      - in: query
        name: contentResource[resource][assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[resource][content]
        description: Textual content
      - in: query
        name: contentResource[resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[resource][entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[resource][objectType]
      - in: query
        name: contentResource[resource][privateKey]
        description: SSH private key
      - in: query
        name: contentResource[resource][publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resource][resources]
      - in: query
        name: contentResource[resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[resource][resource][content]
        description: Textual content
      - in: query
        name: contentResource[resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[resource][resource][objectType]
      - in: query
        name: contentResource[resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: contentResource[resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resource][resource][resources]
      - in: query
        name: contentResource[resource][resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: contentResource[resource][resource][resource][content]
        description: Textual content
      - in: query
        name: contentResource[resource][resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: contentResource[resource][resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: contentResource[resource][resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: contentResource[resource][resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: contentResource[resource][resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: contentResource[resource][resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: contentResource[resource][resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: contentResource[resource][resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: contentResource[resource][resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: contentResource[resource][resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: contentResource[resource][resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: contentResource[resource][resource][resource][objectType]
      - in: query
        name: contentResource[resource][resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: contentResource[resource][resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: contentResource[resource][resource][resource][resources]
      - in: query
        name: contentResource[resource][resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[resource][resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: contentResource[resource][resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[resource][resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: contentResource[resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: contentResource[resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: contentResource[resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[resource][token]
        description: Token that returned from upload
      - in: query
        name: contentResource[resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[resource][version]
        description: The version of the file sync object
      - in: query
        name: contentResource[storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: contentResource[token]
        description: Token that returned from upload
      - in: query
        name: contentResource[url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: contentResource[version]
        description: The version of the file sync object
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - SetContent
  /service/caption_captionasset/action/update:
    get:
      summary: Get Service Caption Captionasset Action Update
      description: Update caption asset
      operationId: captionAsset.update
      x-api-path-slug: servicecaption-captionassetactionupdate-get
      parameters:
      - in: query
        name: captionAsset[accuracy]
        description: The Accuracy of the caption content
      - in: query
        name: captionAsset[actualSourceAssetParamsIds]
        description: Comma separated list of source flavor params ids
      - in: query
        name: captionAsset[captionParamsId]
        description: '`insertOnly`The Caption Params used to create this Caption Asset'
      - in: query
        name: captionAsset[fileExt]
        description: '`insertOnly`The file extension'
      - in: query
        name: captionAsset[format]
        description: '`insertOnly`Enum Type: `KalturaCaptionType`The caption format'
      - in: query
        name: captionAsset[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`Is default caption asset
          of the entry'
      - in: query
        name: captionAsset[label]
        description: Friendly label
      - in: query
        name: captionAsset[language]
        description: 'Enum Type: `KalturaLanguage`The language of the caption asset
          content'
      - in: query
        name: captionAsset[parentId]
        description: '`insertOnly`The parent id of the asset'
      - in: query
        name: captionAsset[partnerData]
        description: Partner private data
      - in: query
        name: captionAsset[partnerDescription]
        description: Partner friendly description
      - in: query
        name: captionAsset[tags]
        description: Tags used to identify the Flavor Asset in various scenarios
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionasset
      - Action
      - Update
  /service/caption_captionparams/action/add:
    get:
      summary: Get Service Caption Captionparams Action Add
      description: Add new Caption Params
      operationId: captionParams.add
      x-api-path-slug: servicecaption-captionparamsactionadd-get
      parameters:
      - in: query
        name: captionParams[description]
        description: The description of the Flavor Params
      - in: query
        name: captionParams[format]
        description: '`insertOnly`Enum Type: `KalturaCaptionType`The caption format'
      - in: query
        name: captionParams[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`Is default caption asset
          of the entry'
      - in: query
        name: captionParams[label]
        description: Friendly label
      - in: query
        name: captionParams[language]
        description: '`insertOnly`Enum Type: `KalturaLanguage`The language of the
          caption content'
      - in: query
        name: captionParams[mediaParserType]
        description: 'Enum Type: `KalturaMediaParserType`Media parser type to be used
          for post-conversion validation'
      - in: query
        name: captionParams[name]
        description: The name of the Flavor Params
      - in: query
        name: captionParams[partnerId]
      - in: query
        name: captionParams[remoteStorageProfileIds]
        description: Comma seperated ids of remote storage profiles that the flavor
          distributed to, the distribution done by the conversion engine
      - in: query
        name: captionParams[requiredPermissions]
      - in: query
        name: captionParams[sourceAssetParamsIds]
        description: Comma seperated ids of source flavor params this flavor is created
          from
      - in: query
        name: captionParams[sourceParamsId]
        description: Id of the caption params or the flavor params to be used as source
          for the caption creation
      - in: query
        name: captionParams[sourceRemoteStorageProfileId]
        description: Id of remote storage profile that used to get the source, zero
          indicates Kaltura data center
      - in: query
        name: captionParams[systemName]
        description: System name of the Flavor Params
      - in: query
        name: captionParams[tags]
        description: The Flavor Params tags are used to identify the flavor for different
          usage (e
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionparams
      - Action
      - Add
  /service/caption_captionparams/action/delete:
    get:
      summary: Get Service Caption Captionparams Action Delete
      description: Delete Caption Params by ID
      operationId: captionParams.delete
      x-api-path-slug: servicecaption-captionparamsactiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionparams
      - Action
      - Delete
  /service/caption_captionparams/action/get:
    get:
      summary: Get Service Caption Captionparams Action Get
      description: Get Caption Params by ID
      operationId: captionParams.get
      x-api-path-slug: servicecaption-captionparamsactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionparams
      - Action
      - Get
  /service/caption_captionparams/action/list:
    get:
      summary: Get Service Caption Captionparams Action List
      description: List Caption Params by filter with paging support (By default -
        all system default params will be listed too)
      operationId: captionParams.list
      x-api-path-slug: servicecaption-captionparamsactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[formatEqual]
        description: 'Enum Type: `KalturaCaptionType`'
      - in: query
        name: filter[formatIn]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[isSystemDefaultEqual]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[systemNameEqual]
      - in: query
        name: filter[systemNameIn]
      - in: query
        name: filter[tagsEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionparams
      - Action
      - List
  /service/caption_captionparams/action/update:
    get:
      summary: Get Service Caption Captionparams Action Update
      description: Update Caption Params by ID
      operationId: captionParams.update
      x-api-path-slug: servicecaption-captionparamsactionupdate-get
      parameters:
      - in: query
        name: captionParams[description]
        description: The description of the Flavor Params
      - in: query
        name: captionParams[format]
        description: '`insertOnly`Enum Type: `KalturaCaptionType`The caption format'
      - in: query
        name: captionParams[isDefault]
        description: 'Enum Type: `KalturaNullableBoolean`Is default caption asset
          of the entry'
      - in: query
        name: captionParams[label]
        description: Friendly label
      - in: query
        name: captionParams[language]
        description: '`insertOnly`Enum Type: `KalturaLanguage`The language of the
          caption content'
      - in: query
        name: captionParams[mediaParserType]
        description: 'Enum Type: `KalturaMediaParserType`Media parser type to be used
          for post-conversion validation'
      - in: query
        name: captionParams[name]
        description: The name of the Flavor Params
      - in: query
        name: captionParams[partnerId]
      - in: query
        name: captionParams[remoteStorageProfileIds]
        description: Comma seperated ids of remote storage profiles that the flavor
          distributed to, the distribution done by the conversion engine
      - in: query
        name: captionParams[requiredPermissions]
      - in: query
        name: captionParams[sourceAssetParamsIds]
        description: Comma seperated ids of source flavor params this flavor is created
          from
      - in: query
        name: captionParams[sourceParamsId]
        description: Id of the caption params or the flavor params to be used as source
          for the caption creation
      - in: query
        name: captionParams[sourceRemoteStorageProfileId]
        description: Id of remote storage profile that used to get the source, zero
          indicates Kaltura data center
      - in: query
        name: captionParams[systemName]
        description: System name of the Flavor Params
      - in: query
        name: captionParams[tags]
        description: The Flavor Params tags are used to identify the flavor for different
          usage (e
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Caption
      - Captionparams
      - Action
      - Update
  /service/captionsearch_captionassetitem/action/parse:
    get:
      summary: Get Service Captionsearch Captionassetitem Action Parse
      description: Parse content of caption asset and index it
      operationId: captionAssetItem.parse
      x-api-path-slug: servicecaptionsearch-captionassetitemactionparse-get
      parameters:
      - in: query
        name: captionAssetId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Captionsearch
      - Captionassetitem
      - Action
      - Parse
  /service/captionsearch_captionassetitem/action/search:
    get:
      summary: Get Service Captionsearch Captionassetitem Action Search
      description: Search caption asset items by filter, pager and free text
      operationId: captionAssetItem.search
      x-api-path-slug: servicecaptionsearch-captionassetitemactionsearch-get
      parameters:
      - in: query
        name: captionAssetItemFilter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][categoriesMatchOr]
      - in: query
        name: captionAssetItemFilter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][categoryIdEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][contentLike]
      - in: query
        name: captionAssetItemFilter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[advancedSearch][cuePointsFreeText]
      - in: query
        name: captionAssetItemFilter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][cuePointTypeIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][distributionProfileId]
      - in: query
        name: captionAssetItemFilter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: captionAssetItemFilter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][extendedStatusIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][field]
      - in: query
        name: captionAssetItemFilter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: captionAssetItemFilter[advancedSearch][idEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][idIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: captionAssetItemFilter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][items]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberIdEq]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberIdIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: captionAssetItemFilter[advancedSearch][metadataProfileId]
      - in: query
        name: captionAssetItemFilter[advancedSearch][noDistributionProfiles]
      - in: query
        name: captionAssetItemFilter[advancedSearch][not]
      - in: query
        name: captionAssetItemFilter[advancedSearch][objectType]
      - in: query
        name: captionAssetItemFilter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][userIdEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][userIdIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][value]
      - in: query
        name: captionAssetItemFilter[advancedSearch][watermarkId]
      - in: query
        name: captionAssetItemFilter[captionParamsIdEqual]
      - in: query
        name: captionAssetItemFilter[captionParamsIdIn]
      - in: query
        name: captionAssetItemFilter[contentLike]
      - in: query
        name: captionAssetItemFilter[contentMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[contentMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[createdAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[createdAtLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[deletedAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[deletedAtLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[endTimeGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[endTimeLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[entryIdEqual]
      - in: query
        name: captionAssetItemFilter[entryIdIn]
      - in: query
        name: captionAssetItemFilter[formatEqual]
        description: 'Enum Type: `KalturaCaptionType`'
      - in: query
        name: captionAssetItemFilter[formatIn]
      - in: query
        name: captionAssetItemFilter[idEqual]
      - in: query
        name: captionAssetItemFilter[idIn]
      - in: query
        name: captionAssetItemFilter[labelEqual]
      - in: query
        name: captionAssetItemFilter[labelIn]
      - in: query
        name: captionAssetItemFilter[languageEqual]
        description: 'Enum Type: `KalturaLanguage`'
      - in: query
        name: captionAssetItemFilter[languageIn]
      - in: query
        name: captionAssetItemFilter[orderBy]
      - in: query
        name: captionAssetItemFilter[partnerDescriptionLike]
      - in: query
        name: captionAssetItemFilter[partnerDescriptionMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[partnerDescriptionMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[partnerIdEqual]
      - in: query
        name: captionAssetItemFilter[partnerIdIn]
      - in: query
        name: captionAssetItemFilter[sizeGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[sizeLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[startTimeGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[startTimeLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[statusEqual]
        description: 'Enum Type: `KalturaCaptionAssetStatus`'
      - in: query
        name: captionAssetItemFilter[statusIn]
      - in: query
        name: captionAssetItemFilter[statusNotIn]
      - in: query
        name: captionAssetItemFilter[tagsLike]
      - in: query
        name: captionAssetItemFilter[tagsMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[tagsMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[typeIn]
      - in: query
        name: captionAssetItemFilter[updatedAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[updatedAtLessThanOrEqual]
      - in: query
        name: captionAssetItemPager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: captionAssetItemPager[pageSize]
        description: The number of objects to retrieve
      - in: query
        name: entryFilter[accessControlIdEqual]
      - in: query
        name: entryFilter[accessControlIdIn]
      - in: query
        name: entryFilter[adminTagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[adminTagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[adminTagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: entryFilter[advancedSearch][categoriesMatchOr]
      - in: query
        name: entryFilter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: entryFilter[advancedSearch][categoryIdEqual]
      - in: query
        name: entryFilter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: entryFilter[advancedSearch][contentLike]
      - in: query
        name: entryFilter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: entryFilter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: entryFilter[advancedSearch][cuePointsFreeText]
      - in: query
        name: entryFilter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: entryFilter[advancedSearch][cuePointTypeIn]
      - in: query
        name: entryFilter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: entryFilter[advancedSearch][distributionProfileId]
      - in: query
        name: entryFilter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: entryFilter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: entryFilter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: entryFilter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: entryFilter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: entryFilter[advancedSearch][extendedStatusIn]
      - in: query
        name: entryFilter[advancedSearch][field]
      - in: query
        name: entryFilter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: entryFilter[advancedSearch][idEqual]
      - in: query
        name: entryFilter[advancedSearch][idIn]
      - in: query
        name: entryFilter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: entryFilter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[advancedSearch][items]
      - in: query
        name: entryFilter[advancedSearch][memberIdEq]
      - in: query
        name: entryFilter[advancedSearch][memberIdIn]
      - in: query
        name: entryFilter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: entryFilter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: entryFilter[advancedSearch][metadataProfileId]
      - in: query
        name: entryFilter[advancedSearch][noDistributionProfiles]
      - in: query
        name: entryFilter[advancedSearch][not]
      - in: query
        name: entryFilter[advancedSearch][objectType]
      - in: query
        name: entryFilter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: entryFilter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: entryFilter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: entryFilter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: entryFilter[advancedSearch][userIdEqual]
      - in: query
        name: entryFilter[advancedSearch][userIdIn]
      - in: query
        name: entryFilter[advancedSearch][value]
      - in: query
        name: entryFilter[advancedSearch][watermarkId]
      - in: query
        name: entryFilter[assetParamsIdsMatchAnd]
      - in: query
        name: entryFilter[assetParamsIdsMatchOr]
      - in: query
        name: entryFilter[categoriesFullNameIn]
      - in: query
        name: entryFilter[categoriesIdsEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[categoriesIdsMatchAnd]
      - in: query
        name: entryFilter[categoriesIdsMatchOr]
        description: All entries of the categories, excluding their child categories
      - in: query
        name: entryFilter[categoriesIdsNotContains]
      - in: query
        name: entryFilter[categoriesMatchAnd]
      - in: query
        name: entryFilter[categoriesMatchOr]
        description: All entries within these categories or their child categories
      - in: query
        name: entryFilter[categoriesNotContains]
      - in: query
        name: entryFilter[categoryAncestorIdIn]
        description: All entries within this categoy or in child categories
      - in: query
        name: entryFilter[createdAtGreaterThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system after a specific time/date (standard
          timestamp format)
      - in: query
        name: entryFilter[createdAtLessThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system before a specific time/date (standard
          timestamp format)
      - in: query
        name: entryFilter[creatorIdEqual]
      - in: query
        name: entryFilter[documentTypeEqual]
        description: 'Enum Type: `KalturaDocumentType`'
      - in: query
        name: entryFilter[documentTypeIn]
      - in: query
        name: entryFilter[durationGreaterThanOrEqual]
      - in: query
        name: entryFilter[durationGreaterThan]
      - in: query
        name: entryFilter[durationLessThanOrEqual]
      - in: query
        name: entryFilter[durationLessThan]
      - in: query
        name: entryFilter[durationTypeMatchOr]
      - in: query
        name: entryFilter[endDateGreaterThanOrEqualOrNull]
      - in: query
        name: entryFilter[endDateGreaterThanOrEqual]
      - in: query
        name: entryFilter[endDateLessThanOrEqualOrNull]
      - in: query
        name: entryFilter[endDateLessThanOrEqual]
      - in: query
        name: entryFilter[entitledUsersEditMatchAnd]
      - in: query
        name: entryFilter[entitledUsersEditMatchOr]
      - in: query
        name: entryFilter[entitledUsersPublishMatchAnd]
      - in: query
        name: entryFilter[entitledUsersPublishMatchOr]
      - in: query
        name: entryFilter[externalSourceTypeEqual]
        description: 'Enum Type: `KalturaExternalMediaSourceType`'
      - in: query
        name: entryFilter[externalSourceTypeIn]
      - in: query
        name: entryFilter[flavorParamsIdsMatchAnd]
      - in: query
        name: entryFilter[flavorParamsIdsMatchOr]
      - in: query
        name: entryFilter[freeText]
      - in: query
        name: entryFilter[groupIdEqual]
      - in: query
        name: entryFilter[hasMediaServerHostname]
      - in: query
        name: entryFilter[idEqual]
        description: This filter should be in use for retrieving only a specific entry
          (identified by its entryId)
      - in: query
        name: entryFilter[idIn]
        description: This filter should be in use for retrieving few specific entries
          (string should include comma separated list of entryId strings)
      - in: query
        name: entryFilter[idNotIn]
      - in: query
        name: entryFilter[isLive]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[isRecordedEntryIdEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[isRoot]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[lastPlayedAtGreaterThanOrEqual]
      - in: query
        name: entryFilter[lastPlayedAtLessThanOrEqual]
      - in: query
        name: entryFilter[limit]
      - in: query
        name: entryFilter[mediaDateGreaterThanOrEqual]
      - in: query
        name: entryFilter[mediaDateLessThanOrEqual]
      - in: query
        name: entryFilter[mediaTypeEqual]
        description: 'Enum Type: `KalturaMediaType`'
      - in: query
        name: entryFilter[mediaTypeIn]
      - in: query
        name: entryFilter[moderationStatusEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: entryFilter[moderationStatusIn]
      - in: query
        name: entryFilter[moderationStatusNotEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: entryFilter[moderationStatusNotIn]
      - in: query
        name: entryFilter[nameEqual]
        description: This filter should be in use for retrieving entries with a specific
          name
      - in: query
        name: entryFilter[nameLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[nameMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[nameMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[objectType]
      - in: query
        name: entryFilter[orderBy]
      - in: query
        name: entryFilter[parentEntryIdEqual]
      - in: query
        name: entryFilter[partnerIdEqual]
        description: This filter should be in use for retrieving only entries which
          were uploaded by/assigned to users of a specific Kaltura Partner (identified
          by Partner ID)
      - in: query
        name: entryFilter[partnerIdIn]
        description: This filter should be in use for retrieving only entries within
          Kaltura network which were uploaded by/assigned to users of few Kaltura
          Partners  (string should include comma separated list of PartnerIDs)
      - in: query
        name: entryFilter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: entryFilter[partnerSortValueLessThanOrEqual]
      - in: query
        name: entryFilter[redirectFromEntryId]
        description: The id of the original entry
      - in: query
        name: entryFilter[referenceIdEqual]
      - in: query
        name: entryFilter[referenceIdIn]
      - in: query
        name: entryFilter[replacedEntryIdEqual]
      - in: query
        name: entryFilter[replacedEntryIdIn]
      - in: query
        name: entryFilter[replacementStatusEqual]
        description: 'Enum Type: `KalturaEntryReplacementStatus`'
      - in: query
        name: entryFilter[replacementStatusIn]
      - in: query
        name: entryFilter[replacingEntryIdEqual]
      - in: query
        name: entryFilter[replacingEntryIdIn]
      - in: query
        name: entryFilter[rootEntryIdEqual]
      - in: query
        name: entryFilter[rootEntryIdIn]
      - in: query
        name: entryFilter[searchTextMatchAnd]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within all of the following metadata
          attributes: name, description, tags, adminTags'
      - in: query
        name: entryFilter[searchTextMatchOr]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within at least one of the following
          metadata attributes: name, description, tags, adminTags'
      - in: query
        name: entryFilter[sourceTypeEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: entryFilter[sourceTypeIn]
      - in: query
        name: entryFilter[sourceTypeNotEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: entryFilter[sourceTypeNotIn]
      - in: query
        name: entryFilter[startDateGreaterThanOrEqualOrNull]
      - in: query
        name: entryFilter[startDateGreaterThanOrEqual]
      - in: query
        name: entryFilter[startDateLessThanOrEqualOrNull]
      - in: query
        name: entryFilter[startDateLessThanOrEqual]
      - in: query
        name: entryFilter[statusEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, at a specific {'
      - in: query
        name: entryFilter[statusIn]
        description: This filter should be in use for retrieving only entries, at
          few specific {
      - in: query
        name: entryFilter[statusNotEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, not at a specific {'
      - in: query
        name: entryFilter[statusNotIn]
        description: This filter should be in use for retrieving only entries, not
          at few specific {
      - in: query
        name: entryFilter[tagsAdminTagsMultiLikeAnd]
      - in: query
        name: entryFilter[tagsAdminTagsMultiLikeOr]
      - in: query
        name: entryFilter[tagsAdminTagsNameMultiLikeAnd]
      - in: query
        name: entryFilter[tagsAdminTagsNameMultiLikeOr]
      - in: query
        name: entryFilter[tagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[tagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[tagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[tagsNameMultiLikeAnd]
      - in: query
        name: entryFilter[tagsNameMultiLikeOr]
      - in: query
        name: entryFilter[totalRankGreaterThanOrEqual]
      - in: query
        name: entryFilter[totalRankLessThanOrEqual]
      - in: query
        name: entryFilter[typeEqual]
        description: 'Enum Type: `KalturaEntryType`'
      - in: query
        name: entryFilter[typeIn]
        description: This filter should be in use for retrieving entries of few {
      - in: query
        name: entryFilter[updatedAtGreaterThanOrEqual]
      - in: query
        name: entryFilter[updatedAtLessThanOrEqual]
      - in: query
        name: entryFilter[userIdEqual]
        description: This filter parameter should be in use for retrieving only entries,
          uploaded by/assigned to a specific user (identified by user Id)
      - in: query
        name: entryFilter[userIdIn]
      - in: query
        name: entryFilter[userIdNotIn]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Captionsearch
      - Captionassetitem
      - Action
      - Search
  /service/captionsearch_captionassetitem/action/searchEntries:
    get:
      summary: Get Service Captionsearch Captionassetitem Action Searchentries
      description: Search caption asset items by filter, pager and free text
      operationId: captionAssetItem.searchEntries
      x-api-path-slug: servicecaptionsearch-captionassetitemactionsearchentries-get
      parameters:
      - in: query
        name: captionAssetItemFilter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][categoriesMatchOr]
      - in: query
        name: captionAssetItemFilter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][categoryIdEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][contentLike]
      - in: query
        name: captionAssetItemFilter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[advancedSearch][cuePointsFreeText]
      - in: query
        name: captionAssetItemFilter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][cuePointTypeIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][distributionProfileId]
      - in: query
        name: captionAssetItemFilter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: captionAssetItemFilter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][extendedStatusIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][field]
      - in: query
        name: captionAssetItemFilter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: captionAssetItemFilter[advancedSearch][idEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][idIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: captionAssetItemFilter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][items]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberIdEq]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberIdIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: captionAssetItemFilter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: captionAssetItemFilter[advancedSearch][metadataProfileId]
      - in: query
        name: captionAssetItemFilter[advancedSearch][noDistributionProfiles]
      - in: query
        name: captionAssetItemFilter[advancedSearch][not]
      - in: query
        name: captionAssetItemFilter[advancedSearch][objectType]
      - in: query
        name: captionAssetItemFilter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: captionAssetItemFilter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][userIdEqual]
      - in: query
        name: captionAssetItemFilter[advancedSearch][userIdIn]
      - in: query
        name: captionAssetItemFilter[advancedSearch][value]
      - in: query
        name: captionAssetItemFilter[advancedSearch][watermarkId]
      - in: query
        name: captionAssetItemFilter[captionParamsIdEqual]
      - in: query
        name: captionAssetItemFilter[captionParamsIdIn]
      - in: query
        name: captionAssetItemFilter[contentLike]
      - in: query
        name: captionAssetItemFilter[contentMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[contentMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[createdAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[createdAtLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[deletedAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[deletedAtLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[endTimeGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[endTimeLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[entryIdEqual]
      - in: query
        name: captionAssetItemFilter[entryIdIn]
      - in: query
        name: captionAssetItemFilter[formatEqual]
        description: 'Enum Type: `KalturaCaptionType`'
      - in: query
        name: captionAssetItemFilter[formatIn]
      - in: query
        name: captionAssetItemFilter[idEqual]
      - in: query
        name: captionAssetItemFilter[idIn]
      - in: query
        name: captionAssetItemFilter[labelEqual]
      - in: query
        name: captionAssetItemFilter[labelIn]
      - in: query
        name: captionAssetItemFilter[languageEqual]
        description: 'Enum Type: `KalturaLanguage`'
      - in: query
        name: captionAssetItemFilter[languageIn]
      - in: query
        name: captionAssetItemFilter[orderBy]
      - in: query
        name: captionAssetItemFilter[partnerDescriptionLike]
      - in: query
        name: captionAssetItemFilter[partnerDescriptionMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[partnerDescriptionMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[partnerIdEqual]
      - in: query
        name: captionAssetItemFilter[partnerIdIn]
      - in: query
        name: captionAssetItemFilter[sizeGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[sizeLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[startTimeGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[startTimeLessThanOrEqual]
      - in: query
        name: captionAssetItemFilter[statusEqual]
        description: 'Enum Type: `KalturaCaptionAssetStatus`'
      - in: query
        name: captionAssetItemFilter[statusIn]
      - in: query
        name: captionAssetItemFilter[statusNotIn]
      - in: query
        name: captionAssetItemFilter[tagsLike]
      - in: query
        name: captionAssetItemFilter[tagsMultiLikeAnd]
      - in: query
        name: captionAssetItemFilter[tagsMultiLikeOr]
      - in: query
        name: captionAssetItemFilter[typeIn]
      - in: query
        name: captionAssetItemFilter[updatedAtGreaterThanOrEqual]
      - in: query
        name: captionAssetItemFilter[updatedAtLessThanOrEqual]
      - in: query
        name: captionAssetItemPager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: captionAssetItemPager[pageSize]
        description: The number of objects to retrieve
      - in: query
        name: entryFilter[accessControlIdEqual]
      - in: query
        name: entryFilter[accessControlIdIn]
      - in: query
        name: entryFilter[adminTagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[adminTagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[adminTagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: entryFilter[advancedSearch][categoriesMatchOr]
      - in: query
        name: entryFilter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: entryFilter[advancedSearch][categoryIdEqual]
      - in: query
        name: entryFilter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: entryFilter[advancedSearch][contentLike]
      - in: query
        name: entryFilter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: entryFilter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: entryFilter[advancedSearch][cuePointsFreeText]
      - in: query
        name: entryFilter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: entryFilter[advancedSearch][cuePointTypeIn]
      - in: query
        name: entryFilter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: entryFilter[advancedSearch][distributionProfileId]
      - in: query
        name: entryFilter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: entryFilter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: entryFilter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: entryFilter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: entryFilter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: entryFilter[advancedSearch][extendedStatusIn]
      - in: query
        name: entryFilter[advancedSearch][field]
      - in: query
        name: entryFilter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: entryFilter[advancedSearch][idEqual]
      - in: query
        name: entryFilter[advancedSearch][idIn]
      - in: query
        name: entryFilter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: entryFilter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[advancedSearch][items]
      - in: query
        name: entryFilter[advancedSearch][memberIdEq]
      - in: query
        name: entryFilter[advancedSearch][memberIdIn]
      - in: query
        name: entryFilter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: entryFilter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: entryFilter[advancedSearch][metadataProfileId]
      - in: query
        name: entryFilter[advancedSearch][noDistributionProfiles]
      - in: query
        name: entryFilter[advancedSearch][not]
      - in: query
        name: entryFilter[advancedSearch][objectType]
      - in: query
        name: entryFilter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: entryFilter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: entryFilter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: entryFilter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: entryFilter[advancedSearch][userIdEqual]
      - in: query
        name: entryFilter[advancedSearch][userIdIn]
      - in: query
        name: entryFilter[advancedSearch][value]
      - in: query
        name: entryFilter[advancedSearch][watermarkId]
      - in: query
        name: entryFilter[assetParamsIdsMatchAnd]
      - in: query
        name: entryFilter[assetParamsIdsMatchOr]
      - in: query
        name: entryFilter[categoriesFullNameIn]
      - in: query
        name: entryFilter[categoriesIdsEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[categoriesIdsMatchAnd]
      - in: query
        name: entryFilter[categoriesIdsMatchOr]
        description: All entries of the categories, excluding their child categories
      - in: query
        name: entryFilter[categoriesIdsNotContains]
      - in: query
        name: entryFilter[categoriesMatchAnd]
      - in: query
        name: entryFilter[categoriesMatchOr]
        description: All entries within these categories or their child categories
      - in: query
        name: entryFilter[categoriesNotContains]
      - in: query
        name: entryFilter[categoryAncestorIdIn]
        description: All entries within this categoy or in child categories
      - in: query
        name: entryFilter[createdAtGreaterThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system after a specific time/date (standard
          timestamp format)
      - in: query
        name: entryFilter[createdAtLessThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system before a specific time/date (standard
          timestamp format)
      - in: query
        name: entryFilter[creatorIdEqual]
      - in: query
        name: entryFilter[documentTypeEqual]
        description: 'Enum Type: `KalturaDocumentType`'
      - in: query
        name: entryFilter[documentTypeIn]
      - in: query
        name: entryFilter[durationGreaterThanOrEqual]
      - in: query
        name: entryFilter[durationGreaterThan]
      - in: query
        name: entryFilter[durationLessThanOrEqual]
      - in: query
        name: entryFilter[durationLessThan]
      - in: query
        name: entryFilter[durationTypeMatchOr]
      - in: query
        name: entryFilter[endDateGreaterThanOrEqualOrNull]
      - in: query
        name: entryFilter[endDateGreaterThanOrEqual]
      - in: query
        name: entryFilter[endDateLessThanOrEqualOrNull]
      - in: query
        name: entryFilter[endDateLessThanOrEqual]
      - in: query
        name: entryFilter[entitledUsersEditMatchAnd]
      - in: query
        name: entryFilter[entitledUsersEditMatchOr]
      - in: query
        name: entryFilter[entitledUsersPublishMatchAnd]
      - in: query
        name: entryFilter[entitledUsersPublishMatchOr]
      - in: query
        name: entryFilter[externalSourceTypeEqual]
        description: 'Enum Type: `KalturaExternalMediaSourceType`'
      - in: query
        name: entryFilter[externalSourceTypeIn]
      - in: query
        name: entryFilter[flavorParamsIdsMatchAnd]
      - in: query
        name: entryFilter[flavorParamsIdsMatchOr]
      - in: query
        name: entryFilter[freeText]
      - in: query
        name: entryFilter[groupIdEqual]
      - in: query
        name: entryFilter[hasMediaServerHostname]
      - in: query
        name: entryFilter[idEqual]
        description: This filter should be in use for retrieving only a specific entry
          (identified by its entryId)
      - in: query
        name: entryFilter[idIn]
        description: This filter should be in use for retrieving few specific entries
          (string should include comma separated list of entryId strings)
      - in: query
        name: entryFilter[idNotIn]
      - in: query
        name: entryFilter[isLive]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[isRecordedEntryIdEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[isRoot]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entryFilter[lastPlayedAtGreaterThanOrEqual]
      - in: query
        name: entryFilter[lastPlayedAtLessThanOrEqual]
      - in: query
        name: entryFilter[limit]
      - in: query
        name: entryFilter[mediaDateGreaterThanOrEqual]
      - in: query
        name: entryFilter[mediaDateLessThanOrEqual]
      - in: query
        name: entryFilter[mediaTypeEqual]
        description: 'Enum Type: `KalturaMediaType`'
      - in: query
        name: entryFilter[mediaTypeIn]
      - in: query
        name: entryFilter[moderationStatusEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: entryFilter[moderationStatusIn]
      - in: query
        name: entryFilter[moderationStatusNotEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: entryFilter[moderationStatusNotIn]
      - in: query
        name: entryFilter[nameEqual]
        description: This filter should be in use for retrieving entries with a specific
          name
      - in: query
        name: entryFilter[nameLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[nameMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[nameMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[objectType]
      - in: query
        name: entryFilter[orderBy]
      - in: query
        name: entryFilter[parentEntryIdEqual]
      - in: query
        name: entryFilter[partnerIdEqual]
        description: This filter should be in use for retrieving only entries which
          were uploaded by/assigned to users of a specific Kaltura Partner (identified
          by Partner ID)
      - in: query
        name: entryFilter[partnerIdIn]
        description: This filter should be in use for retrieving only entries within
          Kaltura network which were uploaded by/assigned to users of few Kaltura
          Partners  (string should include comma separated list of PartnerIDs)
      - in: query
        name: entryFilter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: entryFilter[partnerSortValueLessThanOrEqual]
      - in: query
        name: entryFilter[redirectFromEntryId]
        description: The id of the original entry
      - in: query
        name: entryFilter[referenceIdEqual]
      - in: query
        name: entryFilter[referenceIdIn]
      - in: query
        name: entryFilter[replacedEntryIdEqual]
      - in: query
        name: entryFilter[replacedEntryIdIn]
      - in: query
        name: entryFilter[replacementStatusEqual]
        description: 'Enum Type: `KalturaEntryReplacementStatus`'
      - in: query
        name: entryFilter[replacementStatusIn]
      - in: query
        name: entryFilter[replacingEntryIdEqual]
      - in: query
        name: entryFilter[replacingEntryIdIn]
      - in: query
        name: entryFilter[rootEntryIdEqual]
      - in: query
        name: entryFilter[rootEntryIdIn]
      - in: query
        name: entryFilter[searchTextMatchAnd]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within all of the following metadata
          attributes: name, description, tags, adminTags'
      - in: query
        name: entryFilter[searchTextMatchOr]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within at least one of the following
          metadata attributes: name, description, tags, adminTags'
      - in: query
        name: entryFilter[sourceTypeEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: entryFilter[sourceTypeIn]
      - in: query
        name: entryFilter[sourceTypeNotEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: entryFilter[sourceTypeNotIn]
      - in: query
        name: entryFilter[startDateGreaterThanOrEqualOrNull]
      - in: query
        name: entryFilter[startDateGreaterThanOrEqual]
      - in: query
        name: entryFilter[startDateLessThanOrEqualOrNull]
      - in: query
        name: entryFilter[startDateLessThanOrEqual]
      - in: query
        name: entryFilter[statusEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, at a specific {'
      - in: query
        name: entryFilter[statusIn]
        description: This filter should be in use for retrieving only entries, at
          few specific {
      - in: query
        name: entryFilter[statusNotEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, not at a specific {'
      - in: query
        name: entryFilter[statusNotIn]
        description: This filter should be in use for retrieving only entries, not
          at few specific {
      - in: query
        name: entryFilter[tagsAdminTagsMultiLikeAnd]
      - in: query
        name: entryFilter[tagsAdminTagsMultiLikeOr]
      - in: query
        name: entryFilter[tagsAdminTagsNameMultiLikeAnd]
      - in: query
        name: entryFilter[tagsAdminTagsNameMultiLikeOr]
      - in: query
        name: entryFilter[tagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[tagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[tagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: entryFilter[tagsNameMultiLikeAnd]
      - in: query
        name: entryFilter[tagsNameMultiLikeOr]
      - in: query
        name: entryFilter[totalRankGreaterThanOrEqual]
      - in: query
        name: entryFilter[totalRankLessThanOrEqual]
      - in: query
        name: entryFilter[typeEqual]
        description: 'Enum Type: `KalturaEntryType`'
      - in: query
        name: entryFilter[typeIn]
        description: This filter should be in use for retrieving entries of few {
      - in: query
        name: entryFilter[updatedAtGreaterThanOrEqual]
      - in: query
        name: entryFilter[updatedAtLessThanOrEqual]
      - in: query
        name: entryFilter[userIdEqual]
        description: This filter parameter should be in use for retrieving only entries,
          uploaded by/assigned to a specific user (identified by user Id)
      - in: query
        name: entryFilter[userIdIn]
      - in: query
        name: entryFilter[userIdNotIn]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Captionsearch
      - Captionassetitem
      - Action
      - SearchEntries
  /service/capturespace_capturespace/action/clientUpdates:
    get:
      summary: Get Service Capturespace Capturespace Action Clientupdates
      description: Returns latest version and URL
      operationId: captureSpace.clientUpdates
      x-api-path-slug: servicecapturespace-capturespaceactionclientupdates-get
      parameters:
      - in: query
        name: hashAlgorithm
        description: 'Enum Type: `KalturaCaptureSpaceHashAlgorithm`'
      - in: query
        name: No Name
      - in: query
        name: os
      - in: query
        name: version
      responses:
        200:
          description: OK
      tags:
      - Service
      - Capturespace
      - Capturespace
      - Action
      - Clients
  /service/capturespace_capturespace/action/serveInstall:
    get:
      summary: Get Service Capturespace Capturespace Action Serveinstall
      description: Serve installation file
      operationId: captureSpace.serveInstall
      x-api-path-slug: servicecapturespace-capturespaceactionserveinstall-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: os
      responses:
        200:
          description: OK
      tags:
      - Service
      - Capturespace
      - Capturespace
      - Action
      - ServeInstall
  /service/capturespace_capturespace/action/serveUpdate:
    get:
      summary: Get Service Capturespace Capturespace Action Serveupdate
      description: Serve update file
      operationId: captureSpace.serveUpdate
      x-api-path-slug: servicecapturespace-capturespaceactionserveupdate-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: os
      - in: query
        name: version
      responses:
        200:
          description: OK
      tags:
      - Service
      - Capturespace
      - Capturespace
      - Action
      - Serve
  /service/category/action/add:
    get:
      summary: Get Service Category Action Add
      description: Add new Category
      operationId: category.add
      x-api-path-slug: servicecategoryactionadd-get
      parameters:
      - in: query
        name: category[aggregationCategories]
        description: List of aggregation channels the category belongs to
      - in: query
        name: category[appearInList]
        description: 'Enum Type: `KalturaAppearInListType`If category will be returned
          for list action'
      - in: query
        name: category[contributionPolicy]
        description: 'Enum Type: `KalturaContributionPolicyType`who can assign entries
          to this category'
      - in: query
        name: category[defaultOrderBy]
        description: 'Enum Type: `KalturaCategoryOrderBy`Enable client side applications
          to define how to sort the category child categories'
      - in: query
        name: category[defaultPermissionLevel]
        description: 'Enum Type: `KalturaCategoryUserPermissionLevel`Default permissionLevel
          for new users'
      - in: query
        name: category[description]
        description: Category description
      - in: query
        name: category[inheritanceType]
        description: 'Enum Type: `KalturaInheritanceType`If Category members are inherited
          from parent category or set manualy'
      - in: query
        name: category[isAggregationCategory]
        description: 'Enum Type: `KalturaNullableBoolean`Flag indicating that the
          category is an aggregation category'
      - in: query
        name: category[moderation]
        description: 'Enum Type: `KalturaNullableBoolean`Moderation to add entries
          to this category by users that are not of permission level Manager or Moderator'
      - in: query
        name: category[name]
        description: The name of the Category
      - in: query
        name: category[owner]
        description: Category Owner (User id)
      - in: query
        name: category[parentId]
      - in: query
        name: category[partnerData]
        description: Can be used to store various partner related data as a string
      - in: query
        name: category[partnerSortValue]
        description: Can be used to store various partner related data as a numeric
          value
      - in: query
        name: category[privacyContext]
        description: Set privacy context for search entries that assiged to private
          and public categories
      - in: query
        name: category[privacy]
        description: 'Enum Type: `KalturaPrivacyType`defines the privacy of the entries
          that assigned to this category'
      - in: query
        name: category[referenceId]
        description: Category external id, controlled and managed by the partner
      - in: query
        name: category[tags]
        description: Category tags
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - Add
  /service/category/action/addFromBulkUpload:
    post:
      summary: Post Service Category Action Addfrombulkupload
      description: ""
      operationId: category.addFromBulkUpload
      x-api-path-slug: servicecategoryactionaddfrombulkupload-post
      parameters:
      - in: query
        name: bulkUploadData[fileName]
        description: Friendly name of the file, used to be recognized later in the
          logs
      - in: query
        name: bulkUploadData[objectData][conversionProfileId]
        description: Selected profile id for all bulk entries
      - in: query
        name: bulkUploadData[objectData][objectType]
      - in: formData
        name: fileData
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - AddFromBulkUpload
  /service/category/action/delete:
    get:
      summary: Get Service Category Action Delete
      description: Delete a Category
      operationId: category.delete
      x-api-path-slug: servicecategoryactiondelete-get
      parameters:
      - in: query
        name: id
      - in: query
        name: moveEntriesToParentCategory
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - Delete
  /service/category/action/get:
    get:
      summary: Get Service Category Action Get
      description: Get Category by id
      operationId: category.get
      x-api-path-slug: servicecategoryactionget-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - Get
  /service/category/action/index:
    get:
      summary: Get Service Category Action Index
      description: Index Category by id
      operationId: category.index
      x-api-path-slug: servicecategoryactionindex-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: shouldUpdate
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - Index
  /service/category/action/list:
    get:
      summary: Get Service Category Action List
      description: List all categories
      operationId: category.list
      x-api-path-slug: servicecategoryactionlist-get
      parameters:
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[aggregationCategoriesMultiLikeAnd]
      - in: query
        name: filter[aggregationCategoriesMultiLikeOr]
      - in: query
        name: filter[ancestorIdIn]
        description: not includes the category itself (only sub categories)
      - in: query
        name: filter[appearInListEqual]
        description: 'Enum Type: `KalturaAppearInListType`'
      - in: query
        name: filter[contributionPolicyEqual]
        description: 'Enum Type: `KalturaContributionPolicyType`'
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
      - in: query
        name: filter[createdAtLessThanOrEqual]
      - in: query
        name: filter[depthEqual]
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[fullIdsEqual]
      - in: query
        name: filter[fullIdsMatchOr]
      - in: query
        name: filter[fullIdsStartsWith]
      - in: query
        name: filter[fullNameEqual]
      - in: query
        name: filter[fullNameIn]
      - in: query
        name: filter[fullNameStartsWithIn]
      - in: query
        name: filter[fullNameStartsWith]
      - in: query
        name: filter[idEqual]
      - in: query
        name: filter[idIn]
      - in: query
        name: filter[idNotIn]
      - in: query
        name: filter[idOrInheritedParentIdIn]
      - in: query
        name: filter[inheritanceTypeEqual]
        description: 'Enum Type: `KalturaInheritanceType`'
      - in: query
        name: filter[inheritanceTypeIn]
      - in: query
        name: filter[inheritedParentIdEqual]
      - in: query
        name: filter[inheritedParentIdIn]
      - in: query
        name: filter[managerEqual]
      - in: query
        name: filter[memberEqual]
      - in: query
        name: filter[membersCountGreaterThanOrEqual]
      - in: query
        name: filter[membersCountLessThanOrEqual]
      - in: query
        name: filter[membersIn]
      - in: query
        name: filter[nameOrReferenceIdStartsWith]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentIdEqual]
      - in: query
        name: filter[parentIdIn]
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[pendingMembersCountGreaterThanOrEqual]
      - in: query
        name: filter[pendingMembersCountLessThanOrEqual]
      - in: query
        name: filter[privacyContextEqual]
      - in: query
        name: filter[privacyEqual]
        description: 'Enum Type: `KalturaPrivacyType`'
      - in: query
        name: filter[privacyIn]
      - in: query
        name: filter[referenceIdEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[referenceIdEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaCategoryStatus`'
      - in: query
        name: filter[statusIn]
      - in: query
        name: filter[tagsLike]
      - in: query
        name: filter[tagsMultiLikeAnd]
      - in: query
        name: filter[tagsMultiLikeOr]
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - List
  /service/category/action/move:
    get:
      summary: Get Service Category Action Move
      description: Move categories that belong to the same parent category to a target
        categroy - enabled only for ks with disable entitlement
      operationId: category.move
      x-api-path-slug: servicecategoryactionmove-get
      parameters:
      - in: query
        name: categoryIds
      - in: query
        name: No Name
      - in: query
        name: targetCategoryParentId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - Move
  /service/category/action/unlockCategories:
    get:
      summary: Get Service Category Action Unlockcategories
      description: Unlock categories
      operationId: category.unlockCategories
      x-api-path-slug: servicecategoryactionunlockcategories-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - UnlockCategories
  /service/category/action/update:
    get:
      summary: Get Service Category Action Update
      description: Update Category
      operationId: category.update
      x-api-path-slug: servicecategoryactionupdate-get
      parameters:
      - in: query
        name: category[aggregationCategories]
        description: List of aggregation channels the category belongs to
      - in: query
        name: category[appearInList]
        description: 'Enum Type: `KalturaAppearInListType`If category will be returned
          for list action'
      - in: query
        name: category[contributionPolicy]
        description: 'Enum Type: `KalturaContributionPolicyType`who can assign entries
          to this category'
      - in: query
        name: category[defaultOrderBy]
        description: 'Enum Type: `KalturaCategoryOrderBy`Enable client side applications
          to define how to sort the category child categories'
      - in: query
        name: category[defaultPermissionLevel]
        description: 'Enum Type: `KalturaCategoryUserPermissionLevel`Default permissionLevel
          for new users'
      - in: query
        name: category[description]
        description: Category description
      - in: query
        name: category[inheritanceType]
        description: 'Enum Type: `KalturaInheritanceType`If Category members are inherited
          from parent category or set manualy'
      - in: query
        name: category[isAggregationCategory]
        description: 'Enum Type: `KalturaNullableBoolean`Flag indicating that the
          category is an aggregation category'
      - in: query
        name: category[moderation]
        description: 'Enum Type: `KalturaNullableBoolean`Moderation to add entries
          to this category by users that are not of permission level Manager or Moderator'
      - in: query
        name: category[name]
        description: The name of the Category
      - in: query
        name: category[owner]
        description: Category Owner (User id)
      - in: query
        name: category[parentId]
      - in: query
        name: category[partnerData]
        description: Can be used to store various partner related data as a string
      - in: query
        name: category[partnerSortValue]
        description: Can be used to store various partner related data as a numeric
          value
      - in: query
        name: category[privacyContext]
        description: Set privacy context for search entries that assiged to private
          and public categories
      - in: query
        name: category[privacy]
        description: 'Enum Type: `KalturaPrivacyType`defines the privacy of the entries
          that assigned to this category'
      - in: query
        name: category[referenceId]
        description: Category external id, controlled and managed by the partner
      - in: query
        name: category[tags]
        description: Category tags
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Category
      - Action
      - Update
  /service/categoryentry/action/activate:
    get:
      summary: Get Service Categoryentry Action Activate
      description: activate CategoryEntry when it is pending moderation
      operationId: categoryEntry.activate
      x-api-path-slug: servicecategoryentryactionactivate-get
      parameters:
      - in: query
        name: categoryId
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Categoryentry
      - Action
      - Activate
  /service/categoryentry/action/add:
    get:
      summary: Get Service Categoryentry Action Add
      description: Add new CategoryEntry
      operationId: categoryEntry.add
      x-api-path-slug: servicecategoryentryactionadd-get
      parameters:
      - in: query
        name: categoryEntry[categoryId]
      - in: query
        name: categoryEntry[entryId]
        description: entry id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Categoryentry
      - Action
      - Add
  /service/categoryentry/action/addFromBulkUpload:
    get:
      summary: Get Service Categoryentry Action Addfrombulkupload
      description: ""
      operationId: categoryEntry.addFromBulkUpload
      x-api-path-slug: servicecategoryentryactionaddfrombulkupload-get
      parameters:
      - in: query
        name: bulkUploadData[filter][advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: bulkUploadData[filter][advancedSearch][categoriesMatchOr]
      - in: query
        name: bulkUploadData[filter][advancedSearch][categoryEntryStatusIn]
      - in: query
        name: bulkUploadData[filter][advancedSearch][categoryIdEqual]
      - in: query
        name: bulkUploadData[filter][advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: bulkUploadData[filter][advancedSearch][contentLike]
      - in: query
        name: bulkUploadData[filter][advancedSearch][contentMultiLikeAnd]
      - in: query
        name: bulkUploadData[filter][advancedSearch][contentMultiLikeOr]
      - in: query
        name: bulkUploadData[filter][advancedSearch][cuePointsFreeText]
      - in: query
        name: bulkUploadData[filter][advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: bulkUploadData[filter][advancedSearch][cuePointTypeIn]
      - in: query
        name: bulkUploadData[filter][advancedSearch][depthGreaterThanEqual]
      - in: query
        name: bulkUploadData[filter][advancedSearch][distributionProfileId]
      - in: query
        name: bulkUploadData[filter][advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: bulkUploadData[filter][advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: bulkUploadData[filter][advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: bulkUploadData[filter][advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: bulkUploadData[filter][advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: bulkUploadData[filter][advancedSearch][extendedStatusIn]
      - in: query
        name: bulkUploadData[filter][advancedSearch][field]
      - in: query
        name: bulkUploadData[filter][advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: bulkUploadData[filter][advancedSearch][idEqual]
      - in: query
        name: bulkUploadData[filter][advancedSearch][idIn]
      - in: query
        name: bulkUploadData[filter][advancedSearch][indexIdGreaterThan]
      - in: query
        name: bulkUploadData[filter][advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: bulkUploadData[filter][advancedSearch][items]
      - in: query
        name: bulkUploadData[filter][advancedSearch][memberIdEq]
      - in: query
        name: bulkUploadData[filter][advancedSearch][memberIdIn]
      - in: query
        name: bulkUploadData[filter][advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: bulkUploadData[filter][advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: bulkUploadData[filter][advancedSearch][metadataProfileId]
      - in: query
        name: bulkUploadData[filter][advancedSearch][noDistributionProfiles]
      - in: query
        name: bulkUploadData[filter][advancedSearch][not]
      - in: query
        name: bulkUploadData[filter][advancedSearch][objectType]
      - in: query
        name: bulkUploadData[filter][advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: bulkUploadData[filter][advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: bulkUploadData[filter][advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: bulkUploadData[filter][advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: bulkUploadData[filter][advancedSearch][userIdEqual]
      - in: query
        name: bulkUploadData[filter][advancedSearch][userIdIn]
      - in: query
        name: bulkUploadData[filter][advancedSearch][value]
      - in: query
        name: bulkUploadData[filter][advancedSearch][watermarkId]
      - in: query
        name: bulkUploadData[filter][orderBy]
      - in: query
        name: bulkUploadData[objectType]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Categoryentry
      - Action
      - AddFromBulkUpload
  /service/categoryentry/action/delete:
    get:
      summary: Get Service Categoryentry Action Delete
      description: Delete CategoryEntry
      operationId: categoryEntry.delete
      x-api-path-slug: servicecategoryentryactiondelete-get
      parameters:
      - in: query
        name: categoryId
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Categoryentry
      - Action
      - Delete
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---