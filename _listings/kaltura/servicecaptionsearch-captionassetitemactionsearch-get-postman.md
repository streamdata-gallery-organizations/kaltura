{
  "info": {
    "name": "Kaltura VPaaS Get Service Captionsearch Captionassetitem Action Search",
    "_postman_id": "e9727b07-3071-4c2b-a0d0-2062dcd90e18",
    "description": "Search caption asset items by filter, pager and free text",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "86042908-b5a8-4dc0-86b5-d6083034a13e",
          "name": "captionAssetItem.parse",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/captionsearch_captionassetitem/action/parse?captionAssetId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Parse content of caption asset and index it"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6825b00-c06f-4648-b535-08b049c21ca6"
            }
          ]
        },
        {
          "id": "bae93c71-b4bf-4c08-b85e-8e65517fcfd7",
          "name": "captionAssetItem.search",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/captionsearch_captionassetitem/action/search?captionAssetItemFilter[advancedSearch][attribute]=%7B%7D&captionAssetItemFilter[advancedSearch][categoriesMatchOr]=%7B%7D&captionAssetItemFilter[advancedSearch][categoryEntryStatusIn]=%7B%7D&captionAssetItemFilter[advancedSearch][categoryIdEqual]=%7B%7D&captionAssetItemFilter[advancedSearch][comparison]=%7B%7D&captionAssetItemFilter[advancedSearch][contentLike]=%7B%7D&captionAssetItemFilter[advancedSearch][contentMultiLikeAnd]=%7B%7D&captionAssetItemFilter[advancedSearch][contentMultiLikeOr]=%7B%7D&captionAssetItemFilter[advancedSearch][cuePointsFreeText]=%7B%7D&captionAssetItemFilter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&captionAssetItemFilter[advancedSearch][cuePointTypeIn]=%7B%7D&captionAssetItemFilter[advancedSearch][depthGreaterThanEqual]=%7B%7D&captionAssetItemFilter[advancedSearch][distributionProfileId]=%7B%7D&captionAssetItemFilter[advancedSearch][distributionSunStatus]=%7B%7D&captionAssetItemFilter[advancedSearch][entryDistributionFlag]=%7B%7D&captionAssetItemFilter[advancedSearch][entryDistributionStatus]=%7B%7D&captionAssetItemFilter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&captionAssetItemFilter[advancedSearch][extendedStatusEqual]=%7B%7D&captionAssetItemFilter[advancedSearch][extendedStatusIn]=%7B%7D&captionAssetItemFilter[advancedSearch][field]=%7B%7D&captionAssetItemFilter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&captionAssetItemFilter[advancedSearch][idEqual]=%7B%7D&captionAssetItemFilter[advancedSearch][idIn]=%7B%7D&captionAssetItemFilter[advancedSearch][indexIdGreaterThan]=%7B%7D&captionAssetItemFilter[advancedSearch][isQuiz]=%7B%7D&captionAssetItemFilter[advancedSearch][items]=%7B%7D&captionAssetItemFilter[advancedSearch][memberIdEq]=%7B%7D&captionAssetItemFilter[advancedSearch][memberIdIn]=%7B%7D&captionAssetItemFilter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&captionAssetItemFilter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&captionAssetItemFilter[advancedSearch][metadataProfileId]=%7B%7D&captionAssetItemFilter[advancedSearch][noDistributionProfiles]=%7B%7D&captionAssetItemFilter[advancedSearch][not]=%7B%7D&captionAssetItemFilter[advancedSearch][objectType]=%7B%7D&captionAssetItemFilter[advancedSearch][orderBy]=%7B%7D&captionAssetItemFilter[advancedSearch][type]=%7B%7D&captionAssetItemFilter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&captionAssetItemFilter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&captionAssetItemFilter[advancedSearch][userIdEqual]=%7B%7D&captionAssetItemFilter[advancedSearch][userIdIn]=%7B%7D&captionAssetItemFilter[advancedSearch][value]=%7B%7D&captionAssetItemFilter[advancedSearch][watermarkId]=%7B%7D&captionAssetItemFilter[captionParamsIdEqual]=%7B%7D&captionAssetItemFilter[captionParamsIdIn]=%7B%7D&captionAssetItemFilter[contentLike]=%7B%7D&captionAssetItemFilter[contentMultiLikeAnd]=%7B%7D&captionAssetItemFilter[contentMultiLikeOr]=%7B%7D&captionAssetItemFilter[createdAtGreaterThanOrEqual]=%7B%7D&captionAssetItemFilter[createdAtLessThanOrEqual]=%7B%7D&captionAssetItemFilter[deletedAtGreaterThanOrEqual]=%7B%7D&captionAssetItemFilter[deletedAtLessThanOrEqual]=%7B%7D&captionAssetItemFilter[endTimeGreaterThanOrEqual]=%7B%7D&captionAssetItemFilter[endTimeLessThanOrEqual]=%7B%7D&captionAssetItemFilter[entryIdEqual]=%7B%7D&captionAssetItemFilter[entryIdIn]=%7B%7D&captionAssetItemFilter[formatEqual]=%7B%7D&captionAssetItemFilter[formatIn]=%7B%7D&captionAssetItemFilter[idEqual]=%7B%7D&captionAssetItemFilter[idIn]=%7B%7D&captionAssetItemFilter[labelEqual]=%7B%7D&captionAssetItemFilter[labelIn]=%7B%7D&captionAssetItemFilter[languageEqual]=%7B%7D&captionAssetItemFilter[languageIn]=%7B%7D&captionAssetItemFilter[orderBy]=%7B%7D&captionAssetItemFilter[partnerDescriptionLike]=%7B%7D&captionAssetItemFilter[partnerDescriptionMultiLikeAnd]=%7B%7D&captionAssetItemFilter[partnerDescriptionMultiLikeOr]=%7B%7D&captionAssetItemFilter[partnerIdEqual]=%7B%7D&captionAssetItemFilter[partnerIdIn]=%7B%7D&captionAssetItemFilter[sizeGreaterThanOrEqual]=%7B%7D&captionAssetItemFilter[sizeLessThanOrEqual]=%7B%7D&captionAssetItemFilter[startTimeGreaterThanOrEqual]=%7B%7D&captionAssetItemFilter[startTimeLessThanOrEqual]=%7B%7D&captionAssetItemFilter[statusEqual]=%7B%7D&captionAssetItemFilter[statusIn]=%7B%7D&captionAssetItemFilter[statusNotIn]=%7B%7D&captionAssetItemFilter[tagsLike]=%7B%7D&captionAssetItemFilter[tagsMultiLikeAnd]=%7B%7D&captionAssetItemFilter[tagsMultiLikeOr]=%7B%7D&captionAssetItemFilter[typeIn]=%7B%7D&captionAssetItemFilter[updatedAtGreaterThanOrEqual]=%7B%7D&captionAssetItemFilter[updatedAtLessThanOrEqual]=%7B%7D&captionAssetItemPager[pageIndex]=%7B%7D&captionAssetItemPager[pageSize]=%7B%7D&entryFilter[accessControlIdEqual]=%7B%7D&entryFilter[accessControlIdIn]=%7B%7D&entryFilter[adminTagsLike]=%7B%7D&entryFilter[adminTagsMultiLikeAnd]=%7B%7D&entryFilter[adminTagsMultiLikeOr]=%7B%7D&entryFilter[advancedSearch][attribute]=%7B%7D&entryFilter[advancedSearch][categoriesMatchOr]=%7B%7D&entryFilter[advancedSearch][categoryEntryStatusIn]=%7B%7D&entryFilter[advancedSearch][categoryIdEqual]=%7B%7D&entryFilter[advancedSearch][comparison]=%7B%7D&entryFilter[advancedSearch][contentLike]=%7B%7D&entryFilter[advancedSearch][contentMultiLikeAnd]=%7B%7D&entryFilter[advancedSearch][contentMultiLikeOr]=%7B%7D&entryFilter[advancedSearch][cuePointsFreeText]=%7B%7D&entryFilter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&entryFilter[advancedSearch][cuePointTypeIn]=%7B%7D&entryFilter[advancedSearch][depthGreaterThanEqual]=%7B%7D&entryFilter[advancedSearch][distributionProfileId]=%7B%7D&entryFilter[advancedSearch][distributionSunStatus]=%7B%7D&entryFilter[advancedSearch][entryDistributionFlag]=%7B%7D&entryFilter[advancedSearch][entryDistributionStatus]=%7B%7D&entryFilter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&entryFilter[advancedSearch][extendedStatusEqual]=%7B%7D&entryFilter[advancedSearch][extendedStatusIn]=%7B%7D&entryFilter[advancedSearch][field]=%7B%7D&entryFilter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&entryFilter[advancedSearch][idEqual]=%7B%7D&entryFilter[advancedSearch][idIn]=%7B%7D&entryFilter[advancedSearch][indexIdGreaterThan]=%7B%7D&entryFilter[advancedSearch][isQuiz]=%7B%7D&entryFilter[advancedSearch][items]=%7B%7D&entryFilter[advancedSearch][memberIdEq]=%7B%7D&entryFilter[advancedSearch][memberIdIn]=%7B%7D&entryFilter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&entryFilter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&entryFilter[advancedSearch][metadataProfileId]=%7B%7D&entryFilter[advancedSearch][noDistributionProfiles]=%7B%7D&entryFilter[advancedSearch][not]=%7B%7D&entryFilter[advancedSearch][objectType]=%7B%7D&entryFilter[advancedSearch][orderBy]=%7B%7D&entryFilter[advancedSearch][type]=%7B%7D&entryFilter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&entryFilter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&entryFilter[advancedSearch][userIdEqual]=%7B%7D&entryFilter[advancedSearch][userIdIn]=%7B%7D&entryFilter[advancedSearch][value]=%7B%7D&entryFilter[advancedSearch][watermarkId]=%7B%7D&entryFilter[assetParamsIdsMatchAnd]=%7B%7D&entryFilter[assetParamsIdsMatchOr]=%7B%7D&entryFilter[categoriesFullNameIn]=%7B%7D&entryFilter[categoriesIdsEmpty]=%7B%7D&entryFilter[categoriesIdsMatchAnd]=%7B%7D&entryFilter[categoriesIdsMatchOr]=%7B%7D&entryFilter[categoriesIdsNotContains]=%7B%7D&entryFilter[categoriesMatchAnd]=%7B%7D&entryFilter[categoriesMatchOr]=%7B%7D&entryFilter[categoriesNotContains]=%7B%7D&entryFilter[categoryAncestorIdIn]=%7B%7D&entryFilter[createdAtGreaterThanOrEqual]=%7B%7D&entryFilter[createdAtLessThanOrEqual]=%7B%7D&entryFilter[creatorIdEqual]=%7B%7D&entryFilter[documentTypeEqual]=%7B%7D&entryFilter[documentTypeIn]=%7B%7D&entryFilter[durationGreaterThanOrEqual]=%7B%7D&entryFilter[durationGreaterThan]=%7B%7D&entryFilter[durationLessThanOrEqual]=%7B%7D&entryFilter[durationLessThan]=%7B%7D&entryFilter[durationTypeMatchOr]=%7B%7D&entryFilter[endDateGreaterThanOrEqualOrNull]=%7B%7D&entryFilter[endDateGreaterThanOrEqual]=%7B%7D&entryFilter[endDateLessThanOrEqualOrNull]=%7B%7D&entryFilter[endDateLessThanOrEqual]=%7B%7D&entryFilter[entitledUsersEditMatchAnd]=%7B%7D&entryFilter[entitledUsersEditMatchOr]=%7B%7D&entryFilter[entitledUsersPublishMatchAnd]=%7B%7D&entryFilter[entitledUsersPublishMatchOr]=%7B%7D&entryFilter[externalSourceTypeEqual]=%7B%7D&entryFilter[externalSourceTypeIn]=%7B%7D&entryFilter[flavorParamsIdsMatchAnd]=%7B%7D&entryFilter[flavorParamsIdsMatchOr]=%7B%7D&entryFilter[freeText]=%7B%7D&entryFilter[groupIdEqual]=%7B%7D&entryFilter[hasMediaServerHostname]=%7B%7D&entryFilter[idEqual]=%7B%7D&entryFilter[idIn]=%7B%7D&entryFilter[idNotIn]=%7B%7D&entryFilter[isLive]=%7B%7D&entryFilter[isRecordedEntryIdEmpty]=%7B%7D&entryFilter[isRoot]=%7B%7D&entryFilter[lastPlayedAtGreaterThanOrEqual]=%7B%7D&entryFilter[lastPlayedAtLessThanOrEqual]=%7B%7D&entryFilter[limit]=%7B%7D&entryFilter[mediaDateGreaterThanOrEqual]=%7B%7D&entryFilter[mediaDateLessThanOrEqual]=%7B%7D&entryFilter[mediaTypeEqual]=%7B%7D&entryFilter[mediaTypeIn]=%7B%7D&entryFilter[moderationStatusEqual]=%7B%7D&entryFilter[moderationStatusIn]=%7B%7D&entryFilter[moderationStatusNotEqual]=%7B%7D&entryFilter[moderationStatusNotIn]=%7B%7D&entryFilter[nameEqual]=%7B%7D&entryFilter[nameLike]=%7B%7D&entryFilter[nameMultiLikeAnd]=%7B%7D&entryFilter[nameMultiLikeOr]=%7B%7D&entryFilter[objectType]=%7B%7D&entryFilter[orderBy]=%7B%7D&entryFilter[parentEntryIdEqual]=%7B%7D&entryFilter[partnerIdEqual]=%7B%7D&entryFilter[partnerIdIn]=%7B%7D&entryFilter[partnerSortValueGreaterThanOrEqual]=%7B%7D&entryFilter[partnerSortValueLessThanOrEqual]=%7B%7D&entryFilter[redirectFromEntryId]=%7B%7D&entryFilter[referenceIdEqual]=%7B%7D&entryFilter[referenceIdIn]=%7B%7D&entryFilter[replacedEntryIdEqual]=%7B%7D&entryFilter[replacedEntryIdIn]=%7B%7D&entryFilter[replacementStatusEqual]=%7B%7D&entryFilter[replacementStatusIn]=%7B%7D&entryFilter[replacingEntryIdEqual]=%7B%7D&entryFilter[replacingEntryIdIn]=%7B%7D&entryFilter[rootEntryIdEqual]=%7B%7D&entryFilter[rootEntryIdIn]=%7B%7D&entryFilter[searchTextMatchAnd]=%7B%7D&entryFilter[searchTextMatchOr]=%7B%7D&entryFilter[sourceTypeEqual]=%7B%7D&entryFilter[sourceTypeIn]=%7B%7D&entryFilter[sourceTypeNotEqual]=%7B%7D&entryFilter[sourceTypeNotIn]=%7B%7D&entryFilter[startDateGreaterThanOrEqualOrNull]=%7B%7D&entryFilter[startDateGreaterThanOrEqual]=%7B%7D&entryFilter[startDateLessThanOrEqualOrNull]=%7B%7D&entryFilter[startDateLessThanOrEqual]=%7B%7D&entryFilter[statusEqual]=%7B%7D&entryFilter[statusIn]=%7B%7D&entryFilter[statusNotEqual]=%7B%7D&entryFilter[statusNotIn]=%7B%7D&entryFilter[tagsAdminTagsMultiLikeAnd]=%7B%7D&entryFilter[tagsAdminTagsMultiLikeOr]=%7B%7D&entryFilter[tagsAdminTagsNameMultiLikeAnd]=%7B%7D&entryFilter[tagsAdminTagsNameMultiLikeOr]=%7B%7D&entryFilter[tagsLike]=%7B%7D&entryFilter[tagsMultiLikeAnd]=%7B%7D&entryFilter[tagsMultiLikeOr]=%7B%7D&entryFilter[tagsNameMultiLikeAnd]=%7B%7D&entryFilter[tagsNameMultiLikeOr]=%7B%7D&entryFilter[totalRankGreaterThanOrEqual]=%7B%7D&entryFilter[totalRankLessThanOrEqual]=%7B%7D&entryFilter[typeEqual]=%7B%7D&entryFilter[typeIn]=%7B%7D&entryFilter[updatedAtGreaterThanOrEqual]=%7B%7D&entryFilter[updatedAtLessThanOrEqual]=%7B%7D&entryFilter[userIdEqual]=%7B%7D&entryFilter[userIdIn]=%7B%7D&entryFilter[userIdNotIn]=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search caption asset items by filter, pager and free text"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de3ec0a0-e92e-470a-b209-c7a25a9f2197"
            }
          ]
        }
      ]
    }
  ]
}