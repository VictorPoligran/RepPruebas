language: php

script:
    - vendor/bin/phpunit --coverage-clover coverage.xml

after_success:
    - bash <(curl -s https://codecov.io/bash)
