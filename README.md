# Setup

[![Build Status](http://54.72.23.130/job/property-api-unit-tests/badge/icon)](http://54.72.23.130/job/property-api-unit-tests/)

This is an app that should usually be run in the normal way (ie. using the
lr-\* scripts). However it is also possible to set it up and run it
independently.

To create a virtual env, run the following from a shell:

```
    mkvirtualenv -p /usr/bin/python3 property-api
    source environment.sh
    pip install -r requirements.txt
```

To run it, activate its virtual environment, source the environment.sh file,
and execute it:

```
    workon property-api
    . ./environment.sh && ./run_dev.py
```

## Dependencies

```bash
-bash-4.2$ python3 --version
Python 3.4.1
```

[ElasticSearch](http://www.elasticsearch.org) provides the search functionality, and must be running at the $ELASTIC_SEARCH_ENDPOINT listed in the environment variables.

