# Infrastructure

Brief guide to our infrastructure.

## Static page publishing

### Hosting

We use Amazon Web Services S3 to host static web pages. We have two buckets under an IT-maintained AWS account, a primary in us-east-1 and a mirror in us-west-2.

The primary bucket serves content through CloudFront and is reverse-proxied by an Akamai cache under [http://www.politico.com/interactives/](http://www.politico.com/interactives/).

### Publishing

We publish content to these buckets using our in-house [interactives generator app](https://github.com/The-Politico/generator-politico-interactives). The app includes [gulp](http://gulpjs.com/) tasks which handle publishing, cache invalidation and asset minimization and versioning.

## Dynamic web apps

### In-house apps

Our in-house Django applications tree is hosted by Heroku at [https://datalab.politico.com](https://datalab.politico.com). [See the repo for more details](https://github.com/The-Politico/django-politico-datalab).

### Public-facing apps

Public-facing apps are temporary. Wherever possible, try to create static data resources from dynamic databases by pushing JSON to AWS S3, cf. [White House Visitor Logs](https://github.com/The-Politico/django-politico-datalab/tree/master/visitorlogs). If possible, use AWS Lambda to handle incoming data. If all else fails, use a library like [django-bakery](https://github.com/datadesk/django-bakery).

For temporary apps, we can provision Elastic Beanstalk and EC2 instances on our separate interactives AWS account or can provision additional apps on PaaS providers like Heroku.

### Databases

We maintain a production database in AWS on a separate Amazon account owned by the Interactives Team. It is an AWS RDS t2.medium instance running PostgreSQL 9.6.1 with automated backups going back 14 days. We do not have a test database at this time.

