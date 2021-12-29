#How to run application with newrelic tracking

- Run `composer install`
- edit .rr.yaml to set your application name and newrelic license key
- run `"vendor/bin/rr" get-binary` - see https://github.com/spiral/roadrunner for details
- run `./rr serve`
- open browser and navigate to `http://localhost:8081/`. Access page several times
- go to https://newrelic.com and login into your account
- go to APM tab and find "Default application" (see .rr.yaml)
- ensure that transactions are coming (Note: it may take a few minutes)