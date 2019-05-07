# ![LOGO](logo.png) OpenTrials **flow**ground Connector

## Description

A generated **flow**ground connector for the OpenTrials API (version 0.0.1).

Generated from: https://api.apis.guru/v2/specs/opentrials.local/0.0.1/swagger.json<br/>
Generated at: 2019-05-07T17:43:28+03:00

## API Description



## Authorization

This API does not require authorization.

## Actions

### Returns condition details

*Tags:* `conditions`

#### Input Parameters
* `id` - _required_ - ID of the condition

### x_swagger_router_controller_conditions__id_

### Returns document categories

*Tags:* `document_categories`

### x_swagger_router_controller_document_categories

### Returns documents

*Tags:* `documents`

#### Input Parameters
* `page` - _optional_ - The page number
* `per_page` - _optional_ - Number of items per page

### x_swagger_router_controller_documents

### Returns details of a document

*Tags:* `documents`

#### Input Parameters
* `id` - _required_ - ID of the document

### x_swagger_router_controller_documents__id_

### Returns FDA applications

*Tags:* `fda_applications`

#### Input Parameters
* `page` - _optional_ - The page number
* `per_page` - _optional_ - Number of items per page

### x_swagger_router_controller_fda_applications

### Returns an FDA application details

*Tags:* `fda_applications`

#### Input Parameters
* `id` - _required_ - ID of the FDA application

### x_swagger_router_controller_fda_applications__id_

### Returns intervention details

*Tags:* `interventions`

#### Input Parameters
* `id` - _required_ - ID of the intervention

### x_swagger_router_controller_interventions__id_

### Returns organisation details

*Tags:* `organisations`

#### Input Parameters
* `id` - _required_ - ID of the organisation

### x_swagger_router_controller_organisations__id_

### Returns person details

*Tags:* `persons`

#### Input Parameters
* `id` - _required_ - ID of the person

### x_swagger_router_controller_persons__id_

### Returns publication details

*Tags:* `publications`

#### Input Parameters
* `id` - _required_ - ID of the publication

### x_swagger_router_controller_publications__id_

### Returns trials based on a search query. By default, it'll search in all of a trial's attributes.<br/>
> - `q` is a [ElasticSearch query string](https://www.elastic.co/guide/en/elasticsearch/reference/2.3/query-dsl-query-string-query.html#query-string-syntax) (e.g. `public_title:(depressive OR depression)`)<br/>
> - `page` can take a value between `1` and `100`<br/>
> - `per_page` can take a value between `10` and `100`

*Tags:* `trials`

#### Input Parameters
* `q` - _optional_ - The search query (follows the [ElasticSearch Query String](https://www.elastic.co/guide/en/elasticsearch/reference/2.3/query-dsl-query-string-query.html#query-string-syntax) syntax)
* `page` - _optional_ - The page number
* `per_page` - _optional_ - Number of items per page

### x_swagger_router_controller_search

### Autocomplete search feature for supported database entities (`location`). It has the same options as a regular `search` operation, with an extra **required** `in` parameter indicating the entity type to search.

*Tags:* `search`

#### Input Parameters
* `in` - _required_ - The entity to search for
    Possible values: location.
* `q` - _optional_ - The search query
* `page` - _optional_ - The page number
* `per_page` - _optional_ - Number of items per page

### x_swagger_router_controller_search_autocomplete__in_

### Search the FDA documents

*Tags:* `search`

#### Input Parameters
* `q` - _optional_ - The search query (follows the [ElasticSearch Query String](https://www.elastic.co/guide/en/elasticsearch/reference/2.3/query-dsl-query-string-query.html#query-string-syntax) syntax)
* `text` - _optional_ - Search query on the documents file's text (follows the [ElasticSearch Simple Query String](https://www.elastic.co/guide/en/elasticsearch/reference/2.3/query-dsl-simple-query-string-query.html#_simple_query_string_syntax) syntax)
* `page` - _optional_ - The page number
* `per_page` - _optional_ - Number of items per page

### x_swagger_router_controller_search_fda_documents

### Returns list of sources

*Tags:* `sources`

### x_swagger_router_controller_sources

### x_swagger_pipe_swagger_yaml

### Returns a trial's details and related entities (e.g. `conditions`).

*Tags:* `trials`

#### Input Parameters
* `id` - _required_ - ID of the trial

### x_swagger_router_controller_trials__id_

### Returns a trial's raw records from its sources

*Tags:* `trials`

#### Input Parameters
* `id` - _required_ - ID of the trial

### x_swagger_router_controller_trials__id__records

### Returns a trial's raw record from its sources

*Tags:* `trials`

#### Input Parameters
* `trialId` - _required_ - ID of the trial
* `id` - _required_ - ID of the trial's record

### x_swagger_router_controller_trials__trialId__records__id_

## License

**flow**ground :- Telekom iPaaS / opentrials-local-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
