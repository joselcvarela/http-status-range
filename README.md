#http-status-range
Check if HTTP status code is within range or is a specific code

###Instal
```sh
$npm install --save http-status-range
```

###Usage
```js
  import http from 'http-status-range'
  ...
  async someFn() {
    const r = await fetch('...')

    if (http.isInformational(r.status)) { ... } // Code is between 100 and 199
    else if (http.isSuccessful(r.status)) { ... } // Code is between 200 and 299
    else if (http.isRedirection(r.status)) { ... } // Code is between 300 and 399
    else if (http.isClientError(r.status)) { ... } // Code is between 400 and 499
    else if (http.isServerError(r.status)) { ... } // Code is between 500 and 599

  OR

    if(r.status === ACCEPTED) { ... }
    else if(r.status === BAD_GATEWAY) { ... }
    else if(r.status === BAD_REQUEST) { ... }
    else if(r.status === CONFLICT) { ... }
    else if(r.status === CONTINUE) { ... }
    else if(r.status === CREATED) { ... }
    else if(r.status === EXPECTATION_FAILED) { ... }
    else if(r.status === FAILED_DEPENDENCY) { ... }
    else if(r.status === FORBIDDEN) { ... }
    else if(r.status === GATEWAY_TIMEOUT) { ... }
    else if(r.status === GONE) { ... }
    else if(r.status === HTTP_VERSION_NOT_SUPPORTED) { ... }
    else if(r.status === IM_A_TEAPOT) { ... }
    else if(r.status === INSUFFICIENT_SPACE_ON_RESOURCE) { ... }
    else if(r.status === INSUFFICIENT_STORAGE) { ... }
    else if(r.status === INTERNAL_SERVER_ERROR) { ... }
    else if(r.status === LENGTH_REQUIRED) { ... }
    else if(r.status === LOCKED) { ... }
    else if(r.status === METHOD_FAILURE) { ... }
    else if(r.status === METHOD_NOT_ALLOWED) { ... }
    else if(r.status === MOVED_PERMANENTLY) { ... }
    else if(r.status === MOVED_TEMPORARILY) { ... }
    else if(r.status === MULTI_STATUS) { ... }
    else if(r.status === MULTIPLE_CHOICES) { ... }
    else if(r.status === NETWORK_AUTHENTICATION_REQUIRED) { ... }
    else if(r.status === NO_CONTENT) { ... }
    else if(r.status === NON_AUTHORITATIVE_INFORMATION) { ... }
    else if(r.status === NOT_ACCEPTABLE) { ... }
    else if(r.status === NOT_FOUND) { ... }
    else if(r.status === NOT_IMPLEMENTED) { ... }
    else if(r.status === NOT_MODIFIED) { ... }
    else if(r.status === OK) { ... }
    else if(r.status === PARTIAL_CONTENT) { ... }
    else if(r.status === PAYMENT_REQUIRED) { ... }
    else if(r.status === PERMANENT_REDIRECT) { ... }
    else if(r.status === PRECONDITION_FAILED) { ... }
    else if(r.status === PRECONDITION_REQUIRED) { ... }
    else if(r.status === PROCESSING) { ... }
    else if(r.status === PROXY_AUTHENTICATION_REQUIRED) { ... }
    else if(r.status === REQUEST_HEADER_FIELDS_TOO_LARGE) { ... }
    else if(r.status === REQUEST_TIMEOUT) { ... }
    else if(r.status === REQUEST_TOO_LONG) { ... }
    else if(r.status === REQUEST_URI_TOO_LONG) { ... }
    else if(r.status === REQUESTED_RANGE_NOT_SATISFIABLE) { ... }
    else if(r.status === RESET_CONTENT) { ... }
    else if(r.status === SEE_OTHER) { ... }
    else if(r.status === SERVICE_UNAVAILABLE) { ... }
    else if(r.status === SWITCHING_PROTOCOLS) { ... }
    else if(r.status === TEMPORARY_REDIRECT) { ... }
    else if(r.status === TOO_MANY_REQUESTS) { ... }
    else if(r.status === UNAUTHORIZED) { ... }
    else if(r.status === UNPROCESSABLE_ENTITY) { ... }
    else if(r.status === UNSUPPORTED_MEDIA_TYPE) { ... }
    else if(r.status === USE_PROXY) { ... }
  }
```

### Author
José Varela 

### Contibuting
Just fork this repo and open a PR.
