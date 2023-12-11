from airflow import DAG -> How airflow knows this is a DAG

user_processing -> DAG id, must be unique across all tags in the airflow instance
start_date -> start_date defines the date at which your DAG starts
schedule_interval -> the frequency at which your DAG is triggered
catchup -> If it's set in True will run the non triggered DAG runs between this period of time between now and the start_date
