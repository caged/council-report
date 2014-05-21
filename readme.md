### Process Portland City Council data

### Setup and run

Create a `.env` file in the root of the project and add the following information:

```
AWS_ACCESS_KEY_ID=YOUR AWS ID
AWS_SECRET_ACCESS_KEY=YOUR AWS KEY
AWS_S3_BUCKET=YOUR AWS BUCKET

```

Then install the dependencies and run the script.  This will process the upcoming
agenda items from the [City Council website](http://www.portlandonline.com/Auditor/Index.cfm?c=26997)
and upload the resutls as JSON to s3.

```
bundle install
dotenv script/process-upcoming-agenda-items
```
