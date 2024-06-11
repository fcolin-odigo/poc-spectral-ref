```shell
npm install -g @stoplight/spectral-cli@6.11.1
```

```shell
$ spectral lint singlefile/openapi.yaml 

/home/francois/dev/projects/paas/poc-openapi-ref/singlefile/openapi.yaml
 1:1  warning  oas3-api-servers  OpenAPI "servers" must be present and non-empty array.

✖ 1 problem (0 errors, 1 warning, 0 infos, 0 hints)
```

```shell
$ spectral lint split/openapi.yaml 

/home/francois/dev/projects/paas/poc-openapi-ref/split/openapi.yaml
 1:1  warning  oas3-api-servers  OpenAPI "servers" must be present and non-empty array.

/home/francois/dev/projects/paas/poc-openapi-ref/split/paths/sample4-byId.yaml
 1:5  error  path-params  Operation must define parameter "{tenantId}" as expected by path "/tenants/{tenantId}/sample4/{id}".  get
 1:5  error  path-params  Operation must define parameter "{id}" as expected by path "/tenants/{tenantId}/sample4/{id}".        get

✖ 3 problems (2 errors, 1 warning, 0 infos, 0 hints)
```