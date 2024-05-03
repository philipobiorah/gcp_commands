# gcp_commands

### Executing Spark on Dataproc
- Initialization actions to install additional components on the cluster

```bash
gcloud dataproc clusters create <CLUSTER_NAME>  \
    --initialization-actions gs://$MY_BUCKET/hbase/hbase.sh \
        --num-masters 3 --num-workers 2
