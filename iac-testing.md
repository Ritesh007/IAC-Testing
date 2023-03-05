# IAC testing 
- Testing Infrastructure as code.

## Static Analysis
Static analysis is the process of analyzing software code without executing it.

- Complier/ parser/ Interpreter (validating the code, ex: `terraform validate`)
- Linter (checking IAC code for errors, warnings, and best practices. It has built-in rules that cover a wide range of issues, such as syntax errors, resource naming conventions, and security concerns, ex: `tflint`)
- Dry run (run the code but not executing it, ex: `terraform plan`)

## Unit Testing 
Testing a single unit of code in isolation. The equivalent of unit testing in IAC is testing a single module.
There is no pure unit testing for IAC like app code.
### Test Strategy:
1. Deploy the code in a real env.
1. Validate it works.
1. Undeploy the code.

Terratest can do all the above three steps.
example: https://github.com/gruntwork-io/infrastructure-as-code-testing-talk

To run the code: from the test folder run `go test`.


## Integration testing 

## End to end testing
