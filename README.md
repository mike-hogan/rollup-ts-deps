Repo to reproduce [Rollup issue 832](https://github.com/rollup/plugins/issues/832)

 * npm install
 * npx rollup -c

Yields 

```
[!] Error: Unexpected token (Note that you need plugins to import files that are not JavaScript)
node_modules/@http4t/core/requests.ts (5:30)
3: import {Authority, Uri, UriLike} from "./uri";
4: 
5: export function request(method: Method, uri: UriLike, body?: HttpBody, ...headers: Header[]): HttpRequest {
                                 ^
6:   return {
7:     method,
```
