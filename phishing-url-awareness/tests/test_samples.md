# Test Results

**Python version used:** 3.13.5  
**Operating system:** Windows  
**Date:** 30/10/2026

| # | Input | Expected result | Actual result | Pass/Fail |
|---|---|---|---|---|
| 1 | https://www.example.com/login | No listed warning signs | No listed warning signs found | PASS |
| 2 | http://192.0.2.10/account | IP address + HTTP | IP address + HTTP warning | PASS |
| 3 | http://example.com@sample.invalid/login | @ symbol + HTTP | @ symbol + HTTP warning | PASS |
| 4 | https://a.b.c.d.e.example.invalid/path | Many hostname segments | Many hostname segments warning | PASS |
| 5 | https://xn--example.invalid/ | Punycode-style hostname | Punycode-style hostname warning | PASS |

## Notes

1. I learned how to identify common warning signs in URLs.
2. I learned that IP addresses, @ symbols, HTTP and punycode can be warning signs.
3. I was surprised that a URL showing no warning signs is not necessarily safe.
