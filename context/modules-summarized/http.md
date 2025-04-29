# HTTP Module Summary
HTTP module provides functions for making HTTP requests and handling responses.
## Functions
* get(url, headers, params) - Creates a GET request
* delete(url, headers, params) - Creates a DELETE request
* head(url, headers, params) - Creates a HEAD request
* listen_and_serve(addr, handler) - Starts an HTTP server
* listen_and_serve_tls(addr, cert_file, key_file, handler) - Starts an HTTPS server
* patch(url, headers, body) - Creates a PATCH request
* post(url, headers, body) - Creates a POST request
* put(url, headers, body) - Creates a PUT request
* request(url, options) - Creates a custom HTTP request
## Types
* request - Has url, content_length, header attributes and send(), add_header(), add_cookie(), set_body(), set_data() methods
* response - Has status, status_code, proto, content_length, header, cookies, response attributes and json(), text(), close() methods
* response_writer - Has add_header(), del_header(), write(), write_header() methods
