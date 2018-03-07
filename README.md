# Serafin Endre

Endre is a smoking cessation program for the [Serafin](https://github.com/inonit/serafin) web platform. It is provided here in its entirety, as exported on 2018-03-07.

## Getting started

You should have [Serafin](https://github.com/inonit/serafin) up and running, and preferably freshly initialized and migrated (see the Django management command `flush` if you need a clean slate).

Make sure the docker development setup for Serafin is running:

    $ docker-compose up

Copy the .json files to the Serafin directory so they are volumed into Serafin:

    $ cp <path to serafin-endre>/*.json <path to serafin>

In a separate terminal, import the data with the following command:

    $ docker-compose exec app ./manage.py loaddata system.json filer.base64.json

## License

Copyright (C) 2018 Håvar Brendryen and Marianne T. S. Holter. All rights reserved. This content is licensed under the AGPL v3 license, see [LICENSE.txt](LICENSE.txt) for details.
