---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/{enterpriseId}/storeLayout/pages/{pageId}:
    put:
      summary: Create Store Layout Page
      description: Updates the content of a store page.
      operationId: androidenterprise.storelayoutpages.update
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
  /enterprises/{enterpriseId}/storeLayout/pages/{pageId}/clusters:
    get:
      summary: Get Store Layout Page Clusters
      description: Retrieves the details of all clusters on the specified page.
      operationId: androidenterprise.storelayoutclusters.list
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclusters-get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
    post:
      summary: Insert Store Layout Page Cluster
      description: Inserts a new cluster in a page.
      operationId: androidenterprise.storelayoutclusters.insert
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclusters-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
  /enterprises/{enterpriseId}/storeLayout/pages/{pageId}/clusters/{clusterId}:
    delete:
      summary: Delete Store Layout Page Cluster
      description: Deletes a cluster.
      operationId: androidenterprise.storelayoutclusters.delete
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclustersclusterid-delete
      parameters:
      - in: path
        name: clusterId
        description: The ID of the cluster
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
    get:
      summary: Get Store Layout Page Cluster
      description: Retrieves details of a cluster.
      operationId: androidenterprise.storelayoutclusters.get
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclustersclusterid-get
      parameters:
      - in: path
        name: clusterId
        description: The ID of the cluster
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
    patch:
      summary: Update Store Layout Page Cluster
      description: Updates a cluster. This method supports patch semantics.
      operationId: androidenterprise.storelayoutclusters.patch
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclustersclusterid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterId
        description: The ID of the cluster
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
    put:
      summary: Update Store Layout Page Cluster
      description: Updates a cluster.
      operationId: androidenterprise.storelayoutclusters.update
      x-api-path-slug: enterprisesenterpriseidstorelayoutpagespageidclustersclusterid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: clusterId
        description: The ID of the cluster
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Store Layout Page Cluster
---