# APIService

* [read operations](#read)
* [write operations](#write)

## read

  ### apis.apiregistration.k8s.io.v1.apiservices.get

  list or watch objects of kind APIService

  #### Query

  | Parameter | Description |
  | --------- | ----------- |
  | `qs` | Querystring object |
  | `qs.continue` | The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server the server will respond with a 410 ResourceExpired error indicating the client must restart their list without the continue field. This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. |
  | `qs.fieldSelector` | A selector to restrict the list of returned objects by their fields. Defaults to everything. |
  | `qs.includeUninitialized` | If true, partially initialized resources are included in the response. |
  | `qs.labelSelector` | A selector to restrict the list of returned objects by their labels. Defaults to everything. |
  | `qs.limit` | limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.<br/><br/>The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. |
  | `qs.resourceVersion` | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it&#39;s 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv. |
  | `qs.timeoutSeconds` | Timeout for the list&#x2F;watch call. This limits the duration of the call, regardless of any activity or inactivity. |
  | `qs.watch` | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. |
  | `qs.pretty` | If &#39;true&#39;, then the output is pretty printed. |

  ### apis.apiregistration.k8s.io.v1.watch.apiservices.get

  watch individual changes to a list of APIService

  #### Query

  | Parameter | Description |
  | --------- | ----------- |
  | `qs` | Querystring object |
  | `qs.continue` | The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server the server will respond with a 410 ResourceExpired error indicating the client must restart their list without the continue field. This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. |
  | `qs.fieldSelector` | A selector to restrict the list of returned objects by their fields. Defaults to everything. |
  | `qs.includeUninitialized` | If true, partially initialized resources are included in the response. |
  | `qs.labelSelector` | A selector to restrict the list of returned objects by their labels. Defaults to everything. |
  | `qs.limit` | limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.<br/><br/>The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. |
  | `qs.pretty` | If &#39;true&#39;, then the output is pretty printed. |
  | `qs.resourceVersion` | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it&#39;s 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv. |
  | `qs.timeoutSeconds` | Timeout for the list&#x2F;watch call. This limits the duration of the call, regardless of any activity or inactivity. |
  | `qs.watch` | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. |

  ### apis.apiregistration.k8s.io.v1beta1.apiservices.get

  list or watch objects of kind APIService

  #### Query

  | Parameter | Description |
  | --------- | ----------- |
  | `qs` | Querystring object |
  | `qs.continue` | The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server the server will respond with a 410 ResourceExpired error indicating the client must restart their list without the continue field. This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. |
  | `qs.fieldSelector` | A selector to restrict the list of returned objects by their fields. Defaults to everything. |
  | `qs.includeUninitialized` | If true, partially initialized resources are included in the response. |
  | `qs.labelSelector` | A selector to restrict the list of returned objects by their labels. Defaults to everything. |
  | `qs.limit` | limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.<br/><br/>The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. |
  | `qs.resourceVersion` | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it&#39;s 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv. |
  | `qs.timeoutSeconds` | Timeout for the list&#x2F;watch call. This limits the duration of the call, regardless of any activity or inactivity. |
  | `qs.watch` | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. |
  | `qs.pretty` | If &#39;true&#39;, then the output is pretty printed. |

  ### apis.apiregistration.k8s.io.v1beta1.watch.apiservices.get

  watch individual changes to a list of APIService

  #### Query

  | Parameter | Description |
  | --------- | ----------- |
  | `qs` | Querystring object |
  | `qs.continue` | The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server the server will respond with a 410 ResourceExpired error indicating the client must restart their list without the continue field. This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. |
  | `qs.fieldSelector` | A selector to restrict the list of returned objects by their fields. Defaults to everything. |
  | `qs.includeUninitialized` | If true, partially initialized resources are included in the response. |
  | `qs.labelSelector` | A selector to restrict the list of returned objects by their labels. Defaults to everything. |
  | `qs.limit` | limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.<br/><br/>The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. |
  | `qs.pretty` | If &#39;true&#39;, then the output is pretty printed. |
  | `qs.resourceVersion` | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it&#39;s 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv. |
  | `qs.timeoutSeconds` | Timeout for the list&#x2F;watch call. This limits the duration of the call, regardless of any activity or inactivity. |
  | `qs.watch` | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. |

## write

  ### apis.apiregistration.k8s.io.v1.apiservices.delete

  delete collection of APIService

  #### Query

  | Parameter | Description |
  | --------- | ----------- |
  | `qs` | Querystring object |
  | `qs.continue` | The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server the server will respond with a 410 ResourceExpired error indicating the client must restart their list without the continue field. This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. |
  | `qs.fieldSelector` | A selector to restrict the list of returned objects by their fields. Defaults to everything. |
  | `qs.includeUninitialized` | If true, partially initialized resources are included in the response. |
  | `qs.labelSelector` | A selector to restrict the list of returned objects by their labels. Defaults to everything. |
  | `qs.limit` | limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.<br/><br/>The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. |
  | `qs.resourceVersion` | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it&#39;s 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv. |
  | `qs.timeoutSeconds` | Timeout for the list&#x2F;watch call. This limits the duration of the call, regardless of any activity or inactivity. |
  | `qs.watch` | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. |
  | `qs.pretty` | If &#39;true&#39;, then the output is pretty printed. |

  ### apis.apiregistration.k8s.io.v1.apiservices.post

  create an APIService

  #### Query

  | Parameter | Description |
  | --------- | ----------- |
  | `qs` | Querystring object |
  | `qs.pretty` | If &#39;true&#39;, then the output is pretty printed. |

  #### Body

  | Parameter | Description |
  | --------- | ----------- |
  | `body` | #&#x2F;definitions&#x2F;io.k8s.kube-aggregator.pkg.apis.apiregistration.v1.APIService |

  ### apis.apiregistration.k8s.io.v1beta1.apiservices.delete

  delete collection of APIService

  #### Query

  | Parameter | Description |
  | --------- | ----------- |
  | `qs` | Querystring object |
  | `qs.continue` | The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server the server will respond with a 410 ResourceExpired error indicating the client must restart their list without the continue field. This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. |
  | `qs.fieldSelector` | A selector to restrict the list of returned objects by their fields. Defaults to everything. |
  | `qs.includeUninitialized` | If true, partially initialized resources are included in the response. |
  | `qs.labelSelector` | A selector to restrict the list of returned objects by their labels. Defaults to everything. |
  | `qs.limit` | limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.<br/><br/>The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. |
  | `qs.resourceVersion` | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it&#39;s 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv. |
  | `qs.timeoutSeconds` | Timeout for the list&#x2F;watch call. This limits the duration of the call, regardless of any activity or inactivity. |
  | `qs.watch` | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. |
  | `qs.pretty` | If &#39;true&#39;, then the output is pretty printed. |

  ### apis.apiregistration.k8s.io.v1beta1.apiservices.post

  create an APIService

  #### Query

  | Parameter | Description |
  | --------- | ----------- |
  | `qs` | Querystring object |
  | `qs.pretty` | If &#39;true&#39;, then the output is pretty printed. |

  #### Body

  | Parameter | Description |
  | --------- | ----------- |
  | `body` | #&#x2F;definitions&#x2F;io.k8s.kube-aggregator.pkg.apis.apiregistration.v1beta1.APIService |

