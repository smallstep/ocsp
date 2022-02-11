# ocsp

Fork of x/crypto/ocsp with some extra extensions.

Add it to your code running:

```console
go get go.step.sm/ocsp
```

## Changes

The changes added in this package are:

* Introduction of `Request.Extensions` with the parsed value of
  `requestExtensions`
  ([rfc6960#section-4.1.1](https://datatracker.ietf.org/doc/html/rfc6960#section-4.1.1))
  when parsing OCSP requests.
* Introduction of `Response.ResponseExtensions` with the parsed value of
  `responseExtensions`
  ([rfc6960#section-4.2.1](https://datatracker.ietf.org/doc/html/rfc6960#section-4.2.1))
  when parsing OCSP responses.
* Introduction of `Response.ResponseExtraExtensions`, which values will be
  populated in the `responseExtesions` field in the `CreateResponse` method.
