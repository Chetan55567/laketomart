# laketomart

Data lake to Mart
Now build a Dataflow pipeline that reads data from 2 BigQuery data sources, and then joins the data sources. Specifically, you:

Ingest files from 2 BigQuery sources.
Join the 2 data sources.
Filter out the header row in the files.
Convert the lines read to dictionary objects.
Output the rows to BigQuery.


Make virtual environment and install apachebeam gcp.
Run this command to start a job

python data_lake_to_mart.py --worker_disk_type="compute.googleapis.com/projects//zones//diskTypes/pd-ssd" --max_num_workers=4 --project=$PROJECT --runner=DataflowRunner --staging_location=gs://$PROJECT/test --temp_location gs://$PROJECT/test --save_main_session --region=us-central1
