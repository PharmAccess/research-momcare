Accessing Anonymized Data via DuckDB: https://momcareopensource.blob.core.windows.net/anonymized-fhir/momcare_anonymized.duckdb

To access an anonymized MomCare dataset stored remotely, a user can execute the following code. 

    sql
    ATTACH 'https://momcare_anonymized.pharmaccess.org' AS anonymizeddata;
    SELECT * FROM anonymizeddata.table_name;
